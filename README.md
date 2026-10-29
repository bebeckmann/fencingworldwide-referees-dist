# Fencingworldwide Referees – aktuelle Builds

Auf der obersten Ebene stehen nur die neuesten Pakete je Plattform.
Ältere Versionen bleiben unverändert im [Archive](Archive/) erhalten.

## Aktuelle Pakete

| Plattform | Version / Build | Download |
|---|---|---|
| macOS Apple Silicon | 1.4 / 34 | [ZIP](Fencingworldwide-Referees-macOS-arm64-v1.4-build34.zip) |
| Windows x64 | 1.4 / 35 | [ZIP](Fencingworldwide-Referees-Windows-x64-v1.4-build35.zip) |
| Android | 1.1 / 16 | [APK](Fencingworldwide-Referees-Android-v1.1-build16.apk), [Play-Store-Bundle](Fencingworldwide-Referees-Android-v1.1-build16.aab) |

Desktop Build 34 ergänzt die Check-in-Rückmeldung in der Smartphone-App,
die genaue KO-Stufe, alle eingeteilten Kampfrichter und die Übertragung
begründeter Ergebniskorrekturen. Für Rundengefechte bestätigt der Kampfrichter
zuerst alle Fechter über die Anwesenheitsliste.
Windows Build 35 verpackt den aktuellen Desktop-Quellstand als portable
Einzeldatei; der eingebettete Selbsttest ist erfolgreich.

Android Build 16 und iOS Build 29 enthalten diese Funktionen, den Datenschutz-Link
und neun Sprachen: Deutsch, Englisch, Französisch, Portugiesisch, Italienisch,
Spanisch, Schwedisch, Dänisch und Norwegisch (Bokmål). Die Geräte-/App-Sprache
entscheidet; Englisch ist die Ersatzsprache. Der Cloud-Dienst ist aktualisiert.

Der App-Zugang per QR bleibt enthalten: Anmeldecodes sind eine Stunde gültig
und einmal verwendbar. Ein Ophardt-Konto ist für diese Anmeldung nicht nötig.

## Installation

macOS: ZIP entpacken und die App auf Apple Silicon ab macOS 13 starten.
Python muss nicht separat installiert sein. Die App ist lokal signiert und
nicht durch Apple notarisiert. Beim ersten Start kann Rechtsklick → „Öffnen“
erforderlich sein.

Windows: ZIP vollständig entpacken und `Fencingworldwide Referees.exe` starten.
Python muss nicht separat installiert sein. Das Paket wurde auf einem
Windows-Runner gebaut und mit dem eingebetteten Selbsttest geprüft.

Android: APK als Update installieren, damit lokale App-Daten erhalten bleiben.
Die signierte AAB ist für die Play Console und wird nicht direkt installiert.
iOS wird weiterhin über Xcode beziehungsweise TestFlight verteilt;
hier liegt kein IPA-Paket. Der aktuelle iOS-Quellcode hat Build 29.

## Quellcode und Builds

- [Desktop und Push-Server](https://github.com/bebeckmann/fencingworldwide-referees)
- [Android](https://github.com/bebeckmann/fencingworldwide-referees-android)
- [iOS](https://github.com/bebeckmann/fencingworldwide-referees-ios)
- [Windows-Build](https://github.com/bebeckmann/fencingworldwide-referees/actions/runs/40835588867)

Das Desktop-Repository enthält `scripts/publish_dist.py`. Dieses Skript
übernimmt neue Pakete, verschiebt ältere Versionen nach `Archive/<Plattform>/`
und aktualisiert die Prüfsummen. Pro Plattform bleibt ausschließlich die
neueste Version im Hauptverzeichnis. Gleiche Versionsnamen mit abweichendem
Inhalt werden nicht überschrieben.

## Download und Prüfsummen

Große Pakete werden über Git LFS gespeichert. Nach dem Klonen `git lfs install`
und `git lfs pull` ausführen. Auf GitHub die gewünschte Datei öffnen und
„Download raw file“ verwenden. [SHA256SUMS](SHA256SUMS) enthält die SHA-256-
Prüfsummen der aktuellen und archivierten Pakete mit ihren jeweiligen Pfaden.
