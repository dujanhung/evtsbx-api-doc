# `es.MultiBlock.Sign`

## 🛡️ security risk

**`Sign` blocks can't sanitize it's own content**.

loading `Sign` blocks from untrusted sources may expose the runtime to:

- malicious URLs
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
