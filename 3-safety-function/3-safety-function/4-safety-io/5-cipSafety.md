

# 3.3.4.5 CIP Safety

## 1. CIP Safety ?
- CIP Safety ist ein Sicherheitskommunikationsprotokoll, das das Standard-Common Industrial Protocol (CIP) erweitert.
- Ermöglicht den sicheren Datenaustausch über EtherNet/IP und DeviceNet unter Verwendung des „Black Channel“-Prinzips.
- Entspricht Sicherheitsstandards wie IEC 61508 und ISO 13849 durch Mechanismen wie Zeitüberwachung, Redundanz und CRC-Prüfungen.

## 2. Spezifikationen
### 2.1 EtherNet/IP
- Digitaler Eingang: 0 ~ 240 Bytes
- Digitaler Ausgang: 0 ~ 240 Bytes
- Kommunikationszyklus: 1 ~ 3000 msec
- Unterstützte Kommunikationsgeschwindigkeit: 10 oder 100 MBit/s

### 2.2 CIP Safety
- Sicherheits-E/A: 8/8 Bytes 
- Kommunikationszyklus: 20 ~ 100 msec


## 3. CIP-Safety-Parameter

![](../../../_assets/cipSafety/cipSafety_Parameters.png)

 - Aktivieren/Deaktivieren: Legt fest, ob die CIP-Safety-Funktion verwendet werden soll.
 - SNN: Legt die Sicherheitsnetzwerknummer fest.
 - Configure Signature : Reserved



## 4. CIP-Safety-Konfigurationsverfahren

1) Anschluss des Hi7 EtherNet/IP-Adapters und des EtherNet/IP-Scanners
2) Hinzufügen der EDS-Datei über das Engineering-Tool (Studio 5000)
3) CIP-Safety-Steuerungseinstellungen (Studio 5000)
4) Hi7-Einstellungen (TP-Benutzeroberfläche)
4.1) EtherNet/IP-Einstellungen
4.2) CIP-Safety-Einstellungen
5) Überprüfen des EtherNet/IP- und CIP-Safety-Kommunikationsstatus
6) Zuweisung von Sicherheitssignalen


### 1 Anschluss des Hi7 EtherNet/IP-Adapters und des EtherNet/IP-Scanners
![](../../../_assets/cipSafety/connect.png)

### 2 Hinzufügen der EDS-Datei über das Engineering-Tool (Studio 5000)
- Installieren Sie die EDS-Datei (Hi7_EIP_250203.eds) mit dem „Device Description File Installation Tool”.
### 3 CIP-Safety-Steuerungseinstellungen (Studio 5000)
1) Starten Sie Studio 5000 und erstellen Sie ein neues Projekt.
2) Wählen Sie im Controller Organizer (Steuerungsorganisator) eine Steuerung aus, die CIP- Safety-Kommunikation unterstützt (z. B. CPU 1769-L30ERMS), wählen Sie Ethernet, klicken Sie mit der rechten Maustaste und klicken Sie auf „Neues Modul“.
3) Suchen Sie „Hi7 EIP Adapter“ und klicken Sie auf die Schaltfläche „Erstellen“.<br>
![CIP Safety](../../../_assets/cipSafety/new_module.png)

4) Legen Sie den Gerätenamen im Feld „Name“ fest.
5) Legen Sie die IP-Adresse fest, z. B. 192.168.4.150.
6) Legen Sie die Sicherheitsnetzwerknummer fest, z. B. 1111_2222_3333.<br>
![CIP Safety](../../../_assets/cipSafety/Setting_SNN.png)


