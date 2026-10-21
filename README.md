# Fencingworldwide Referees – aktuelle Builds

Auf der obersten Ebene stehen nur die neuesten Pakete je Plattform.
Ältere Versionen bleiben unverändert im [Archive](Archive/) erhalten.

## Aktuelle Pakete

| Plattform | Version / Build | Download |
|---|---|---|
| macOS Apple Silicon | 1.4 / 33 | [ZIP](Fencingworldwide-Referees-macOS-arm64-v1.4-build33.zip) |
| Windows x64 | 1.4 / 33 | [ZIP](Fencingworldwide-Referees-Windows-x64-v1.4-build33.zip) |
| Android | 1.1 / 13 | [APK](Fencingworldwide-Referees-Android-v1.1-build13.apk), [Play-Store-Bundle](Fencingworldwide-Referees-Android-v1.1-build13.aab) |

Die Desktop-Version 1.4 ergänzt den App-Zugang per QR für Kampfrichtende ohne
Ophardt-Konto. Anmeldecodes sind eine Stunde gültig und einmal verwendbar.
Die Python-App kann einzelne Codes und mehrere markierte Personen auf A4
zum Drucken ausgeben, jeweils mit dem Namen unter dem Code und Ablaufzeit.
Android 1.1 und iOS 1.6 (Build 26) können diese Anmeldecodes scannen und
anschließend die normalen Gefechts-, Push- und Ergebnisfunktionen verwenden.
Die neue Serverversion muss für die QR-Anmeldung ebenfalls bereitgestellt sein.

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
hier liegt kein IPA-Paket.

## Quellcode und Builds

- [Desktop und Push-Server](https://github.com/bebeckmann/fencingworldwide-referees)
- [Android](https://github.com/bebeckmann/fencingworldwide-referees-android)
- [iOS](https://github.com/bebeckmann/fencingworldwide-referees-ios)
- [Windows-Build](https://github.com/bebeckmann/fencingworldwide-referees/actions/runs/39644695314)

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
