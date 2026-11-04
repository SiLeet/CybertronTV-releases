# CybertronTV — Downloads

Fertige Windows-Programme von **CybertronTV**, dem Netzwerk-Scanner & TV-Unlocker (Full Rust).
Dieses Repository enthält nur die veröffentlichten Programme; der Quellcode wird separat gepflegt.

**Neueste Version:** [Releases → Latest](https://github.com/SiLeet/CybertronTV-releases/releases/latest)

## Installation
- `CybertronTV-vX.Y.Z-windows-x64.zip` herunterladen und in einen eigenen Ordner entpacken (z. B. unter Dokumente). Keine Installation nötig.
- `CybertronTV.exe` startet die Oberfläche; `CybertronTV-console.exe` ist für Befehle in cmd/PowerShell (`--help`).
- Voraussetzung: Windows 10 oder 11, 64 Bit.

## Kurzanleitung zum Ausdrucken
„In 10 Minuten startklar“ – je eine A4-Seite:
- [Kurzanleitung-DE.pdf](https://github.com/SiLeet/CybertronTV-releases/releases/latest/download/Kurzanleitung-DE.pdf) (Deutsch)
- [Kurzanleitung-RU.pdf](https://github.com/SiLeet/CybertronTV-releases/releases/latest/download/Kurzanleitung-RU.pdf) (Русский)

Beide liegen ab Version 1.4.0 auch im ZIP.

## Erste Schritte
1. **Scannen:** Netz eintragen (z. B. `192.168.178.0/24`) oder „Lokale Netze erkennen“ → „Scan starten“. Fernseher erscheinen oben in der Liste. Der TV muss eingeschaltet sein.
2. **TV auswählen:** Zeile anklicken — rechts erscheinen Infos, Fernbedienung und eine Schritt-für-Schritt-Anleitung für genau diese Marke.
3. **Freischalten (einmalig):**
   - *Android / Google / Fire TV:* Entwickleroptionen + Debugging am TV einschalten (Anleitung im Programm), dann „ADB verbinden“.
   - *Samsung:* am TV Apps » `12345` » Developer Mode EIN » Host-PC-IP eintragen » TV neu starten; dann „sdb automatisch holen“ und „TizenTube installieren“.
4. **Gratis-Apps:** „Standard-Apps herunterladen“ (SmartTube = YouTube ohne Werbung, Kodi, Stremio) → „APKs installieren…“. Weitere Tipps im Programm unter „Frei schauen (ohne Abo)“ und „Русский / Russisch“.

## Hilfe
Klappt etwas nicht: **Einstellungen → Log-Ordner öffnen** und die Logdatei von heute schicken (`%APPDATA%\CybertronTV\logs`, ohne Passwörter und Tokens). Ab Version 1.4.0.

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
