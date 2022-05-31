# Präfixe verwenden

## Keine Präfixe

Formalparameter von Bausteinen werden ohne Präfixe verwendet. Auch bei der Übergabe eines PLC-Datentyps wird kein Präfix verwendet.

Präfix | Typ
-------- |  ---------------
Kein Präfix | **Eingangs- und Ausgangsparameter** <br> Zugriff von außen möglich <br> &rarr; **enable** <br> &rarr; **error**
Kein Präfix | **Durchgangsparameter** <br> Änderung der verschalteten Daten sowohl durch Benutzer als auch durch Baustein möglich <br> &rarr; conveyorSetpoints
Kein Präfix | **Global-Datenbausteine** <br> Weder der Globaldatenbaustein noch die enthaltenen Elemente erhalten einen Präfix <br> &rarr; recipes

## Temoräre und statische Variablen mit Präfix "temp" bzw. "stat"

Um statische und temporäre Variablen klar von Formalparametern im Code zu trennen, werden die Präfixe ***temp_*** bzw. ***stat_*** verwendet.

Präfix | Typ
-------- |  ---------------
**stat_** | **Statische Variable** <br> Kein Zugriff auf die Lokaldaten von außerhalb erlaubt <br> &rarr; **stat_enableDrive**
**temp_**| **Temporäre Variable** <br> Kein Zugruff auf die Lokaldaten von außerhalb möglich <br> &rarr; temp_CenteringHomed

***Begründung:*** Dies erleichter dem Programmierer eines Bausteins die Unterscheidung zwischen Formalparameter und Lokaldaten. Dadurch können sofort die ZUgriffsrechte auf die Variable für den Benutzer definiert und erkannt werden.


