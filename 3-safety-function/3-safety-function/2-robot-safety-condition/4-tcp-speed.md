# 3.3.2.4 TCP-Geschwindigkeitsbegrenzung

Diese Funktion überwacht die TCP-Geschwindigkeit relativ zum Roboterkoordinatensystem. Bei Überschreitung der Überwachungsgrenze wird sofort ein Sicherheitsstopp (Stop 0, Stopp 1 oder Stopp 2) ausgelöst.

Die Parameterwerte können Sie im Menü **\[System > 8: Sicherheitssystem > 2: Parametereinstellungen > 1: Robotergrenzen > 4: TCP-Geschwindigkeit]** festlegen.

<p align="center">
<img src="../../../_assets/tcp_speed_param.png"></img>
<em><p align="center">Bildschirm zur Einstellung der TCP-Geschwindigkeitsparameter</p></em>
</p>


| **Parameter** |                                  **Beschreibung**                                  |  **Standardeinstellung** |
| :------: | :----------------------------------------------------------------: | :---------: |
| Aktivieren | <p>Funktionsaktivierung</p><p>(Ungültig / Gültig / Sichere E/A)</p> | Ungültig |
| Stoppmethode | <p>Stoppmethode bei Funktionsverletzung</p><p>(Stop 0 / Stopp 1 / Stopp 2 / Kein Stopp)</p> | Stopp 1 |
| Bewegungsoptimierung | <p>Anpassung an eine Bewegung, die die TCP-Geschwindigkeitsgrenze nicht überschreitet</p><p>(Aktivieren / Deaktivieren)</p> | Deaktivieren |
| Geschwindigkeitsanpassung | <p>Geschwindigkeitsanpassungsfunktion abhängig vom Eingangssignal verwenden</p><p>(Aktivieren / Deaktivieren)</p> | Deaktivieren |
| <p>Geschwindigkeitsbegrenzungswert</p><p>[mm/s]</p> | <p>TCP-Geschwindigkeitsbegrenzungswert</p><p>(0 ~ 50000)</p> | 50000 |
| <p>Verzögerungsverhältnis</p><p>[%]</p> | <p>Verzögerungsverhältnis für die Geschwindigkeitsanpassung</p><p>(0 ~ 100)</p> | 100 |
| <p>Verzögerungszeit</p><p>[ms]</p> | <p>Bei Geschwindigkeitsänderung durch Anpassung wird nach der Verzögerungszeit der geänderte Geschwindigkeitsbegrenzungswert überwacht</p><p>(0 ~ 1000)</p> | 1000 |
| <p>Eingangssignal</p><p>[Typ, Nummer]</p> | <p>Eingangssignal für die Drehzahlanpassung</p><p>( [Keine, -] / [Sicherheitseingang, 1~8] / [PROFIsafe, 1~64] )</p> | 0 |

{% hint style="warning" %}
**\[Vorsicht]**: Achten Sie bei der Aktivierung der Geschwindigkeitsüberwachungsfunktion unbedingt auf die Bremsreaktionszeit und schließen Sie die Abdeckung, um Kollisionen und Verletzungen zu vermeiden.
{% endhint %}
 