# 3.3.2.3 Gelenkstoppüberwachung

Die Stoppüberwachung überwacht jede Achse auf abnormale Bewegungen während des Roboterstopps. Wird ein festgelegter Grenzwert überschritten, wird sofort ein Sicherheitsstopp (Stopp 0) ausgelöst.

Parameterwerte können im Menü **\[System > 8: Sicherheitssystem > 1: Parametereinstellungen > 1: Robotergrenzwerte > 3: Gelenkstopp]** eingestellt werden.

<p align="center">
<img src="../../../_assets/joint_sos_param.png"></img>
<em><p align="center">Bildschirm für die Parametereinstellungen der Überwachung beenden</p></em>
</p>

|  **Parameter** |                       **Beschreibung**                       |  **Standardeinstellung**  |
| :-------: | :------------------------------------------------: | :----------: |
| Aktivierung | <p>Funktion aktiviert</p><p>(Ungültig / Gültig / Sichere E/A)</p> | Ungültig |
| Gelenkaktivierung | <p>Jedes Gelenk aktiviert</p><p>(Aktiv / Deaktiviert)</p> | Deaktiviert |
| <p>Zulässiger Bereich</p><p>[Grad]</p> | <p>Winkelgrenzwert für jedes Gelenk</p><p>(0,0 ~ 3,0)</p> | 0,001 |

{% hint style="warning" %}
**\[Vorsicht]**: Wenn die Überwachungsparameter nicht eingehalten werden, muss vor dem Neustart unbedingt überprüft werden, ob sich der Roboter normal bewegt.
{% endhint %}