7) Klicken Sie in der Moduldefinition auf die Schaltfläche „Ändern“ und legen Sie die Größe der Sicherheits-E/A und Standard-E/A fest.
- Standard-E/A (exklusiver Eigentümer): 240 Bytes
- Sicherheits-E/A: jeweils 8 Byte
8) Bitte setzen Sie „Konfigurationssignatur” nicht.
9) Schließen Sie das Fenster „Modultyp auswählen”.<br>
![CIP Safety](../../../_assets/cipSafety/Setting_module.png)
10) Überprüfen Sie, ob das Modul hinzugefügt wurde.<br>
![CIP Safety](../../../_assets/cipSafety/module_added.png)
11) Klicken Sie im Menü der Symbolleiste auf die Schaltfläche „Offline” und anschließend auf die Schaltfläche „Herunterladen”.<br>
![CIP Safety](../../../_assets/cipSafety/download.png)
12) Nachdem die konfigurierten Werte heruntergeladen wurden, ändern Sie die Umschaltfläche von „Guard Logix“ von PROG auf RUN.
### 4) Hi7-Einstellungen (TP-Benutzeroberfläche)
#### 4.1 EtherNet/IP-Einstellungen
1) Navigieren Sie zum Menü: System → Steuerungsparameter → Industrielle Kommunikation → EtherNet/IP-Einstellungen
2) Protokolleinstellung = Adapter
3) Stellen Sie den LAN-Port für den EtherNet/IP-Adapter auf LAN2 ein.
4) Stellen Sie die Eingangs-/Ausgangsgröße auf jeweils 240 Byte ein.
5) Ändern Sie die übrigen Einstellungen wie in der Abbildung gezeigt nicht.<br>
![CIP Safety](../../../_assets/cipSafety/ethernetIP.png)

#### 4.2 CIP-Safety-Einstellungen
1) Navigieren Sie zum Menü: System → Sicherheitssystem → Parametereinstellungen → Sicherheitseingang/ -ausgang → CIP Safety.
2) Schalten Sie die Schaltfläche EIN.
3) Stellen Sie SNN beispielsweise auf 1111_2222_3333 ein.
4) Klicken Sie auf die Schaltfläche „Übernehmen“.
5) Starten Sie die Robotersteuerung neu.<br>
![CIP Safety](../../../_assets/cipSafety/cipSafety_Parameters.png)
### 5 Überprüfen Sie den Kommunikationsstatus.
#### 5.1 EtherNet/IP
1) Überprüfen Sie, ob die Lizenz-LED leuchtet.
2) Überprüfen Sie, ob die Run-LED leuchtet.
3) Überprüfen Sie, ob die Kommunikations-LED leuchtet.
4) Wenn die Fehler-LED leuchtet, überprüfen Sie den Fehlernamen.<br>
![CIP Safety](../../../_assets/cipSafety/eip_status.png)
#### 5.2 CIP Safety
1) Überprüfen Sie, ob der Geräte-Status „Ausführung“ lautet.
2) Überprüfen Sie, ob der Kommunikationsstatus „Online, verbunden“ lautet.
3) Überprüfen Sie, ob die IO-Anzahl kontinuierlich ansteigt.<br>
![CIP Safety](../../../_assets/cipSafety/cipsafety_status.png)

### 6 Sicherheitssignal-Zuweisung
#### 6.1 CIP-Safety-E/A-Zuweisung<br>
* [3.3.3.3 Sicherheitssignal-Zuweisung](3-safety-function/3-safety-function/3-safety-io/3-Linker.md) Siehe Seite
#### 6.2 Beispiel für CIP-Safety-E/A-Zuweisung
1) CIP-Safety-Eingang (Richtung Master -> Slave)
1ch(0 bit) = Arm Limit<br>
![CIP Safety](../../../_assets/cipSafety/alloc_in.png)<br>
<br> <br>
![CIP Safety](../../../_assets/cipSafety/alloc_in2.png)<br>

2) CIP-Safety-Ausgang (Richtung Slave -> Master)
1ch(0 bit) = E-Stop Status<br>
![CIP Safety](../../../_assets/cipSafety/alloc_out.png)<br>
<br> <br>
![CIP Safety](../../../_assets/cipSafety/alloc_out2.png)<br>

