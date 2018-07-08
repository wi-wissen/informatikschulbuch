# CSS und die Boxen

05.06.2017

## Entwicklerwerkzeuge im Browser

Bisher haben wir einzelne Elemente von Webseiten gestaltet. Hier untersuchen wir die Beziehung der Elemente untereinander:

*Mozilla Firefox 53*: Drücke <kbd>Strg</kbd> + <kbd>Umschalt</kbd> + <kbd>C</kbd>

*Google Chrome 58*: Drücke <kbd>Strg</kbd> + <kbd>Umschalt</kbd> + <kbd>C</kbd>

Es öffnet sich am unteren Rand des Browsers die Entwicklerwerkzeuge.

In den Entwicklerwerkzeugen kannst du einen Blick hinter die Kulissen werfen und die Webseite für dich verändern.

t> Fahre über verschiedene Bereiche der Webseite.

Du wirst feststellen, dass diese in farbige Kästen getaucht werden. Diese dienen dazu, dir bei der Orientierung zu helfen.

t> Fahre nun mit der Maus über diesen Textabschnitt. 					

Auch dieser Textabschnitt erscheint in einer Box. Das liegt daran, dass der Browser alle Elemente einer Webseite in einzelne Boxen einsortiert. Diese Boxen können verschieden angeordnet werden.

## Abstände von Boxen

t> Verwende wieder die Elementuntersuchenfunktion mit Drücke <kbd>Strg</kbd> + <kbd>Umschalt</kbd> + <kbd>C</kbd>

t> Fahre mit der Maus über die `div` mit Innenabstand.

<div class="panel panel-default"><div class="panel-body"><div style="padding: 10px; background: none repeat scroll 0 0 #F1F3F4; border: 1px solid #d5d5d5;"><code>div</code> mit Innenabstand</div><div style="margin: 10px; background: none repeat scroll 0 0 #F1F3F4; border: 1px solid #d5d5d5;"><code>div</code> mit Außenabstand</div><div style="padding: 10px; margin: 10px; background: none repeat scroll 0 0 #F1F3F4; border: 1px solid #d5d5d5;"><code>div</code> mit Innen- und Außenabstand</div></div></div>

*Mozilla Firefox 53*:  Im Unteren Bereich unten Rechts findest du nach dem Aktivieren des Tabs „Berechnet“ ein Modell der Box:

![img](/img/09-1.png)

*Google Chrome 58*:

Im unteren rechten Bereich findest du ein Modell der Box:

![img](/img/09-2.png)

t> Ermittle die Bedeutung der CSS-Attribute margin, padding und border.

i> Tipp: Ein Englischwörterbuch oder die ausführliche Dokumentation helfen dir notfalls weiter.

Experten: Verändere die CSS-Attribute der gegebenen Boxen mit dem Entwicklerwerkzeug.

## Zusammenfallende Außenabstände

t> Lies dir den Abschnitt [collapsing margins von wiki.selfhtml.org](https://wiki.selfhtml.org/wiki/CSS/Box-Modell#Zusammenfallende_Au.C3.9Fenabst.C3.A4nde_.28collapsing_margins.29) durch.

t> Notiere dir kurz, was collapsing margins sind.

i> Ausführliche Dokumentation: <https://wiki.selfhtml.org/wiki/CSS/Box-Modell>