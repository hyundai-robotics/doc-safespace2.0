
﻿
# 3.3.3.4 PROFINET

*1. PROFINET HW(BD671)**
![!Profinet Consol Image](../../../_assets/safetyio_profisafe/BD671_hw.PNG)

- Power Input : 24Vdc input
- Serial Communication Port : Connect Cable with BD642A Board
- PROFINET I/O Ethernet Port : Connect with PROFINET Master
- F/W Download Port : F/W download via J Link
- RS232 Port
- Baudrate : 115200 bps
- Data : 8bit, Parity : none, Stop bits : 1bit
- LED
- LED1 : Maintenance LED
- LED2 :  Diagnosis LED
- LED3 :  Run LED
- LED4 :  Error LED
- DCP ( LED3, LED4 Blinking)


*2. Profinet-Einstellungen*

Die PROFINET-Einstellungen können über die RS232-Kommunikation des BD671 geändert werden.
In diesem Kapitel werden die Parameter im Zusammenhang mit PROFINET erläutert.

![!Profinet Consol Image](../../../_assets/safetyio_profisafe/BD671_console.png)

- S : Submodul hinzufügen.
- s : Submodul entfernen.
- H : Liste der derzeit installierten Submodule anzeigen.
- n : Legen Sie den PROFINET-Gerätenamen fest.
- N : MAC-Adresse des PROFINET-Geräts festlegen.
- o : IP-Adresse, Subnetzmaske und Gateway festlegen.

*3. Modulinformationen**
- Anzahl der Module: 1 ea
- ID : 0x21
- Sub Module ID : 0x2
- Description :  8 Bytes I/O PS2v61
- Größe der Eingangsdaten: 13 Bytes
- Größe der Ausgangsdaten: 13 Bytes
- Zulässiger Steckplatz: 1
- Zulässiger Substeckplatz: 1

*4. Spec**
- PNIO Version : V2.43
- Conformance Class : B
- Application Class : Functional Safety
- Net load Class : II
- MRP (Media Redundancy Protocol)
- Device Redundancy (S2)
- Dynamic Reconfiguration (DR)
- I&M Records 0 ~ 4
- Supported Protocols : SNMP, LLDP
- Minimum Device Interval : 1 ms
- iParameter: Nicht unterstützt.
- Parametrierung im laufenden Betrieb: Nicht unterstützt.
- PROFIenergy: Nicht unterstützt.

> Die Parametereinstellung durch TP unten befindet sich in Vorbereitung.

![!Profinet TP Image](../../../_assets/safetyio_profisafe/profinet.PNG)

- PROFINET IO-Gerätename: Legen Sie den PROFINET-Gerätenamen fest. Die ersten Buchstaben des Gerätenamens sind fest als „HRC-PN-DEV-“ vorgegeben, die nachfolgenden Zahlen kann der Anwender frei wählen.
- IP-Adresse: Legen Sie die IP-Adresse fest. Beispiel: 192.168.1.100
- Subnetzmaske: Legen Sie die Subnetzmaske fest. Beispiel: 255.255.255.0
- Gateway: Legen Sie die Gateway-Adresse fest. Beispiel: 192.168.1.1
- MAC-Adresse: Dieser Parameter kann nicht festgelegt werden und ist schreibgeschützt.