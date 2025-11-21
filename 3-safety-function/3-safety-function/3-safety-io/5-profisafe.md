

# 3.3.3.5 PROFIsafe

*1. PROFIsafe-Einstellungen*

![!Profisafe Consol Image](../../../_assets/safetyio_profisafe/BD671_console.png)

- Quelladresse: Quelladresse festlegen. (Fest auf 1)
- Zieladresse: Zieladresse festlegen. (Einstellbereich: 1 ~ 65534)
 
*2. Referenzinformationen*
  
- Adresstyp: Adresstyp 1 (nur Zieladresse aktiviert)
- Reaktion auf Device_Fault: Wenn dieses Gerät in den Zustand „Fault“ (Fehler) wechselt, werden alle F-Ausgänge in den Zustand „Fail-safe“ (Ausfallsicherheit) (0) versetzt. Nachdem der Fehlerzustand des Geräts behoben wurde, ist ein Vorgang wie „Global-Acknowledge“ (Globale Bestätigung) vom F-Host erforderlich, um das F-Gerät wieder zu integrieren.
 
*3. Alarmliste*

|Alarm No.|Alarm Decsription  |
|--|--|
| 0x10 |Fehler bei der Parametereinstellung |
| 0x13 |Kommunikationsfehler |
| 0x19 |Fehler bei der Sicherheitsfunktion |
| 0x1C |Interner Kommunikationsfehler 1 |
| 0x1D |Interner Kommunikationsfehler 2 |
| 0x1E |Interner Kommunikationsfehler 3 |
| 0x40 |Fehler bei der Einstellung der F-Dest-Adresse |
| 0x41 |Der Wert der F-Dest-Adresse ist ungültig |
| 0x42 |Fehler bei der Einstellung der F-Src-Adresse |
| 0x43 |Der Wert des F-Watchdogs ist ungültig
| 0x45 |Fehler bei der F-CRC-Länge |
| 0x46 |Fehler bei der F-PAR-Version |
| 0x47 |CRC1-Fehler |
| 0x4C |F-Block-ID-Fehler |
| 0x4D |CRC2-Fehler|
| 0x4E |F-Watchdog-Zeitüberschreitung|


> Die Parametereinstellung durch TP unten befindet sich in Vorbereitung.

![!Profisafe TP Image](../../../_assets/safetyio_profisafe/profisafe.PNG)

- Quelladresse: Quelladresse festlegen. (Fest auf 1)
- Zieladresse: Zieladresse festlegen. (Einstellbereich: 1 ~ 65534)
