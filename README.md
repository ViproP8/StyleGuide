# StyleGuide

## Ziele

Die hier beschriebenen Regeln und Empfehlungen sollen helfen einen einheitlichen Programmcode zu erstellen, der besser gewartet und wiederverwendet werden kann. 
Für die Wartbarkeit und Übersichtlichkeit des Quellcodes ist es zunächst erforder- lich, sich an eine gewisse äußere Form zu halten. Optische Effekte tragen nur unwesentlich zur Qualität der Software bei. Viel wichtiger ist es beispielsweise auch Regeln zu finden, die die Entwickler folgendermaßen unterstützen:

* Vermeiden von Tipp- und Flüchtigkeitsfehlern, die der Compiler anschließend falsch interpretiert. <br> **Ziel:** Der Compiler soll so viele Fehler wie möglich erkennen.
* Unterstützung des Programmierers bei der Diagnose von Programmfehlern, z. B. versehentliche Wiederverwendung einer temporären Variablen über einen Zyklus hinaus. <br> **Ziel:** Der Bezeichner weist frühzeitig auf Probleme hin.
* Vereinheitlichung von Standardapplikationen und Standardbibliotheken <br> **Ziel:** Die Einarbeitung soll einfach sein und die Wiederverwendbarkeit von Programmcode erhöht werden.
* Einfache Wartung und Vereinfachung der Weiterentwicklung <br> **Ziel:** Änderungen von Programmcode in den einzelnen Modulen, die Organi- sationsbausteine, Funktionen, Funktionsbausteine und Datenbausteine in Bibliotheken oder im Projekt umfassen können, sollen minimale Auswirkungen auf das Gesamtprogramm/ die Gesamtbibliothek haben. Änderungen von Programmcode in den einzelnen Modulen sollen von verschiedenen Programmierern durchführbar sein.

### Vorteile eines Einheitlichen Programmierstils
* Einheitlicher durchgängiger Stil
* Leicht lesbar und verständlich
* Einfache Wartung und Wiederverwendbarkeit
* Einfache und schnelle Fehlererkennung und -korrektur
* Effiziente Zusammenarbeit zwischen mehreren Programmierern

[Begrifssklärung](/clarificationOfTerms.md)
[Einsatz von Präfixen](/prefixes.md)



## Regelverletzungen und andere Vorgaben

Bei Kundenprojekten sind die geforderten Normen sowie die kunden- oder branchenspezifischen Standards des Kunden oder der verwendeten Technologie  einzuhalten und besitzen Priorität gegenüber diesem Styleguide oder Teilen davon.<br>
Bei einer Kombination von Kundenvorgaben und diesem Styleguide ist auf die Integrität der Kombination beider Vorgaben und des Gesamtprojekts zu achten.
Eine Regelverletzung ist an der entsprechenden Stelle im Anwenderprogramm zu begründen und zu dokumentieren.<br>
Die vom Kunden definierten Regeln sind in geeigneter Form zu dokumentieren
