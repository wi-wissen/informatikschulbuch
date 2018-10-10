# Listen und Tabellen in HTML

## Listen

```html
<ul>
	<li>Listenelement 1</li>
	<li>Listenelement 2</li>
</ul>
```

Eine Liste besteht aus einem Element `<ul></ul>` , welches alle Listenelemente kapselt. Ein einzelner Anstrich wird mit einem `<li></li>` angegeben.

`<ul>` ist die Abkürzung für unordered list, also einer ungeordneten Liste. Möchtest du deine Liste geordnet, also mit 1. und 2., so nimmst du stattdessen `<ol>` , was die Abkürzung für ordered List ist.

t> Erstelle eine sortierte Liste deiner Lieblingsgerichte. 
t> Erstelle eine unsortierte Liste mit 5 Farben.

## Tabelle

Eine Tabelle besteht aus mehreren Zellen (Rechtecken), welche in Zeilen und Spalten angeordnet werden. Wo welche Zelle steht, ergibt sich aus der Reihenfolge.

```html
<table>
	<tr>
		<td>Zelle links oben</td>
		<td>Zelle rechts oben</td>
	</tr>
	<tr>
		<td>Zelle links unten</td>
		<td>Zelle rechts unten</td>
	</tr>
</table>
```

`<table>` markiert das größte Rechteck für die Tabelle. Mit `<tr>` wird table row abgekürzt, was Tabellenzeile bedeutet. Somit wird als nächstes ein Rechteck für die Zeile gezogen. Darin sind `<td>` Elemente, welche table data bedeutet, was eine Tabellenzelle markiert. Hier kannst du den eigentlichen Zelleninhalt reinschreiben.

t> Erstelle im [Editor](https://apps.wi-wissen.de/html-css-js-editor/) eine Tabelle mit den Spaltenköpfen Links und Rechts und darunter jeweils dem Ausruf "Jawoll!"

t> Erstelle im [Editor](https://apps.wi-wissen.de/html-css-js-editor/) eine Tabelle mit 4 Spalten und 3 Zeilen

t> Expertenaufgabe: Informiere dich, was der Tabellenkopf und -body ist.