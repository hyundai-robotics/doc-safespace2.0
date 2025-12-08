# 3.3.4.3 Sicherheitssignalzuweisung

Die Zuweisung von Sicherheitssignalen dient dazu, externe Signale wie Sicherheitseingänge/-ausgänge, zusätzliche Sicherheitseingänge/-ausgänge und Sicherheitskommunikationseingänge/-ausgänge mit verschiedenen logischen Signalen (Systemsicherheitseingänge/-ausgänge, Sicherheitsanwendungssignale) zu verbinden, über die die Robotersteuerung verfügt.
**\[System > 8: Sicherheitssystem > 2: Parametereinstellungen > 3: Sicherheitsein-/ausgänge > 1: Eingangs-/Ausgangsbelegung]** In diesem Menü können Sie die Parameterwerte einstellen. 

![](../../../_assets/safety_io/SIO_Alloc_diagram1.bmp)

![](../../../_assets/safety_io/SIO_Alloc_diagram2.bmp)

-------------------------------------------------------------------------

### Hinzufügen einer Sicherheitssignalzuweisung
1) Wählen Sie die gewünschte Funktion aus der Eingangs-/Ausgangsfunktionsliste auf der linken Seite aus.
2) Drücken Sie die Taste **[Auswählen]** und wählen Sie den Index (H/W-Kanal oder Bitnummer) aus.
3) Je nach Eingangs-/Ausgangsfunktionsliste können Sie einen Unterkanal auswählen, um eine detaillierte Funktionsnummer auszuwählen.

<p align="center">
<img src="../../../_assets/safety_io/io_alloc_param1.png"></img>
<em><p align="center">Einstellungsbildschirm für die Zuweisung von Sicherheitssignalen</p></em>
</p>

<p align="center">
<img src="../../../_assets/safety_io/io_alloc_param2.png"></img>
<em><p align="center">Bildschirm für detaillierte Einstellungen zur zusätzlichen Zuweisung von Sicherheitssignalen</p></em>
</p>


{% hint style="warning" %}
* Jede einzelne Eingangsfunktion kann nur mit einem einzigen Eingangskanal verbunden werden.<br>
* „Grundlegender Sicherheitseingang”, „Zusätzlicher Sicherheitseingang” und „Sicherheitskommunikationseingang” können nicht doppelt zugewiesen werden.<br>
* Wenn doppelte Eingangseinstellungen vorgenommen werden, tritt der Fehler „E52030 (x ch) Doppelte Zuweisung des Sicherheitseingangs” auf.

{% endhint %}

### Löschen einer Sicherheitssignalzuweisung
1) Wählen Sie eine bereits festgelegte Zuweisungsfunktion auf der rechten Seite des Bildschirms aus.
2) Drücken Sie die unten angezeigte Taste **[Verwerfen]**.

---

### Standardwerte für Sicherheitssignale

| **Kanal** | **Funktion** |
| :-------: | :------------------------------------------------: |
| Sicherheitseingangskanal 1 | Externer Not-Halt-Eingang (Notfall) |
| Sicherheitseingangskanal 2 | Allgemeiner Eingang für Sicherheitsvorrichtung (SGG) |
| Sicherheitseingangskanal 3 | Automatischer Eingang für Sicherheitsvorrichtung (SGA) |
| Sicherheitseingangskanal 4 | - |
| Sicherheitsausgangskanal 1 | Not-Halt-Aktivierungsstatus|

### Funktionsliste für Sicherheitseingangssignale

