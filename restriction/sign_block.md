# `es.MultiBlock.Sign`

## 🛡️ security risk

the text renderer does **NOT** perform validation or sanitization by itself.

loading sign data from untrusted sources may expose the runtime to:

- malicious hyperlinks
- remote code execution
- memory exhaustion

**only load sign data from trusted sources or locked multiplayer rooms**.

## ☢️ runtime stability

editing large contents directly in-game is not recommended.

observed risks include:

- interruptions caused by ADs
- external apps switching triggered by ADs
- forced application restart caused by OOM

**these interruptions may result in lost or corrupted sign data**.
