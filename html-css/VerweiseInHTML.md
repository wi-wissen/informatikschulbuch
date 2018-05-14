# Verweise

In diesem Kapitel wollen wir uns ansehen, wie wir von formatierten Text zu einer tatsächlichen Webseite gelangen. Dazu gehören auf jeden Fall das Setzen von Links und das einbinden von Bildern.

Das wir beides in diesem Kapitel behandeln ist kein Zufall. In beiden Fällen müssen wir den Browser nämlich anweisen noch eine weitere Datei zu betrachten. Entweder zeigen wir ihm die nächste HTML-Datei oder eine Bilddatei, die er gleich einbinden soll.

i> Neben Bildern können wir auch Videos, Ton, PDF Dokumente und sogar ganze Karten einbinden, das sind aber schon kniffligere Themen.)

## Aufbau eines Verweises

Ein Verweis ist genau wie ein Link aufgebaut, den du in die Adressleiste deines Browsers eingibst.

```
https://apps.wi-wissen.de/lehrunterlagen.php
```

1. `https` – Protokoll für eine verschlüsslte Verbindung
2. `apps` – Subdomain ein spezieller Bereich innerhalb einer Domain. Früher auch oft www für den Bereich der Webseite für den Browser.
3. `wi-wissen` – Domainname, welcher ermglicht die Adresse des Rechners im Internet zu finden.
4. `de` - Domainendung - unterhalb dieser befinden sich Domainnamen, welche jeweilse eindeutig sein müssen
5. `lehrunterlagen.php` – Datei (könnte auch ein 
   Ordnerpfad sein) die der Browser dir zeigen soll. php bedeutet in diesem
    Fall, dass der Server die Seite noch berechnen muss, ehe er die 
   Webseite an den Browser ausliefern darf.

t> Notiere die folgende Domain in deinen Hefter und gib an, was die einzelnen Bestandteile bedeuten: 

```
https://lops-leipzig.de/schule/about_us.html
```

## Verweisarten

### absolute Verweise

Gibst du in deinen Browser einen Verweis musst du immer die vollständige Adresse eingeben, damit dein Rechner weiß, wie wo er die Webseite herbekommen kann. Dadurch ist es egal auf welcher Seite du vorher warst. Du kommst immer auf der neuen Adresse an. Das ist ähnlich einer Postanschrift. Hier ist es auch ganz egal in welchen Briefkasten ich den Brief einwerfe.					

```
https://apps.wi-wissen.de/html-css-js-editor/img/bird.jpg
```

### relative Verweise

Manchmal ist es unpraktisch immer die ganze Adresse anzugeben. Etwa wenn
 du vorhast den Domainnamen deiner Webseite zu ändern, dann müsstest du 
auch alle Links anpassen. Dies funktioniert nur, wenn du schon auf einer ganz speziellen Webseite im Internet bist. Das ist wie eine Wegbeschreibung "*200m geradeaus und dann scharf links, dann bist du gegen den Laternenpfahl gelaufen.*. Du rennst nur gegen den Laternenpfahl, wenn du dich an einer speziellen Position befindest.					

```
img/bird.jpg
```

Du siehst, dieser relative Verweis ist auch viel kürzer und erpart und ein wenig Schreibarbeit. Um zu der Datei zu gelangen soll der Browser zuerst in den Ordner `img` gehen und anschließend das Bild `bird.jpg` abrufen. 

i> Der Ordner `..` weißt den Browser einen Ordner über den aktuellen Ordner zu gehen. und mit `/` geht es ganz nach oben in das Wurzelverzeichnis oder hier bekannt als Domainname mit Domainendung.

t> Notiere in deinem Hefter, was ein relativer und was ein aboluster Verweis (Adresse) ist.

t>  Gib ein Beispiel, wann eine absolute Adresse im Internet verwendet werden muss.

t>  Gib ein Beispiel, wann eine relative Adresse verwendet werden kann. Begründe den Vorteil in dieser Situation.

## Links

```
<a href="https://wi-wissen.de/">WIssen</a>
```

t> Gib den obigen Befehl in den [Editor](https://apps.wi-wissen.de/html-css-js-editor/) ein und untersuche, was der Befehl bedeutet.

Hier haben wir etwas Neues. Bisher kannten wir nur `<a>WIssen</a>`. Nun steht im Startelement noch zusätzlich `href="https://wi-wissen.de/"`. Hierdurch wird das Textelement Link genauer für den Webbrowser beschrieben, was aber so nicht unmittelbar angezeigt wird.

Da es den Link genauer beschreibt, sagt man auch `href` ist eine Eigenschaft des Links. Bei HTML heißt Eigenschaft Attribut. `"https://wi-wissen.de/"` ist der Wert des Attributes (Attributwert), welcher in Anführungszeichen geschrieben wird.

t> Notiere in deinem Hefter was Attribute in HTML sind. Es könnte praktisch sein einen Link als Beispiel mit aufzuschreiben.

## Bilder

Das Einbinden eines Bildes funktioniert, ähnlich eines Links, nur dass hier nicht auf das Bild verwiesen wird, sondern es direkt in der HTML-Webseite angezeigt wird:

```html
<img src="img/dog.jpg" alt="Dog" />
```

t>  Gib den Befehl in den [Editor](https://apps.wi-wissen.de/html-css-js-editor/) ein.

t>  Finde mithilfe von [selfhtml.org](https://wiki.selfhtml.org/wiki/Img) her aus, was `src` und `alt` bedeuten.