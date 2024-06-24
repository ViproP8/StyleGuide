# Nomenklatur und Formatierung

Der Name in Bezeichnern (Bausteine, Variablen etc.) ist in Englischer Sprache
(English – United States) zu verfassen. Der Name gibt den Sinn und Zweck des
Bezeichners im Kontext des Quellcodes wieder und lässt damit einen Rückschluss
auf dessen Funktionalität bzw. Verwendung zu.

* Die gewählte Schreibweise der Bezeichner muss in allen Bausteinen und PLCDatentypen beibehalten werden und ist so kurz wie möglich zu gestalten
* Gleiche funktionale Bedeutung erhält namensgleiche Bezeichner. Dies gilt auch bezüglich Groß- und Kleinschreibung.
* Für Bezeichner, die aus mehreren Worten bestehen, ist die Reihenfolge der Worte wie die des gesprochenen Worts zu wählen
* Funktionen/ Funktionsbausteine beginnen nach Möglichkeit mit einem Verb, z. B. "Get", "Set", "Put", "Find", "Search", "Calc".
* Ist der Bezeichner ein Arraybezeichner, ist er im Plural zu verwenden. Unzählbare Nomen bleiben im Singular ("data", "information", "content").
* Statische und temporäre Boolesche Variablen sind häufig zustandsanzeigende Variablen. In einem solchen Falle sind Namen mit "is", "can" oder "has" am eingängigsten und verständlichsten.

## Sinnvolle Komentare und Eigenschaften verwenden

Kommentarfelder und Eigenschaftsfelder sind zu verwenden und mit sinnvollen Kommentaren und Information zu füllen. Dazu zählen z. B.

* Bausteintitel und Bausteinkommentar ("Entwicklerinformationen dokumentieren")
* Bausteinschnittstellen
* Netzwerktitel und Netzwerkkommentare
* Bausteine, deren Variablen und Konstanten
* PLC-Datentypen und deren Variablen
* PLC-Variablentabellen, PLC-Variablen und Anwenderkonstanten
* PLC-Meldetextlisten
* Bibliothekseigenschaften

Ein Kommentar liefert dem Leser Information darüber, warum etwas an der
betreffenden Stelle getan wird. Er darf nicht den Code als redundanten Klartext
wiedergeben – also nicht was getan wird – das beschreibt bereits der Code –
sondern warum es getan wird.

## Entwicklerinformationen dokumentieren 

Jeder Baustein erhält einen Beschreibungskopf im Programmcode (SCL) bzw. im Blockkommentar (KOP, FUP). Darin müssen die wichtigsten Informationen zur
Bausteinentwicklung hinterlegt werden. 
<br>
Die nachfolgende Schablone für einen Beschreibungskopf enthält sowohl die Elemente aus den Baustein-Eigenschaften als auch entwicklerspezifische
Elemente, die nicht in die Eigenschaften übernommen werden müssen.
Die Beschreibung enthält folgende Punkte:

* Titel/ Bausteinbezeichner
* Beschreibung der Funktionalität
* (Optional) Name der Bibliothek
* Autor
* Einschränkungen bei der Benutzung (z. B. bestimmte OB-Typen)
* Voraussetzungen (z. B. zusätzliche Hardware)
* (Optional) zusätzliche Informationen
* Änderungslog mit Version, Datum, Autor und Änderungsbeschreibung (bei Safety-Bausteinen Safety-Signatur)

```
(*******************************************************************************************************
***************************************** Funktionsname ************************************************
********************************************** ****** **************************************************
********************************************************************************************************
Author:             John Doe 

Description:        Möglichst ausführliche und detallierte Beschreibung der Funktion.
                    Ablauf und Funktionsweise. Beschreibung der Ein- und Ausgänge, als auch der Logik.
                 
Requirments:        Anforderungen, die an diesen Baustein gestellt werden. Grenzwerte oder Anforderungen 
                    speziele PLC-Datentypen
                    
Restrictions:       Eventuelle Einschränkungen (Optional)                    
********************************************************************************************************
Changelog:
Version         | Date:         | Author:           | Change:   
********************************************************************************************************
1.0.0           | 14.06.2015    | John Doe          | First release   

*******************************************************************************************************)
```
