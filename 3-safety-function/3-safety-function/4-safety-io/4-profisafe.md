

# 3.3.4.4 PROFIsafe

## 1. PROFIsafe ?
- Ein Sicherheitsprotokoll (Sicherheitsprofil), das auf PROFINET/PROFIBUS arbeitet.
- Überträgt Sicherheitsdaten über den Standard-PROFINET-Kommunikationskanal („Black Channel“).
- Unterstützt die Übertragung von Sicherheitssignalen ohne zusätzliche Verkabelung.

## 2. PROFINET- & PROFIsafe-Spezifikationen
- Digitaler Eingang: 50, 120 und 240 Byte (wählen Sie eine Byte-Anzahl aus) 
- Digitaler Ausgang: 50, 120 und 240 Byte (wählen Sie eine Byte-Anzahl aus) 
- Sicherheits-E/A: 8/8 Byte (aktiviert oder deaktiviert) 
- Mindestkommunikationszyklus: 1 ms
- Unterstützte Kommunikationsgeschwindigkeit: 10 oder 100 MBit/s
- Conformance Class : B
- Netload Class : II
- Optional Feature : Legacy, MRP

## 3. PROFIsafe-Parameter

![](../../../_assets/safetyio_profisafe/profisafe_param.png)

 - Quelladresse: Legt die Quelladresse fest. (Fest auf 1 eingestellt)
 - Zieladresse: Legt die Zieladresse fest. (Einstellbereich: 1 ~ 99)

  ***Anmerkungen*** 
 - Adresstyp:  Adresstyp 1 (nur Zieladresse ist aktiviert)
 - Reaktion auf Device_Fault: Wenn dieses Gerät in den Zustand „Fault“ (Fehler) wechselt, werden alle F-Ausgänge in den Zustand „Fail-safe“ (Ausfallsicherheit) (0) versetzt. Nachdem der Fehlerzustand des Geräts behoben wurde, ist ein Vorgang wie „Global-Acknowledge“ (Globale Bestätigung) vom F-Host erforderlich, um das F-Gerät wieder zu integrieren.


## 4. PROFIsafe-Konfigurationsverfahren

1) Anschluss von BD671, F-Host und Hi7 Com
2) Registrierung der GSDML-Datei (TIA Portal)
3) PROFIsafe-Controller-Einstellungen (TIA Portal)
<br>3.1) PROFINET-Einstellungen
<br>3.2) PROFIsafe-Einstellungen
4) Hi7-Einstellungen (TP-Benutzeroberfläche)
<br>4.1) PROFINET-Einstellungen
<br>4.2) PROFIsafe-Einstellungen
5) Verifizierung der PROFINET- und PROFIsafe-Kommunikation
6) PROFINET-E/A-Signalzuweisung (FB-Block-Einstellungen)
7) PROFIsafe-E/A-Signalzuweisung


### 4.1 Anschluss von BD671, F-Host und Hi7 Com

#### 4.1.1 LAN-Kabelverbindung
1) Verbinden Sie den „PROFIsafe F-Host“ über ein LAN-Kabel mit dem BD671.
2) Überprüfen Sie, ob die Link-LED blinkt.
3) Verbinden Sie den LAN3-Anschluss der Hi7 COM und den BD671 mit einem LAN-Kabel.
4) Überprüfen Sie, ob die Link-LED blinkt.

![](../../../_assets/safetyio_profisafe/profisafe_connect.png)

#### 4.1.2 Hi7 Com-Verbindungseinstellungen
1) Navigieren Sie wie folgt zum Menü: System -> Steuerungsparameter -> Industrielle Kommunikation -> EtherCAT-Master-Einstellungen
2) Konfigurieren Sie die Einstellungen wie unten gezeigt.
- EtherCAT Master : ON
- Port : LAN3
3) Wählen Sie „OptionBD – PROFINET_IO” aus der Slave-Liste aus und drücken Sie die Schaltfläche „Übernehmen”.
4) Starten Sie die Hi7-Robotersteuerung neu.
5) Überprüfen Sie nach dem Neustart den Status der Run-LEDs, Kommunikations-LEDs und Fehler-LEDs.

