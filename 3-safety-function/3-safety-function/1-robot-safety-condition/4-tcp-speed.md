# 3.3.1.4 TCP-Geschwindigkeitsbegrenzung

Eine Funktion, die die TCP-Geschwindigkeit basierend auf dem Roboterkoordinatensystem überwacht. Bei einer Verletzung der Überwachung wird sofort ein Sicherheitsstopp (Stopp 0, Stopp 1, Stopp 2) ausgelöst.

Über das Menü \[System > 4: Anwendungsparameter > 18: SafeSpace2.0 > Parametereinstellungen > Roboterbeschränkung > TCP-Geschwindigkeitsbegrenzung]* können Sie die Parameterwerte festlegen.

![!Bildschirm zur Einstellung der TCP-Geschwindigkeitsparameter](../../../_assets/tcp_speed_param.png)

| **| Parameter | 　　　　　　　　　Beschreibung                                                  |  Standardeinstellung |** | 　　　　　　　　　**| Parameter | 　　　　　　　　　Beschreibung                                                  |  Standardeinstellung |**                                                  |  **| Parameter | 　　　　　　　　　Beschreibung                                                  |  Standardeinstellung |** |
| :------: | ---------------------------------------------------------------- | :---------: |
| Activation | <p>Funktionsaktivierungsstatus</p><p>(Off/On/Safety Input)</p> |   Off  |
| Sicherheitsstopp |   <p>Stoppmethode bei Funktionsverletzung</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Replan |   <p>Ob die Geschwindigkeitskontrollfunktion je nach Eingangssignal verwendet werden soll</p><p>(On/Off)</p>  |  Off |
| Geschwindigkeitsgrenzwert |   <p>TCP-Geschwindigkeitsgrenzwert</p><p>(0 ~ 50000 (mm/s))</p>  | 50000 |
| Verzögerungsverhältnis   <p>Verzögerungsverhältnis, das bei Replan verwendet werden soll</p><p>(0 ~ 100 (%))</p>  | 0 |
| Verzögerungszeit |   <p>Wenn Sie die Geschwindigkeit mit RePlan ändern, wird die Überwachung mit dem geänderten Geschwindigkeitsgrenzwert nach der Verzögerungszeit durchgeführt  </p><p>(0 ~ 1000(ms))</p>  | 0 |
| Zuweisung von Eingangssignalen   <p>Eingangssignal für Replan</p><p>(0 ~ 16)</p>  |  0 |

{% hint style="warning" %}
*\[Achtung]**: Berücksichtigen Sie bei der Einstellung der Geschwindigkeitsüberwachungsfunktion unbedingt die Stopp-Reaktionszeit und die Abdeckung, um Kollisionen und Verletzungen zu vermeiden.
{% endhint %}
 