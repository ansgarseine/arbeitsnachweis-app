# Arbeitsnachweis App

Statische, buildfreie Offline-PWA für Arbeitsnachweise mit wasserzeichenversehenen Beweisfotos, optionaler GPS-Position und optionaler Kundenunterschrift.

## Lokal testen

`index.html` über einen lokalen Webserver öffnen. Für Kamera, Standort, PWA-Installation und Offline-Cache ist eine sichere Verbindung erforderlich (HTTPS oder `localhost`).

## GitHub Pages

1. Die Dateien in das Repository hochladen.
2. Unter **Settings → Pages** als Quelle den Branch `main` und den Ordner `/ (root)` auswählen.
3. Die veröffentlichte HTTPS-Adresse einmal online aufrufen. Danach cached der Service Worker die App-Dateien für die Offline-Nutzung.

Ein Build- oder Installationsschritt ist nicht erforderlich. jsPDF ist lokal enthalten; `logo-data.js` enthält das Firmenlogo als eingebettete PNG-Base64-Daten. Die Lizenz der mitgelieferten jsPDF-Datei liegt in `jspdf-LICENSE.txt`.

Arbeitsnachweise und Fotos werden lokal verarbeitet und nicht an einen Server übertragen. Nur der zuletzt eingegebene Monteurname wird im lokalen Browserspeicher gemerkt.
