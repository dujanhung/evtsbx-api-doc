# `es.MultiBlock.Sign.Text` risks

# <a id="minimap"/> minimap

╠╦ [security risks](#securityRisks)<br>
┃┣╾ [bad texts](#securityRisks_badTexts)<br>
┃┗╾ [malicious URLs](#securityRisks_maliciousURLs)<br>
╠╦ [runtime risks](#runtimeRisks)<br>
┃┣╾ [corruption](#runtimeRisks_corruption)<br>
┃┣╾ [OOM](#runtimeRisks_OOM)<br>
┃┣╾ [reduced FPS](#runtimeRisks_reducedFPS)<br>
┃┗╾ [broken text rendering](#runtimeRisks_brokenTextRendering)

# <a id="securityRisks"/> security risks

[⛖](#minimap)

## <a id="securityRisks_badTexts"/> bad texts

some texts, such as bad word or NSFW ASCII art, may be exposed to players as is.

[⛖](#minimap)

## <a id="securityRisks_maliciousURLs"/> malicious URLs

some URLs may lead players to harmful websites.

[⛖](#minimap)

# <a id="runtimeRisks"/> runtime risks

[⛖](#minimap)

## <a id="runtimeRisks_corruption"/> corruption

`move` may inject `NaN` values into internal scripts.

[⛖](#minimap)

## <a id="runtimeRisks_OOM"/> OOM

a very heavy text, such as 1 TB, may overflow RAMs.

[⛖](#minimap)

## <a id="runtimeRisks_reducedFPS"/> reduced FPS

`<quad>` may reduces FPS.

[⛖](#minimap)

## <a id="runtimeRisks_brokenTextRendering"/> broken text rendering

`<quad>` may overflow.

<img src="https://github.com/dujanhung/evtsbx-gallery/blob/main/meme/rain.jpg"/>

[⛖](#minimap)
