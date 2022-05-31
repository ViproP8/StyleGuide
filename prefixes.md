# Präfixe verwenden

## Keine Präfixe

Formalparameter von Bausteinen werden ohne Präfixe verwendet. Auch bei der Übergabe eines PLC-Datentyps wird kein Präfix verwendet.
Globaldatenbausteine, die keinem Funktionsbaustein oder Funktion zueghörig sind, bekommen ebenfalls keinen Präfix.

Präfix | Typ
-------- |  ---------------
Kein Präfix | **Eingangs- und Ausgangsparameter** <br> Zugriff von außen möglich <br> &rarr; **enable** <br> &rarr; **error**
Kein Präfix | **Durchgangsparameter** <br> Änderung der verschalteten Daten sowohl durch Benutzer als auch durch Baustein möglich <br> &rarr; conveyorSetpoints
Kein Präfix | **Global-Datenbausteine** <br> Weder der Globaldatenbaustein noch die enthaltenen Elemente erhalten einen Präfix <br> &rarr; recipes



## Funktionseigene Datenbausteine 

Datenbausteine, die einer Funktion oder einem Funktionsbaustein zugehörig sind, werden entsprechend der Funktion benannt. Ihnen wird der Präfix ***db** vorangestellt.

Funktion |  Zugehöriger Datenbaustein 
-------- |  --------------- 
RecipeHandler |  dbRecipeHandler
safety |   dbSafety



## Temoräre und statische Variablen mit Präfix "temp" bzw. "stat"

Um statische und temporäre Variablen klar von Formalparametern im Code zu trennen, werden die Präfixe ***temp_*** bzw. ***stat_*** verwendet.

Präfix | Typ
-------- |  ---------------
**stat_** | **Statische Variable** <br> Kein Zugriff auf die Lokaldaten von außerhalb erlaubt <br> &rarr; **stat_enableDrive**
**temp_**| **Temporäre Variable** <br> Kein Zugruff auf die Lokaldaten von außerhalb möglich <br> &rarr; **temp_CenteringHomed**

***Begründung:*** Dies erleichter dem Programmierer eines Bausteins die Unterscheidung zwischen Formalparameter und Lokaldaten. Dadurch können sofort die ZUgriffsrechte auf die Variable für den Benutzer definiert und erkannt werden.

## Instanzdaten mit Präfix ***inst*** bzw. ***Inst**

Sowohl Einzelinstanzen, als auch Multiinstanzen und Paramaterinstanzen erhalten einen Präfix. Bei Einzelinstanzen wird ein ***Inst***, bei Multi- und Parameterinstanzen ein ***inst*** vorangestellt.
Präfix | Typ
-------- |  ---------------
**inst_** | **Variablen bei Mulitinstanzen und Parameterinstanzen** <br> &rarr; inst_TON_ResetWarning <br> &rarr; **inst_ConveyorFunction(s)** (Bei Arrays von Instanzen)
**Inst_** | **Einzelinstanzdatenbausteine** <br> &rarr; Inst_ConveyorFunction 

## PLC-Datentypen mit Präfix type

Einem PLC-Datentyp wird das Präfix **type** vorangestellt. Die Elemente im PLC-Datentyp erhalten wiederum keinen Präfix.

Präfix | Typ
-------- |  ---------------
**type** | **PLC-Datentyp** <br> Nur der PLC-Datentyp erhält das Präfix, nicht die enthaltenen Elemente <br> &rarr; typeConveyorSetpoints <br> &rarr; **typeMovikitPositioning**


## Bezeichner von Konstanten GROSS schreiben

Die Namen von Konstanten (globale und lokale Konstanten) werden durchgehend in Großschrift geschrieben (UPPER_CASING). Zum Trennen und Erkennen einzelner Worte oder Abkürzungen ist jeweils ein Unterstrich zwischen den einzelnen Wörtern einzusetzen

&rarr; **MAX_VELOCITY** <br>
&rarr; **SEGMENT_NUMBER**