![](../../../_assets/safetyio_profisafe/EC_master_setting1.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/EC_master_setting2.png)


### 4.2 Registrierung der GSDML-Datei (TIA Portal)
1) Starten Sie das TIA Portal.
2) Navigieren Sie wie rechts im Menü gezeigt: [Extras] → [Gerätebeschreibungsdateien (GSD) verwalten].
3) Klicken Sie auf die Schaltfläche „…“ und legen Sie das Verzeichnis fest, in dem sich die GSDML-Datei befindet.
4) Wählen Sie „GSDML-V2.43-Hyundai-Robotics-HI6-20250418.xml” aus der auf dem Bildschirm angezeigten Liste aus und klicken Sie auf die Schaltfläche [Installieren].
5) Überprüfen Sie, ob die Datei als neues Gerät im Hardwarekatalog registriert wurde. <br>
![](../../../_assets/safetyio_profisafe/profisafe_gsdmal.png)

### 4.3 PROFIsafe-Controller-Einstellungen (TIA Portal)
#### 4.3.1 PROFINET-Einstellungen
1) Starten Sie TIA Portal und erstellen Sie ein neues Projekt.
2) Doppelklicken Sie auf den Bereich Geräte & Netze, um ihn zu öffnen.<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network.png)

3) Wählen Sie einen Controller aus, der PROFIsafe-Kommunikation unterstützt (z. B. CPU 1511F-1 PN), und ziehen Sie ihn in die Netzwerkansicht.
4) Fügen Sie das im vorherigen Schritt hinzugefügte Gerät (HRC, PROFINET I/O DAP) aus dem Hardwarekatalog hinzu und ziehen Sie es in die Netzwerkansicht.
5) Verbinden Sie die beiden Geräte, indem Sie die LAN-Ports in den Geräteabbildungen per Drag & Drop verschieben.<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network2.png)

6) Doppelklicken Sie im Bildschirm „Geräte & Netze“ auf das HRC-IO-Gerät.
7) Wählen Sie den gewünschten Slot aus.
8) Ziehen Sie das gewünschte Modul (DI, DO oder PROFIsafe-E/A) aus dem Katalog auf der rechten Seite und verschieben Sie es in das Fenster „Geräteübersicht“.<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network3.png)

9) Doppelklicken Sie im Bildschirm „Geräte & Netze“ auf das HRC-IO-Gerät.
10) Klicken Sie erneut auf das HRC-IO-Gerät, um den Bildschirm „Einstellungen“ zu öffnen.
11) Navigieren Sie unten zur Registerkarte „Allgemein“.
12) Wählen Sie im Menü auf der linken Seite Ethernet-Adressen aus.
13) Deaktivieren Sie „PROFINET-Gerätenamen automatisch generieren“.
14) Setzen Sie „PROFINET-Gerätename“ auf „hd-hrc-0“ und speichern Sie die Einstellung.<br>
![](../../../_assets/safetyio_profisafe/profisafe_device_network4.png)

#### 4.3.2 PROFIsafe-Einstellungen
1) Doppelklicken Sie im Bildschirm „Geräte & Netze“ auf das HRC-IO-Gerät.
2) Wählen Sie den PROFIsafe-Slot im Bildschirm „Geräteübersicht“ auf der rechten Seite aus.
3) Der Bildschirm für die PROFIsafe-Kommunikationseinstellungen erscheint im unteren Bereich.
4) Klicken Sie auf die Registerkarte „PROFIsafe“.
5) Setzen Sie „F_Dest_Add“ auf „1“.


### 4.4 Hi7-Einstellungen (TP-Benutzeroberfläche)
#### 4.4.1 PROFINET-Einstellungen
1) Stellen Sie die Parameter auf die gleichen Werte ein, die im F-Host wie folgt festgelegt wurden:
- PROFINET IO Device Name : hd-hrc-0
- Slot 1 : Digital Input : 240
- Slot 2 : Digital Output : 240
- Slot 3 : Safety I/O : Yes
- (Die IP-Adresse muss nicht geändert werden.)
2) Klicken Sie auf die Schaltfläche „Übernehmen“.<br>
![](../../../_assets/safetyio_profisafe/4_1_profinet_config.png)

