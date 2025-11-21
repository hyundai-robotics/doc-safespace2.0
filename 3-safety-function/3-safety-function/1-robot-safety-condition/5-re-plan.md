# 3.3.1.5 Re-Plan

Re-Plan ist eine Funktion, die die Geschwindigkeit des Roboters auf der Grundlage von Signalen steuert, die von externen Sicherheitssensoren empfangen werden. Die Betriebsgeschwindigkeit des Roboters ändert sich entsprechend dem Eingabesignal auf das Verzögerungsverhältnis, und die TCP-Geschwindigkeit wird nach der Verzögerungszeit bei der entsprechenden Geschwindigkeit überwacht. Wenn die Verzögerungszeit nicht ausreicht oder der Roboter nicht ausreichend verzögert und den TCP-Geschwindigkeitsgrenzwert überschreitet, wird sofort ein Sicherheitsstopp (Stopp 0, Stopp 1, Stopp 2) ausgelöst.

Über das Menü \[System > 4: Anwendungsparameter > 18: SafeSpace2.0 > 1: Sicherheitsfunktion > Parametereinstellungen > Roboterbeschränkung > Re-Plan]* können Sie die Parameterwerte festlegen.

![!Einstellungsbildschirm „Re-Plan“](../../../_assets/replan.png)

|  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |** |                       **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**                       |  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**  |
| :-------: | :------------------------------------------------: | :----------: |
| Replan |   <p>Ob die Geschwindigkeitskontrollfunktion je nach Eingangssignal verwendet werden soll</p><p>(On/Off)</p>  |  Off |
| Geschwindigkeitsbegrenzungswert | <p>TCP-Geschwindigkeitsbegrenzungswert nach Re-Plan</p><p>(0 bis 50000 (mm/s))</p> | 50000 |
| Verzögerungsverhältnis |   <p>Verzögerungsverhältnis, das bei Replan verwendet werden soll</p><p>(0 ~ 100 (%))</p>  | 0 |
| Verzögerungszeit |   <p>Wenn Sie die Geschwindigkeit mit RePlan ändern, wird die Überwachung mit dem geänderten Geschwindigkeitsgrenzwert nach der Verzögerungszeit durchgeführt  </p><p>(0 ~ 1000(ms))</p>  | 0 |
| Zuweisung von Eingangssignalen |   <p>Eingangssignal für Replan</p><p>(0 ~ 16)</p>  |  0 |

{% hint style="warning" %}
* Berücksichtigen Sie bei der Konfiguration von Geschwindigkeitsbegrenzungen unbedingt die Stoppzeit und den Schutz, um Kollisionen und Verletzungen zu vermeiden.
* Da die Aufprallkraft des Roboters proportional zur kinetischen Energie zunehmen kann, wenn die Geschwindigkeit hoch und die Nutzlast groß ist, kann es zu erheblichen Auswirkungen kommen, wenn der Roboter mit einem externen Objekt kollidiert. Halten Sie im kollaborativen Raum eine sichere Geschwindigkeit und Nutzlast ein.
{% endhint %}
