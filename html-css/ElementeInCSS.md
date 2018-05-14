# Elemente in CSS

Bisher sahen unsere Webseiten noch alle sehr gleich aus. Es wird Zeit frischen Wind reinzubringen und unsere Webseiten nach unseren Wünchen zu stylen!

## Grundlagen

Um abweichend von dem Browser vorgeschlagenen Aussehen, dies anzupassen gibt es die CSS-Sprache. Mit dieser wird beschrieben, wie die Webseite aussehen soll:

```html
<h1>grüne Überschrift</h1>
```

```css
h1 {
	color:green;
}
```

t> Gib obiges Beispiel in den [Editor](https://apps.wi-wissen.de/html-css-js-editor/) ein.					

In obigen Beispiel wurde die Überschrift anstelle der vom Browser vorgeschlagenen schwarzen Farbe in grün geschrieben.

Dies liegt daran, dass wir in CSS die Eigenschaft `color` mit dem Eigenschaftswert `green` belegt haben. (Da green ein Schlüsselwort ist muss es nicht, wie in ähnlichen Situationen, in Anführungszeichen gesetzt werden.

Grundsätzlich ist eine HTML-Element-Beschreibung in CSS immer wie folgt aufgebaut:

```css
Element {
	Attribut1: Attributwert1; 
	Attribut2: Attributwert2;
}
```

Nach dem das Element benannt wurde (etwa `body` oder `h1`), wird mit den geschweiften Klammern `{}` Beginn und Ende der Eigenschaften für das Element angezeigt. mit `Attribut1: Attributwert1` wird dem Attribut ein Wert zugewiesen. Das Semikolon `;` beendet die aktuelle Zuweisung und ermöglicht eine weitere.

## Elemente adressieren

In obigen Beispiel haben wir alle Überschriften `h1` grün gefärbt. Oft ist das nicht gewollt und man möchte nur spezielle Elemente ansprechen. Dafür gibt es zwei Möglichkeiten:

## `class`

```html
<h1 class="gruen">grüne Überschrift</h1>
```

```css
.gruen {
	color:green;
}
```

Hier werden nur alle Überschriften grün gefärbt, welche bei dem Attribut `class` den Attrributwert `gruen` haben.

## `id`

```html
<h1 id="top">grüne Überschrift</h1>
```

```css
#top {
	color:green;
}
```

Hier darf es nur ein einziges Element geben. Dieses wird ähnlichen Beispiel mit `id` gekennzeichnet. Dadurch wird etwa derhindert, dass mehrmals eine oberste Überschrift ausgerufen wird.

Beachte, dass einmal das Element direkt genannt wurde, sowie diesen entweder ein `.` oder `#` vorgestellt wurde.

t> Übernimm das Beispiel `class`  in den [Editor](https://apps.wi-wissen.de/html-css-js-editor/). 

t> Ändere die Farbe von grün auf rot.

## HTML und CSS zusammenfügen.

Um die CSS-Befehle mit dem HTML-Dokument zu verknüpfen gibt es zwei Möglichkeiten. Beide Möglichkeiten werden im `head` des HTML-Dokumentes umgesetzt, da die Befehle ja nicht angezeigt, sondern ausgeführt werden sollen.

### CSS in HTML einbetten

```html
<style> 
	h1 {
		color:green;
	} 
</style>
```

Hier wird ein HTML-Element namens style im `head`-Bereich des HTML-Dokuments geöffnet. Darin kann CSS geschrieben werden.

### Aus HTML auf CSS verweisen

```html
<link href="css/style.css" rel="stylesheet">
```

Hier wird für die CSS-Befehle eine extra Datei namens style.css im Unterordner css abgelgt. (Beachte Kapitel Verweise in HTML)

t> Erstelle im head deiner Filmwebseite ein CSS-Element.

t> Übernimm darin das Beispiel und prüfe, dass deine Überschriften 1. Grades (`h1`) grün geworden sind. 