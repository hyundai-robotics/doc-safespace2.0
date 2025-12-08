# 3.3.2.6 Re Plan-Funktion

Replan ist eine Funktion, die die Robotergeschwindigkeit anhand von Signalen externer Sicherheitssensoren anpasst. Die Betriebsgeschwindigkeit des Roboters wird entsprechend der Verzögerungsrate des Eingangssignals angepasst, und die TCP-Geschwindigkeit wird nach einer Verzögerungszeit bei der entsprechenden Geschwindigkeit überwacht.

Reicht die Verzögerungszeit nicht aus oder verzögert der Roboter nicht ausreichend, sodass die TCP-Geschwindigkeitsgrenze überschritten wird, wird sofort ein Sicherheitsstopp (Stop 0, Stopp 1, Stopp 2) ausgelöst.

Die Parameterwerte können Sie im Menü **\[System > 8: Sicherheitssystem > 2: Parametereinstellung > 1: Robotergrenzen > 6: Neuplanung]** einstellen.

<p align="center">
<img src="../../../_assets/3/re_plan.png"></img>
<em><p align="center">Bildschirm „Einstellungen Re plan“.</p></em>
</p>

|  **Parameter** |                       **Beschreibung**                       |  **Standardeinstellung**  |
| :-------: | :------------------------------------------------: | :----------: |
| Replan | <p>Geschwindigkeitsregelung abhängig vom Eingangssignal verwenden</p><p>(Aktivieren / Deaktivieren)</p> | Deaktivieren |
| <p>Verzögerungszeit</p><p>[ms]</p> | <p>Geschwindigkeitsbegrenzungswert nach Geschwindigkeitsänderung mit Replan überwachen</p><p>(0 ~ 1000)</p> | 2000 |
| <p>Geschwindigkeitsbegrenzungswert</p><p>[mm/s]</p> | <p>TCP-Geschwindigkeitsbegrenzungswert nach Replan</p><p>(0 ~ 50000)</p> | 50000 |
| <p>Geschwindigkeitsverhältnis</p><p>[%]</p> | <p>Verzögerungsverhältnis bei Replan</p><p>(0 ~ 100)</p> | 100 |
| <p>Eingangssignal</p><p>[Typ, Nummer]</p> | <p>Eingangssignal für Re plan</p><p>( [Keine, -] / [Sicherheitseingang, 1~8] / [PROFIsafe, 1~64] )</p> | 0 |

{% hint style="warning" %}
* Bei der Konfiguration von Geschwindigkeitsbegrenzungen ist stets die Bremszeit zu berücksichtigen und der Roboter abzudecken, um Kollisionen und Verletzungen zu vermeiden.
* Hohe Geschwindigkeiten und große Nutzlasten können, proportional zur kinetischen Energie des Roboters, dessen Aufprallkraft erhöhen. Daher kann es bei einer Kollision mit einem externen Objekt zu einem erheblichen Aufprall kommen. In kollaborativen Umgebungen ist daher eine sichere Geschwindigkeit und Nutzlast einzuhalten.
{% endhint %}
