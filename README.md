# Fencingworldwide Referees – Builds

Dieses Repository enthält portable Desktop-Anwendungen und signierte Android-Pakete.
Die aktuellen Quellstände liegen in den separaten Repositories für
[Desktop und Push-Server](https://github.com/bebeckmann/fencingworldwide-referees),
[Android](https://github.com/bebeckmann/fencingworldwide-referees-android) und
[iOS](https://github.com/bebeckmann/fencingworldwide-referees-ios).

## Aktuelle Pakete

| Plattform | Version / Build | Datei |
|---|---|---|
| macOS Apple Silicon | 1.3 / 32 | [ZIP](Fencingworldwide-Referees-macOS-arm64-v1.3-build32.zip) |
| Android | 1.0 / 12 | [APK](Fencingworldwide-Referees-Android-v1.0-build12.apk), [Play-Store-Bundle](Fencingworldwide-Referees-Android-v1.0-build12.aab) |
| Windows x64 | 1.3 / 32 | [ZIP](Fencingworldwide-Referees-Windows-x64-v1.3-build32.zip) |

Der macOS-Build 31 enthält die Korrekturen für Ergebnisbestätigung je Fechter
und die KO-Übertragung anhand der tatsächlichen Touch-Formularfelder.
Der macOS-Build 32 ergänzt dauerhafte rotierende Laufzeitlogs und detaillierte
Push-Zustellungsdiagnosen.
Android-Build 12 entspricht dem aktuellen Android-Quellstand.
Der Windows-Build 31 enthält ebenfalls den aktuellen Desktop-Quellstand mit
diesen Ergebnis- und KO-Korrekturen. Ältere Pakete bleiben zur
Nachvollziehbarkeit erhalten.
Der Windows-Build 32 ergänzt getrennte Hinweise und Logeinträge für abgelehnte
Anmeldungen und Verbindungsfehler. Die Login-Logdatei liegt unter
`%APPDATA%\Ophardt Referees\ophardt-referees.log`.

## Installation

macOS: ZIP entpacken und die App auf Apple Silicon ab macOS 13 starten.
Python muss nicht separat installiert werden. Beim ersten Start kann
Rechtsklick → „Öffnen“ erforderlich sein, da die App lokal signiert,
aber nicht durch Apple notarisiert ist.

Android: Die APK als Update installieren, damit lokale App-Daten erhalten bleiben.
Die AAB ist für den Upload in die Play Console bestimmt und wird nicht direkt installiert.
iOS wird über Xcode beziehungsweise TestFlight verteilt; hier liegt kein IPA-Paket.

Windows: ZIP entpacken und `Fencingworldwide Referees.exe` starten.

## Download und Prüfsummen

Die großen Pakete werden über Git LFS gespeichert. Beim Klonen `git lfs install`
und anschließend `git lfs pull` ausführen. Auf GitHub die jeweilige Datei öffnen
und über „Download raw file“ herunterladen.
Die SHA-256-Prüfsummen stehen in [SHA256SUMS](SHA256SUMS).
