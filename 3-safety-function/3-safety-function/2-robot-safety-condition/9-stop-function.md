# 3.3.2.9 Stoppeinstellungen

Wählen Sie für jede Sicherheitsfunktion den passenden Sicherheitsstopptyp. Sicherheitsstoppfunktionen bringen den Roboter bei einem Sicherheitsverstoß in einen sicheren Zustand. Es gibt drei Typen: Alle Sicherheitsstoppfunktionen erfüllen die Anforderung 4.2.2.4 der IEC 61800-5-2.

* **Stopp 0**: Alle Motoren in den Verbindungsmodulen werden sofort stromlos geschaltet und angehalten.
* **Stopp 1**: Alle Motoren in den Verbindungsmodulen verlangsamen sich und kommen dann zum Stillstand. Anschließend wird die Stromzufuhr zu den Motoren unterbrochen.
* **Stopp 2**: Alle Motoren in den Verbindungsmodulen verlangsamen sich, und der Not-Aus-Schalter (SOS) wird aktiviert. Die Stromzufuhr zu allen Motoren bleibt bestehen.

Die Art des Stopps aufgrund einer Sicherheitsfunktionsverletzung wird im Menü für funktionsspezifische Parametereinstellungen festgelegt.
Die Stopptypeinstellungen für die nach ISO 10218-1 erforderlichen Stopps lauten wie folgt:

Parameterwerte können im Menü **\[System > 8: Sicherheitssystem > 1: Grundeinstellungen > 2: Stoppeinstellungen]** eingestellt werden.

<p align="center">
<img src="../../../_assets/safety_stop_param.png"></img>
<em><p align="center">Einstellungsbildschirm stoppen</p></em>
</p>

|  **Parameter** |                       **Beschreibung**                       |  **Standardeinstellung**  |
| :-------: | :------------------------------------------------: | :----------: |
| Notstopp | <p>Wählen Sie den Stopptyp für einen Notstopp</p><p>(Stopp 0, Stopp 1)</p> | Stopp 1 |
| Schutzstopp | <p>Wählen Sie den Stopptyp für einen Schutzstopp</p><p>(Stopp 0, Stopp 1, Stopp 2)</p> | Stopp 1 |
| Normalstopp | <p>Wählen Sie den Stopptyp für einen Normalstopp</p><p>(Stopp 0, Stopp 1)</p> | Stopp 1 |
| Manueller Stopp | <p>Stoppen bei Geschwindigkeitsüberschreitung im manuellen Modus</p><p>(Stopp 0, Stopp 1)</p> | Stopp 1 |


{% hint style="warning" %}
**\[Vorsicht]**: Sie sollten für jede Funktion durch eine Risikobewertung eine geeignete Abbruchmethode festlegen.
{% endhint %}
