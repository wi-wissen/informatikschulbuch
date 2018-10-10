# Layout mit CSS

<div class="alert alert-warning"><p>Für HTML und CSS werden neue Sprachversionen veröffentlicht. Hier kommen neue Funktionen dazu und neue verbindliche Sprachelemente werden definiert (Ein klein wenig wie ein neuer Duden oder die neue deutsche Rechtschreibung.).</p><p>Webbrowser unterstützen in verschiedenen Versionen verschiedene Sprachversionen und manchmal leider auch eigene Dialekte.</p><p>Die hier vorgestellte Lösung wird u.a. von Firefox ab Version 52, Chrome ab Version 57, Edge ab Version 16 und Safari ab Version 10.1 (alle im Frühjahr bis Sommer 2017 erscheinen) unterstützt. Ältere Browser oder etwa der Internet Explorer sprechen eigene Dialekte oder kennen die Funktion nicht.</p></div>
## Das unsichtbare Netz

### [Flexbox](https://wiki.selfhtml.org/wiki/CSS/Eigenschaften/Flexbox)

[Sehr viele Browser](http://caniuse.com/#feat=flexbox) können mit Flexbox oder etwa mit Frameworks wie [Bootstrap](http://getbootstrap.com/) (welches [ab Version 4](https://v4-alpha.getbootstrap.com/layout/grid/) auf Flexbox aufbaut) unterstützt werden.

### [Grid](https://wiki.selfhtml.org/wiki/CSS/Eigenschaften/grid)

Grid (zu deutsch Gitter) wird über die gesamte Webseite oder einen Teil davon gelegt. Anschließend können daran Elemente ausgerichtet werden:

![img](/img/10-1.png)

Im Folgenden soll anhand obiger Darstellung gezeigt werden, wie dies in HTML und CSS umgesetzt werden kann:

```html
<body>
	<header>Überschrift</header>
	<nav>Navigation</nav>
	<main> Lorem ipsum dolor sit amet, consetetur sadipscing elitr, ...</main>
</body>
```

Zuerst erklären wir, dass wir mithilfe des Gitters arbeiten möchten:

```css
body {
	display: grid;
}
```

Alles innerhalb des body wird nun am Gitter ausgerichtet.

Nun beschreiben wir unser Gitter:

```css
body {
	display: grid;
	grid-template-rows: 1fr 1fr 1fr 1fr 1fr 1fr 1fr ;
	grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr 1fr;
}
```

Hier wurden 7 Zeilen (`rows`) und 7 Spalten (`colums`) angelegt. Alle Zellen sollen gleich groß sein. Daher sind diese alle `1fr` groß. `fr` ist eine neue Einheit. Sie errechnet sich automatisch aus der Anzahl der Spalten bzw. Zeilen. Hier gilt  `1fr` = 100%/7 = `14,28%`.

```css
grid-template-rows: 1fr 2fr 1fr;
```

Hier ist die mittlere Spalte doppelt so breit wie die anderen beiden. Du hättest auch `25% 50% 25%` schreiben können.

Absolute Breiten gehen natürlich auch, da Bildschirme sehr verschiedene Auflösungen und Pixeldichten haben, musst du hier genau nachdenken. Absolute Größen sind etwa sinnvoll, wenn du eine Navigationsliste erstellst und diese unabhängig von den anderen Elemente eine feste Höhe haben soll.

 

## Jedes hat seinen Platz

In dem erstellten Gitter beschreiben wir nun, wo unsere Überschrift sein soll:

```css
header {
	grid-row: 1;
	grid-column-start: 3;
	grid-column-end: 6;
}
```

Die Überschrift ist in der 1. Zeile (es wird nicht von 0 sondern von 1 losgezählt). Sie beginnt in der 3. Spalte und endet genau vor der 6. Spalte. Folglich geht die Überschrift von der 3. bis zur 5. Spalte.

Den Text positionierst du mit

```css
main {
	grid-row-start: 3;
	grid-row-end: 8;
	grid-column-start: 2;
	grid-column-end: 7;
}
```

An den beiden obigen Beispielen siehst du gut eine Kurzschreibweise: Erstreckt sich ein Element nur innerhalb einer Spalte oder Zeile, so reicht `grid-row` bzw. `grid-column`. Soll es mehrere umfassen, wird mit `–start` und `–end` gearbeitet. Es gibt noch weitere Schreibweisen, die im Endeffekt zum gleichen Ergebnis führen.

t> Übernimm die CSS-Befehle in den [Editor](https://apps.wi-wissen.de/html-css-js-editor/13pRy)

t> Schreibe selbst das CSS für `nav`

t> Übe deine Fähigkeiten, indem du im [Grid Garden](http://cssgridgarden.com/#de) die Pflanzen bis Level 6 wässerst.

t> Experten: Schaffe möglichst viele Level!

Weiterführende Artikel:

* <https://wiki.selfhtml.org/wiki/CSS/Eigenschaften/grid>
* <http://maddesigns.de/css-grid-layout-2764.html>

s> Glückwunsch! Du hast nun erweiterte Fähigkeiten in CSS erworben!

t> Wende all dein Wissen und Geschick aus den vorangegangenen Kapiteln auf das Erweitern deiner Filmwebseite mit der letzten Aufgabe an.