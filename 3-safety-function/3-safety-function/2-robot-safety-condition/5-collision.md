# 3.3.1.6 Kollisionserkennung

Eine Kollision wird erkannt, wenn die auf den Roboter ausgeübte äußere Kraft den zulässigen Wert überschreitet. Sie können die Empfindlichkeit jeder Achse einstellen. Je höher die Empfindlichkeit, desto geringer ist die äußere Kraft, die als Kollision erkannt wird. Bei einer Verletzung der Überwachung wird sofort ein Sicherheitsstopp (Stopp 0, Stopp 1, Stopp 2) ausgelöst.

Über das Menü \[System > 4: Anwendungsparameter > 18: SafeSpace2.0 > 1: Sicherheitsfunktion > Parametereinstellungen > Roboterbeschränkung > Kollisionserkennung]* können Sie die Parameterwerte festlegen.

![!Einstellungsbildschirm für Kollisionserkennung](../../../_assets/col-det.png)

| **| Parameter | 　　　　　　　　　Beschreibung                                                  |  Standardeinstellung |** | 　　　　　　　　　**| Parameter | 　　　　　　　　　Beschreibung                                                  |  Standardeinstellung |**                                                  |  **| Parameter | 　　　　　　　　　Beschreibung                                                  |  Standardeinstellung |** |
| :------: | ---------------------------------------------------------------- | :---------: |
| Activation | <p>Funktionsaktivierungsstatus</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stoppmethode bei Funktionsverletzung</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Joint OnOff |   <p>Aktivierungsstatus jedes Gelenks</p><p>(On/Off)</p>  |  Off |
| Empfindlichkeit |   <p>Erkennungsempfindlichkeit für jedes Gelenk</p><p>(0 ~ 200 (%))</p>  |  100 |

{% hint style="warning" %}
* Da die Aufprallkraft des Roboters proportional zur kinetischen Energie zunehmen kann, wenn die Geschwindigkeit hoch und die Nutzlast groß ist, kann es zu erheblichen Auswirkungen kommen, wenn der Roboter mit einem externen Objekt kollidiert. Halten Sie im kollaborativen Raum eine sichere Geschwindigkeit und Nutzlast ein.
* Es kann zu Fehlalarmen kommen, wenn die Werkzeuginformationen und das Zusatzgewicht anders als die tatsächlichen Werte eingestellt sind. Überprüfen Sie alle Informationen, bevor Sie die Kollisionserkennungsfunktion verwenden.
{% endhint %}
