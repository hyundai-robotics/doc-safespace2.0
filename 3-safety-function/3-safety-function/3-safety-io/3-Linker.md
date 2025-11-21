# 3.3.3.3 Sicherheitssignalzuweisung

Die Sicherheitssignalzuweisung dient dazu, externe Signale wie Sicherheitseingänge/-ausgänge, zusätzliche Sicherheitseingänge/-ausgänge und Sicherheitskommunikationseingänge/-ausgänge mit verschiedenen logischen Signalen oder Zustandsvariablen der Robotersteuerung zu verbinden.

![!Additional Input Image](../../../_assets/safety_io/io_alloc.PNG)

### Hinzufügen einer Sicherheitssignalzuweisung
1) Wählen Sie die gewünschte Funktion aus der E/A-Funktionsliste auf der linken Seite aus.
2) **2) Drücken Sie die Taste [PICK] und wählen Sie den Index (H/W-Kanal oder Bitnummer) aus.** 버튼을 누르고 인덱스(H/W 채널 또는 Bit 번호)를 선택
3) Entsprechend der E/A-Funktionsliste können Sie eine Untergruppe auswählen, um eine detaillierte Funktionsnummer auszuwählen.

![!Additional Input Image](../../../_assets/safety_io/io_alloc2.PNG)

### Löschen einer Sicherheitssignalzuweisung
1) Wählen Sie eine bereits festgelegte Zuweisungsfunktion auf der rechten Seite des Bildschirms aus.
2) 아래에 보이는 **2) Drücken Sie die unten angezeigte Taste [Verwerfen].** 버튼을 누름

---

### Standardwerte für Sicherheitssignale

|  **|  Kanal |     Funktion                       |** |     **|  Kanal |     Funktion                       |**                       |
| :-------: | :------------------------------------------------: |
| Sicherheitseingangskanal 1 | Externer Not-Halt-Eingang (Notfall) |
| Sicherheitseingangskanal 2 | Allgemeiner Eingang für Sicherheitsvorrichtung (SGG) |
| Sicherheitseingangskanal 3 | Automatischer Eingang für Sicherheitsvorrichtung (SGA) |
| Sicherheitseingangskanal 4 | - |
| Sicherheitsausgangskanal 1 | Not-Halt-Aktivierungsstatus|

### Liste der Sicherheitssignalfunktionen

|  **|  Kanal |     Funktion                       |** |     **|  Kanal |     Funktion                       |**                       |
| :-------: | :------------------------------------------------: |
| Notfall | Externer Not-Halt-Eingang|
| SGG| Allgemeiner Eingang für Sicherheitsvorrichtung|
| SGA | Automatischer Eingang für Sicherheitsvorrichtung|
| Protective stop | - |
| Normal stop | - |
| Zustimmschalter | Externer Zustimmschalter |
| Motor ein | Externer Motor ein |
| Remote | Externer Modus-Eingang (Remote) |
| Manuell | Externer Modus-Eingang (Manuell) |
| Auto | Externer Moduseingang (Auto) |
| Arm-Grenze | Arm-Grenzeingang|
| Primärachsen-Grenze | Eingang für Primärachsen-Grenze |
| Zusatzachsen-Grenze | Eingang für Zusatzachsen-Grenze |
| Grenze für externe Achsen | Eingang für Grenze für externe Achsen |
| Monitored standstill #1 ~ #8 | - |
| Joint speed set #1 ~ #8 | - |
| TCP speed set #1 ~ #16 | - |
| Joint angle #1 ~ #8 | - |
| TCP position(cell) #1 ~ #16 | - |
| TCP orientation #1 ~ #8 | - |
| Self collision | - |
| Power #1 ~ #16 | - |
| Momentum #1 ~ #16 | - |
| Collision detection #1 ~ #16 | - |
| Speed & separation #1 ~ #84 | - |
| Mastering test switch| - |