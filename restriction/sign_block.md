# `es.MultiBlock.Sign.Text` risks

# security risks

## bad texts

some texts, such as bad word or NSFW ASCII art, may be exposed to players as is.

## malicious URLs

some URLs may lead players to harmful websites.

# runtime risks

## `move` misuse

`move` may inject `NaN` values into internal scripts.

## memory overflow

a very heavy text, such as 1 TB, may overflow RAMs.

## reduced FPS

a text, such as `<quad>`, may reduces FPS.

## broken text rendering

a text, such as `<quad>` or Zargo, may breaks text rendering.