#### 4.4.2 PROFIsafe-Einstellungen

1) Setzen Sie die Zieladresse auf 1, entsprechend dem im vorherigen Kapitel festgelegten Wert.
2) Klicken Sie auf die Schaltfläche „Übernehmen“.<br>
![](../../../_assets/safetyio_profisafe/4_2_profisafe_config.png)

### 4.5 Überprüfung der PROFINET- und PROFIsafe-Kommunikation

### 4.5.1 Safety-KOP-Programm (TIA Portal)
1) Erstellen Sie auf der Registerkarte „Geräteübersicht“ ein KOP-Programm (Kontaktplan) wie unten gezeigt und laden Sie es auf die Steuerung herunter.<br>
![](../../../_assets/safetyio_profisafe/5_1_Safety_Ladder.png)
2) Überprüfen Sie nach dem Herunterladen, ob auf dem Bildschirm „Dezentrale Peripherie“ (Distribution I/O) ein grünes Häkchen angezeigt wird.<br>
![](../../../_assets/safetyio_profisafe/5_1_Safety_Ladder2.png)

### 4.5.2 TP-Bildschirm
1) PROFINET
Navigieren Sie im Menü zu „System“ -> „Sicherheitssystem“ -> „Überwachung“ -> „PROFINET-Status“.<br>
![](../../../_assets/safetyio_profisafe/5_2_pnio_status.png)
- Überprüfen Sie die Statusinformationen für jeden Slot.
- Überprüfen Sie, ob der Zähler kontinuierlich ansteigt.

2) PROFIsafe
Navigieren Sie im Menü zu „System“ -> „Sicherheitssystem“ -> „Überwachung“ -> „PROFIsafe-Status“.<br>
![](../../../_assets/safetyio_profisafe/5_2_profisafe_status.png)
- Prüfen Sie, ob der FappState auf CYCLE Data EX steht.
- Überprüfen Sie, ob der Zähler kontinuierlich ansteigt.

### 4.6 PROFINET-E/A-Signalzuweisung (FB-Block-Einstellungen)
1) Navigieren Sie zu System → Steuerungsparameter → Ein-/Ausgangssignal-Einstellungen → FB-Block-Zuweisung.
2) Ändern Sie die Blockeinstellungen nach Bedarf auf PROFINET-E/A, so viele wie benötigt werden (bis zu zwei).
 (Die maximale PROFINET-E/A-Größe beträgt 240 Byte und die Größe des einzelnen FB-Blocks beträgt 120 Byte. Daher werden **alle Einstellungen, die zwei überschreiten, ignoriert.**)<br>
![](../../../_assets/safetyio_profisafe/6_fb_block.png)

3) Navigieren Sie zusätzlich zum Menü „Bedingungseinstellungen“ und überprüfen Sie, ob der SPS-Betriebsmodus auf AUS steht.<br>
![](../../../_assets/safetyio_profisafe/6_1_condition.png)
4) Prüfen Sie die Ein-/Ausgangssignale auf dem TIA Portal-Bildschirm und dem Bildschirm für Allgemeine E/A.<br>
![](../../../_assets/safetyio_profisafe/6_3_public_io.png)

### 4.7 PROFIsafe-E/A-Signalzuweisung
1) PROFIsafe-E/A-Signalzuweisung
* Siehe Seite [3.3.4.3 Sicherheitssignal-Zuweisung](../4-safety-io/3-Linker.md)

2) Beispiel für PROFIsafe-E/A-Signalzuweisung
<br>
<br>2-1) PROFIsafe-Eingang (Richtung Master -> Slave)
[Setzen Sie Kanal 1 (0 Bit) auf Arm-Begrenzung] <br>
![](../../../_assets/safetyio_profisafe/7_PS_in.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/7_PS_in2.png)
<br> <br>
2-2) PROFIsafe-Ausgang (Richtung Slave -> Master)
<br> <br>
[Setzen Sie Kanal 1 (0 Bit) auf Not-Halt-Status]<br>
![](../../../_assets/safetyio_profisafe/7_PS_out.png)
<br> <br>
![](../../../_assets/safetyio_profisafe/7_PS_out2.png)



