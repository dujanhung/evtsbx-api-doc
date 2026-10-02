# `es.MultiBlock.Sign` risks

# <a id="minimap"/> minimap

╠╦ [security risks](#securityRisks)<br>
┃┣╾ [bad texts](#securityRisks_badTexts)<br>
┃┗╾ [malicious URLs](#securityRisks_maliciousURLs)<br>
╠╦ [runtime risks](#runtimeRisks)<br>
┃┣╾ [corruption](#runtimeRisks_corruption)<br>
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

## <a id="runtimeRisks_corruption"/> memory corruption

`move` may inject `NaN` values.

[⛖](#minimap)

## <a id="runtimeRisks_brokenTextRendering"/> broken text rendering

`<quad>` may break rendering.

<img src="https://github.com/dujanhung/evtsbx-gallery/blob/main/meme/rain.jpg"/>

[⛖](#minimap)
