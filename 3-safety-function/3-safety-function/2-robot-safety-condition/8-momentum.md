# 3.3.2.8 Impulseinstellung

Diese Funktion überwacht, ob der vom Roboter erzeugte Impuls den zulässigen Grenzwert überschreitet. Bei einer Überschreitung des Grenzwerts wird sofort ein Sicherheitsstopp (Stop 0, Stopp 1 oder Stopp 2) ausgelöst.

Die Parameterwerte können Sie im Menü **\[System > 8: Sicherheitssystem > 2: Parametereinstellungen > 1: Robotergrenzen > 8: Impuls]** festlegen.

<p align="center">
<img src="../../../_assets/momentum_param.png"></img>
<em><p align="center">Bildschirm „Momentum-Einstellungen“.</p></em>
</p>

| **Parameter** | 　　　　　　　　　**Beschreibung**                                                  |  **Standardeinstellung** |
| :------: | :----------------------------------------------------------------: | :---------: |
| Aktivieren | <p>Funktionsstatus</p><p>(Ungültig / Gültig / Sichere E/A)</p> | Ungültig |
| Stoppmethode | <p>Stoppmethode bei Funktionsverletzung</p><p>(Stop 0 / Stopp 1 / Stopp 2 / Kein Stopp)</p> | Stopp 1 |
| Bewegungsoptimierung | <p>Optimierung der Bewegung, sodass der Impulsgrenzwert des Roboters nicht überschritten wird</p><p>(Aktiv / Deaktiviert)</p> | Deaktiviert |
| <p>Maximaler Impuls</p><p>[kg m/s]</p> | <p>Impulsgrenzwert des Roboters</p><p>(5 bis 5000)</p> | 1000 |

{% hint style="warning" %}
* Hohe Geschwindigkeiten und große Nutzlasten, proportional zur kinetischen Energie des Roboters, können die Aufprallkraft erhöhen. Daher kann eine Kollision mit einem externen Objekt erhebliche Auswirkungen haben. In kollaborativen Umgebungen ist auf sichere Geschwindigkeit und Nutzlast zu achten.
* Abweichende Einstellungen für Werkzeuginformationen und Zusatzgewichte können zu Fehlalarmen führen. Bitte überprüfen Sie die Angaben, bevor Sie diese Funktion nutzen.
{% endhint %}