|  **Kanal** |     **Funktion**                       |       **Beschreibung**    |
| :-------: | :--------------------------: | :--------------------------------------------------: |
| Notfall | Externer Not-Halt-Eingang| OFFEN: Not-Halt aktiviert<br>GESCHLOSSEN: Not-Halt freigegeben |
| SGG| Allgemeiner Eingang für Sicherheitsvorrichtung| OFFEN: Sicherheitsvorrichtung offen (Gefahr) <br>GESCHLOSSEN: Sicherheitsvorrichtung geschlossen (Sicher) |
| SGA | Automatischer Eingang für Sicherheitsvorrichtung | OFFEN: Sicherheitsvorrichtung offen (Gefahr) <br>GESCHLOSSEN: Sicherheitsvorrichtung geschlossen (Sicher) |
| Sicherheitshalt | Sicherheitshalt-Eingang | OFFEN: Sicherheitshalt aktiviert <br>GESCHLOSSEN: Sicherheitshalt freigegeben |
| Normalhalt | Normalhalt-Eingang | OFFEN: Normalhalt aktiviert <br>GESCHLOSSEN: Normalhalt freigegeben |
| Zustimmschalter | Externer Zustimmschalter | OFFEN: Schalter freigegeben <br>GESCHLOSSEN: Betrieb möglich (Motorstartversuch) |
| Motor ein | Externer Motor ein | Motorstartversuch bei steigender Flanke |
| Remote | Eingang externe Betriebsart (Remote) | OFFEN: Betriebsartwechsel durch internes Modussignal <br>GESCHLOSSEN: Betriebsartwechsel durch externes Moduseingangssignal
| Manuell | Eingang externe Betriebsart (Manuell) | OFFEN: Keine Funktion <br>GESCHLOSSEN: Eingang externer manueller Betrieb |
| Auto | Eingang externe Betriebsart (Automatik) | OFFEN: Keine Funktion <br>GESCHLOSSEN: Eingang externer Automatikbetrieb |
| Arm-Begrenzung | Eingang Arm-Begrenzung| OFFEN: Eingang Begrenzungssignal (Gefahr) <br>GESCHLOSSEN: Begrenzungssignal geschlossen (Sicher) |
| Hauptachsen-Begrenzung | Eingang Hauptachsen-Begrenzung | OFFEN: Eingang Begrenzungssignal (Gefahr) <br>GESCHLOSSEN: Begrenzungssignal geschlossen (Sicher) |
| Zusatzachsen-Begrenzung | Eingang Zusatzachsen-Begrenzung | OFFEN: Eingang Begrenzungssignal (Gefahr) <br>GESCHLOSSEN: Begrenzungssignal geschlossen (Sicher) |
| Externe Achsen-Begrenzung | Eingang Externe Achsen-Begrenzung | OFFEN: Eingang Begrenzungssignal (Gefahr) <br>GESCHLOSSEN: Begrenzungssignal geschlossen (Sicher) |
| Überwachter Stillstand #1 ~ #8 | Stillstandsüberwachung<br>(sos_0~sos_7) | OFFEN: Funktion aktiviert<br>GESCHLOSSEN: Funktion deaktiviert |
| Gelenkgeschwindigkeits-Satz #1 ~ #8 | Gelenkgeschwindigkeit<br>(speed_0~speed_7) | OFFEN: Funktion aktiviert<br>GESCHLOSSEN: Funktion deaktiviert |
| TCP-Geschwindigkeits-Satz #1 ~ #16 | TCP-Geschwindigkeit<br>(speed_0~speed_15) | OFFEN: Funktion aktiviert<br>GESCHLOSSEN: Funktion deaktiviert |
| Gelenkwinkel #1 ~ #8 | Gelenkraum<br>(space_0~space7) | OFFEN: Funktion aktiviert<br>GESCHLOSSEN: Funktion deaktiviert |
| TCP-Position (Raum) #1 ~ #16 | TCP-Raum<br>(space_0~space15) | OFFEN: Funktion aktiviert<br>GESCHLOSSEN: Funktion deaktiviert |
| TCP-Orientierung #1 ~ #8 | Werkzeugorientierung<br>(orient_0~orient7) | OFFEN: Funktion aktiviert<br>GESCHLOSSEN: Funktion deaktiviert |
| Selbstkollision | Selbstkollision | OFFEN: Funktion aktiviert<br>GESCHLOSSEN: Funktion deaktiviert |
| Leistung #1 ~ #16 | Leistung<br>(power_0~power_15) | OFFEN: Funktion aktiviert<br>GESCHLOSSEN: Funktion deaktiviert |
| Momentum #1 ~ #16 | Momentum<br>(mmt_0~mmt_15) | OFFEN: Funktion aktiviert<br>GESCHLOSSEN: Funktion deaktiviert |
| Kollisionserkennung #1 ~ #16 | Kollisionserkennung<br>(coldet_0~coldet_15) | OFFEN: Funktion aktiviert<br>GESCHLOSSEN: Funktion deaktiviert |
| Geschwindigkeit & Abstand #1 ~ #84 | RePlan | OFFEN: Funktion aktiviert<br>GESCHLOSSEN: Funktion deaktiviert |
| Schalter Justagetest | Schalter Justagetest | OFFEN: Funktion aktiviert<br>GESCHLOSSEN: Funktion deaktiviert |

