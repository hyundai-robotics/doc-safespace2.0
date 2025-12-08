# 3.3.1.1 Allgemein

Legen Sie die Schwellenwerte für die für den Roboterbetrieb erforderlichen Kernfunktionen fest (Geschwindigkeitsüberwachung im manuellen Modus, Stoppzeit- und Stoppwegüberwachung). Konfigurieren Sie außerdem, ob die Roboter- und Bereichsüberwachung vollständig aktiviert sind. Selbst wenn die Roboter- und Bereichsüberwachung aktiviert sind, funktioniert die Überwachung nicht, wenn die Sicherheitsfunktion deaktiviert ist. Tritt ein Überwachungsverstoß auf, wird der konfigurierte Sicherheitsstopp (Stop 0, Stopp 1) sofort ausgelöst.


Sie können Parameterwerte im Menü **\[System > 8: Sicherheitssystem > 1: Grundeinstellungen > 1: Allgemein]** festlegen.

<p align="center">
<img src="../../../_assets/3/general.png"></img>
<em><p align="center">설정 화면</p></em>
</p>


|  **Parameter** |                       **Beschreibung**                       |  **Standardeinstellung**  |
| :-------: | :------------------------------------------------: | :-------------: |
| Sicherheitsfunktion | <p>Aktiviert die Roboter- und Bereichsüberwachungsfunktionen?</p><p>(Aktivieren / Deaktivieren)</p> | Deaktivieren |
| <p>Geschwindigkeit im manuellen Modus</p><p>[mm/s]</p> | <p>Funktion aktiviert?</p><p>(10 ~ 250)</p> | 250 |
| <p>Stoppzeit</p><p>[ms]</p> | <p>Stoppmethode bei Funktionsverletzung</p><p>(100 ~ 2000)</p> | 2000 |
| - Bewegungsoptimierung | <p>Anpassung an eine Bewegung, die die Stoppzeitbegrenzung einhält</p><p>(Aktivieren / Deaktivieren)</p> | Deaktivieren |
| <p>Stoppdistanz</p><p>[mm]</p> | <p>Aktivierung jedes Gelenks</p><p>(50 ~ 2000)</p> | 2000 |
| - Bewegungsoptimierung | <p>Anpassung an eine Bewegung, die die Stoppdistanzbegrenzung einhält</p><p>(Aktivieren / Deaktivieren)</p> | Deaktivieren |

{% hint style="warning" %}
**[Achtung]**: Auch wenn die Sicherheitsfunktion deaktiviert ist, bleiben die für den Roboterbetrieb notwendigen Funktionen (manuelle Geschwindigkeit, Stoppzeit, Überwachung des Stoppabstands) aktiv.
{% endhint %}

{% hint style="warning" %}
**[Achtung]**: Die Stoppzeit und der Stoppabstand geben die Zeit und den Abstand an, bis der Roboter tatsächlich zum Stillstand kommt, wenn stop1 ausgeführt wird. Wird der eingestellte Wert überschritten, wird sofort stop0 aktiviert. 
{% endhint %}
 