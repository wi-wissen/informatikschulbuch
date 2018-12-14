# Gesichtererkennung

i> Bisher war es ziemlich schwierig selbst mit künstlichen neuronalen Netzen zu arbeiten. Daher haben Entwickler das eigentliche TensorFlow.js noch weiter vereinfacht. Ein Projekt heißt [face-api.js](https://github.com/justadudewhohacks/face-api.js). 

![bbt-0](img/bbt-0.jpeg)

Gesichter zu erkennen lässt sich praktisch in drei Schritte einteilen:

1. Gesichter verorten
2. Gesichter normalisieren
3. Gesichter einer Gruppe von bekannten Gesichtern zuordnen

Der erste Schritte ist der einfachste. Schon recht alte digitale Kameras konnten Gesichter aufgrund ihrer Form auf Bildern identifizieren.

![bbt-1](img/bbt-1.jpeg)

Im zweiten Schritt soll das Gesicht so gedreht und zugeschnitten werden, dass nur die für den dritten Schritt relevanten Teile zu erkennen sind. Dazu werden die folgenden markanten Punkte ermittelt:

![bbt-2](img/bbt-2.png)

So sieht dann in etwa das Ergebnis aus:

![bbt-2-1](img/bbt-2-1.png)

Jetzt werden die Gesichter mit einer Auswahl (hier sind es 20, für ein Video wären mehrere hundert gut) verglichen:

![bbt-3-1](img/bbt-3-1.png)

Das Endergebnis kann dann etwa wie folgt visualisiert werden:

![bbt-final](img/bbt-final.png)

w> Alle Bilder sind Eigentum der jeweiligen Urheber. [Der vollständige Artikel](https://itnext.io/face-api-js-javascript-api-for-face-recognition-in-the-browser-with-tensorflow-js-bcc2a6c4cf07) ist auf englisch bei itnext.io verfügbar.



## Ausprobieren

i> Das Ausprobieren ist diesmal nicht ganz so einfach, da hier ein node-Server benötigt wird. Aus rechtlichen Gründen wird im moment kein öffentlicher Server bereitgestellt.

**Vorbereitung**

Installiere [node](https://nodejs.org/de/) und [git](https://git-scm.com/downloads)

Öffne eine Kommandozeile (etwa im Startmenu nach `cmd` suchen) und gib folgende Befehle ein:

w> Alle Dateien werden in den aktuellen Ordner gelegt. Das ist oft `C:\User\DEINNAME`. Möchtest du das nicht, musst du den Ordner wechseln oder die Dateien im Anschluss löschen.

```bash
git clone https://github.com/justadudewhohacks/face-api.js.git
cd examples
npm i
npm start
```

Jetzt kannst du <http://localhost:3000/> aufrufen und mit kurzer Verzögerungszeit die Gesichtserkennung beim Arbeiten beobachten.