### Funktionsliste der Sicherheitsausgangssignale
|  **Kanal** |     **Funktion**                       |       **Beschreibung**    |
| :-------: | :--------------------------: |  :--------------------------------------------------: |
| Status Not-Halt-Aktivierung | Not-Halt-Status | OFFEN: Ein oder mehrere von TP, OP oder ext. Not-Halt sind gedrückt<br>GESCHLOSSEN: Kein TP, OP oder ext. Not-Halt gedrückt  |
| Status Sicherheitshalt-Aktivierung | Sicherheitshalt-Status | OFFEN: Nicht im Sicherheitshalt-Zustand<br>GESCHLOSSEN: Im Sicherheitshalt-Zustand |
| Status Normaler Halt-Aktivierung | Status Normaler Halt | OFFEN: Nicht im Zustand Normaler Halt<br>GESCHLOSSEN: Im Zustand Normaler Halt |
| Status Remote-Betrieb | Status Externer Betrieb | OFFEN: Interner Betriebsmodus<br>GESCHLOSSEN: Status Fernbetrieb |
| Status Handbetrieb | Status Handbetrieb | OFFEN: Nicht im Handbetrieb<br>GESCHLOSSEN: Im Handbetrieb |
| Status Automatikbetrieb | Status Automatikbetrieb | OFFEN: Nicht im Automatikbetrieb<br>GESCHLOSSEN: Im Automatikbetrieb|
| Status Motor Aus | Status Motor Aus | OFFEN: Zustand Motor Ein<br>GESCHLOSSEN: Zustand Motor Aus|
| Status Sicherheitsfunktion-Aktivierung | Status Sicherheitsfunktion-Aktivierung | OFFEN: Sicherheitsfunktion deaktiviert<br>GESCHLOSSEN: Sicherheitsfunktion aktiviert |
| Aktivierungsstatus Überwachter Stillstand | Aktivierungsstatus Überwachung Sicherer Betriebshalt | OFFEN: Überwachung Sicherer Betriebshalt deaktiviert<br>GESCHLOSSEN: Überwachung Sicherer Betriebshalt aktiviert |
| RePlan Aktivierungsstatus | RePlan Aktivierungsstatus | OFFEN: RePlan deaktiviert<br>GESCHLOSSEN: RePlan aktiviert |
| Verletzungsalarm | Status Sicherheitsfunktions-Verletzung | OFFEN: Sicherheitsfunktion verletzt<br>GESCHLOSSEN: Keine Verletzung der Sicherheitsfunktion |
| Verletzung Überwachter Stillstand #1~#8 | Verletzung Sicherer Betriebshalt<br>(sos_0~sos_7) | OFFEN: Sicherer Betriebshalt verletzt<br>GESCHLOSSEN: Keine Verletzung Sicherer Betriebshalt |
| Verletzung Gelenkgeschwindigkeits-Satz #1 ~ #8 | Verletzung Gelenkgeschwindigkeit<br>(speed_0~speed_7) | OFFEN: Gelenkgeschwindigkeit verletzt<br>GESCHLOSSEN: Keine Verletzung Gelenkgeschwindigkeit |
| Verletzung TCP-Geschwindigkeits-Satz #1 ~ #16 | Verletzung TCP-Geschwindigkeit<br>(speed_0~speed_15) | OFFEN: TCP-Geschwindigkeit verletzt<br>GESCHLOSSEN: Keine Verletzung TCP-Geschwindigkeit |
| Verletzung Gelenkwinkel #1~#8 | Verletzung Gelenkraum<br>(space_0~space7) | OFFEN: Verletzung Gelenkraum<br>GESCHLOSSEN: Keine Verletzung Gelenkraum |
| Verletzung TCP-Position #1~#16 | Verletzung TCP-Raum<br>(space_0~space15) | OFFEN: TCP-Raum verletzt<br>GESCHLOSSEN: Keine Verletzung TCP-Raum |
| Verletzung TCP-Orientierung #1~#8 | Werkzeugorientierung<br>(orient_0~orient7) | OFFEN: Werkzeugorientierung verletzt<br>GESCHLOSSEN: Keine Verletzung Werkzeugorientierung |
| Selbstkollisionserkennung | Selbstkollisionserkennung | OFFEN: Selbstkollision erkannt<br>GESCHLOSSEN: Keine Selbstkollision |
| Verletzung Leistung #1~#16 | Leistungsverletzung<br>(power_0~power_15) | OFFEN: Leistung verletzt (Grenzwert überschritten)<br> GESCHLOSSEN: Keine Leistungsverletzung |
| Verletzung Momentum #1~#16 | Momentum-Verletzung<br>(mmt_0~mmt_15) | OFFEN: Momentum verletzt<br> GESCHLOSSEN: Keine Momentum-Verletzung |
| Verletzung Kollisionserkennung #1~#16 | Kollisionserkennung <br>(coldet_0~coldet_15) | OFFEN: Kollision erkannt<br> GESCHLOSSEN: Keine Kollision |
| Fehler Justagetest | Fehler Justagetest | OFFEN: Fehler beim Justagetest aufgetreten<br> GESCHLOSSEN: Kein Fehler beim Justagetest |
| Fehler Bremstest | Fehler Bremstest | OFFEN: Fehler beim Bremstest aufgetreten<br> GESCHLOSSEN: Kein Fehler beim Bremstest |

{% hint style="info" %}
* In der Sicherheitskommunikation ist **OFFEN = Bit 0**, **GESCHLOSSEN = Bit 1** definiert.

{% endhint %}
