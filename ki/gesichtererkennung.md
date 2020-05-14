# Gesichtererkennung

i>Die folgenden Beispiele kannst du dank der [face-api.js](https://github.com/justadudewhohacks/face-api.js) von [justadudewhohacks](https://github.com/justadudewhohacks) [**hier**](https://justadudewhohacks.github.io/face-api.js/face_and_landmark_detection) ausprobieren. (Beachte, dass dafür wirklich viele Daten runtergeladen werden müssen.)

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



## Eine virtuelle Clownsnase aufsetzen.

Hast du schonmal in die Wolken gesehen oder die Raufasertapete interessiert gemustert und plötzlich ein Gesicht gesehen? Das ist ganz normal. Für Menschen ist es sehr wichtig Gesichter zu sehen, daher kann das schonmal sein, dass wir da ein wenig über das Ziel hinaus schießen. Folglich hat man das auch sehr schnell den Rechnern beigebracht.

Hier werden wir uns eine virtuelle Clownsnase aufsetzen:

<div class="plyr__video-embed" id="player">
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/mN__yB4-P-4?origin=https://buch.informatik.cc&amp;iv_load_policy=3&amp;modestbranding=1&amp;playsinline=1&amp;showinfo=0&amp;rel=0&amp;enablejsapi=1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

<figcaption>Video bei <a href="https://youtu.be/mN__yB4-P-4">YouTube</a> ansehen </figcaption>

Hinweis: Dein Kamerabild wird auf deinem Rechner verarbeitet, du musst dir also keine Sorgen machen, dass es im Internet landet. Du kannst das Internet in der Zeit auch von dir trennen.

t> Expertenaufgabe: Schaffst du es anstelle des Kreises einen Smilie passend über dein Gesicht zu legen.

Du fragst dich wie viele Gesichter sich eine künstliche Intelligenz ansehen musste, um diese sicher zu erkennen? Nunja mehr ist besser, aber hier waren es über 32.000 Photos mit darauf 390.000 Gesichtern.

## lokal Ausprobieren

i> Hier ist eine [Online-Demonstration](https://justadudewhohacks.github.io/face-api.js/face_and_landmark_detection).

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