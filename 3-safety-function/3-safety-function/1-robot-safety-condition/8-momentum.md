# 3.3.1.8 Momentenüberwachung

Eine Funktion, die überwacht, ob das vom Roboter erzeugte Moment den zulässigen Wert überschreitet. Bei einer Verletzung der Überwachung wird sofort ein Sicherheitsstopp (Stopp 0, Stopp 1, Stopp 2) ausgelöst.

Über das Menü \[System > 4: Anwendungsparameter > 18: SafeSpace2.0 > 1: Sicherheitsfunktion > Parametereinstellungen > Roboterbeschränkung > Momentenüberwachung ]* können Sie die Parameterwerte festlegen.

![!Einstellungsbildschirm für Leistungsüberwachung](../../../_assets/momentum.png)

| **| Parameter | 　　　　　　　　　Beschreibung                                                  |  Standardeinstellung |** | 　　　　　　　　　**| Parameter | 　　　　　　　　　Beschreibung                                                  |  Standardeinstellung |**                                                  |  **| Parameter | 　　　　　　　　　Beschreibung                                                  |  Standardeinstellung |** |
| :------: | ---------------------------------------------------------------- | :---------: |
| Activation | <p>Funktionsaktivierungsstatus</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stoppmethode bei Funktionsverletzung</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Leistung |:   <p>Grenzwert für das Momentum des Roboters</p><p>(5 ~ 1000 (W))</p>  | 1000 |

{% hint style="warning" %}
* Da die Aufprallkraft des Roboters proportional zur kinetischen Energie zunehmen kann, wenn die Geschwindigkeit hoch und die Nutzlast groß ist, kann es zu erheblichen Auswirkungen kommen, wenn der Roboter mit einem externen Objekt kollidiert. Halten Sie im kollaborativen Raum eine sichere Geschwindigkeit und Nutzlast ein.
* Es kann zu Fehlalarmen kommen, wenn die Werkzeuginformationen und das Zusatzgewicht anders als die tatsächlichen Werte eingestellt sind. Bitte überprüfen Sie die Informationen, bevor Sie die Funktion verwenden.
{% endhint %}
