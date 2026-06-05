> [!CAUTION]
>
> ### 🛡️ security risk
>
> the text renderer does **NOT** perform validation or sanitization by itself.
>
> loading sign data from untrusted sources may expose the runtime to:
> - malicious hyperlinks
> - remote code execution
> - memory exhaustion (OOM) via oversized text buffers
> - excessive `<quad>` tag rendering
> - excessive Unicode characters rendering.
>
> **only load sign data from trusted save files or verified multiplayer environments**.

>[!CAUTION]
>
> ### ☢️ runtime stability
>
>
> editing large contents directly in-game is not recommended.
>
> observed risks include:
> - interruptions caused by ADs
> - external apps switching triggered by ADs
> - forced application restart caused by OOM
>
> **these interruptions may result in lost or corrupted sign data**.

>[!TIP]
>
> for safer sign contents editing, users must:
>
> - prepare contents in an external file
> - paste contents from clipboard
> - disable network connectivity
> - use devices with sufficient RAM (16 GB recommended)