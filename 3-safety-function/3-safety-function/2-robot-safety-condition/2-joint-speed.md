# 3.3.2.2 Gelenkgeschwindigkeitsgrenze

Der Parameter „Gelenkgeschwindigkeitseinstellung“ ist ein Grenzwert zur Überwachung der Gelenkgeschwindigkeit des Roboters. Wird der Grenzwert überschritten, wird der festgelegte Sicherheitsstopp (Stop 0, Stopp 1 oder Stopp 2) sofort aktiviert.

<p align="center">
<img src="../../../_assets/joint_speed.PNG"></img>
<em><p align="center">Beispiel für die Einstellung der Gelenkgeschwindigkeit</p></em>
</p>

Sie können Parameterwerte im Menü **\[System > 8: Sicherheitssystem > 2: Parametereinstellungen > 1: Robotergrenzen > 2: Gelenkgeschwindigkeit]** festlegen.

<p align="center">
<img src="../../../_assets/joint_speed_param.png"></img>
<em><p align="center">Einstellungsbildschirm für Gelenkgeschwindigkeit</p></em>
</p>

|  **Parameter** |                       **Beschreibung**                       |  **Standardeinstellung**  |
| :-------: | :------------------------------------------------: | :----------: |
| Aktivieren | <p>Funktionsstatus</p><p>(Ungültig / Gültig / Sichere E/A)</p> | Ungültig |
| Stoppmethode | <p>Stoppmethode bei Funktionsverletzung</p><p>(Stopp 0 / Stopp 1 / Stopp 2 / Kein Stopp)</p> | Stopp 1 |
| Bewegungsoptimierung | <p>Optimierung der Bewegung, sodass die Gelenkgeschwindigkeit nicht überschritten wird</p><p>(Aktiv / Deaktiviert)</p> | Deaktiviert |
| Gelenkaktivierung | <p>Aktiviert jedes Gelenk</p><p>(Aktiv / Deaktiviert)</p> | Deaktiviert |
Typ | <p>Betriebsart für jedes Gelenk</p><p>(Rotation / Linear)</p> | Rotation |
<p>Geschwindigkeit</p><p>[mm/s]</p> | <p>Geschwindigkeitsbegrenzung für jedes Gelenk</p><p>(0 ~ 10000)</p> | 1000,0 |

{% hint style="warning" %}
**\[Vorsicht]**: Achten Sie bei der Aktivierung der Geschwindigkeitsüberwachungsfunktion unbedingt auf die Bremsreaktionszeit und schließen Sie die Abdeckung, um Kollisionen und Verletzungen zu vermeiden.
{% endhint %}
 
