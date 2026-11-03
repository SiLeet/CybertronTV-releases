# CybertronTV — Downloads

Fertige Windows-Programme von **CybertronTV**, dem Netzwerk-Scanner & TV-Unlocker (Full Rust).
Dieses Repository enthält nur die veröffentlichten Programme; der Quellcode wird separat gepflegt.

**Neueste Version:** [Releases → Latest](https://github.com/SiLeet/CybertronTV-releases/releases/latest)

## Installation
- `CybertronTV-vX.Y.Z-windows-x64.zip` herunterladen und in einen eigenen Ordner entpacken (z. B. unter Dokumente). Keine Installation nötig.
- `CybertronTV.exe` startet die Oberfläche; `CybertronTV-console.exe` ist für Befehle in cmd/PowerShell (`--help`).
- Voraussetzung: Windows 10 oder 11, 64 Bit.

## SmartScreen
Die Programme sind nicht signiert. Windows zeigt beim ersten Start „Der Computer wurde durch Windows geschützt“ → **Weitere Informationen** → **Trotzdem ausführen**.

## Prüfsumme
Jedes Release enthält `SHA256SUMS`. In PowerShell:

```powershell
Get-FileHash .\CybertronTV-vX.Y.Z-windows-x64.zip -Algorithm SHA256
```

## Updates
Ab Version 1.2.0 prüft CybertronTV beim Start, ob hier eine neue Version liegt, und bietet „Jetzt aktualisieren“ an (abschaltbar im Über-Dialog). Die neue Exe wird per SHA-256 geprüft, bevor sie die alte ersetzt.

## Lizenz
MIT — siehe [LICENSE](LICENSE).
