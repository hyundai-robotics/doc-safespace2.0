# 3.3.4.1 Grundlegende Sicherheits-Eingangs-/Ausgangssignale

Legen Sie die Parameter für die Sicherheits-Eingangs-/Ausgangssignale fest.  
Es gibt 4 Eingangssignale und 1 Ausgangssignal, die alle als Doppelsignale fungieren.
**\[System > 8: Sicherheitssystem > 2: Parametereinstellungen > 3: Sicherheitsein-/ausgänge > 2: Grundlegende Ein-/Ausgänge]** In diesem Menü können Sie die Parameterwerte einstellen. 

## 1. Eingangssignaleinstellungen

<p align="center">
<img src="../../../_assets/safety_io/def_input.png"></img>
<em><p align="center">Bildschirm „Grundlegende Ein-/Ausgangseinstellungen“ (Eingang)</p></em>
</p>

| Parameter <br>[Einheit]          | Beschreibung                                                                                                                                       | Eingangsbereich       | Standard |
|:------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|:--------------:|:------:|
| Impulstest                  | Legen Sie fest, ob für jeden Kanal ein Impulstest verwendet werden soll.                                                                                                     | Aktivieren/Deaktivieren | Deaktivieren |
| Fehlerhaltezeit <br>[msec] | Wenn in einem Kanal ein Fehler auftritt, wechselt das System erst nach Ablauf der **Fehlerhaltezeit** vom Fail-Safe-Zustand in den aktuellen Eingangsstatus, selbst wenn der Fehler behoben wurde.<br>Es können nur durch 5 teilbare Werte eingegeben werden. | 0 ~ 65530      | 1000   |
| Filterzeit <br>[msec]      | Das gleiche Signal muss während der für jeden Kanal eingestellten **Filterzeit** eingegeben werden, damit es als gültiges Signal verarbeitet wird.<br>Es können nur durch 5 teilbare Werte eingegeben werden.                       | 0 ~ 500        | 100    |
| Diskrepanzzeit <br>[msec] | Grundlegende Eingangssignale werden als gültige Signale verarbeitet, wenn die beiden dualen Signale identisch sind. <br>Ein Alarm wird ausgelöst, wenn die beiden Signale länger als die eingestellte **Diskrepanzzeit** voneinander abweichen. <br>Es können nur durch 5 teilbare Werte eingegeben werden. | 0 ~ 5000       | 1000   |

### Verdrahtungsbeispiel)
![](../../../_assets/safety_io/CN_SI1.bmp)


## 2. Ausgangssignaleinstellungen

<p align="center">
<img src="../../../_assets/safety_io/def_output.png"></img>
<em><p align="center">Bildschirm „Grundlegende Ein-/Ausgangseinstellungen“ (Ausgang)</p></em>
</p>

| Parameter <br>[Einheit]          | Beschreibung                                                                                                                                       | Eingangsbereich       | Standard |
|:------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|:--------------:|:------:|
| Impulstest                  | Legen Sie fest, ob für jeden Kanal ein Impulstest verwendet werden soll.                                                                                                     | Aktivieren/Deaktivieren | Deaktivieren |
| Fehlerhaltezeit <br>[ms] | Wenn in einem Kanal ein Fehler auftritt, bleibt das System während der **Fehlerhaltezeit** im Zustand **Offen (Fail-Safe)**, auch wenn der Fehler behoben wurde. Danach wechselt es zum normalen Ausgangszustand.<br>Es können nur durch 5 teilbare Werte eingegeben werden. | 0 ~ 65530      | 1000   |

### Verdrahtungsbeispiel)
![](../../../_assets/safety_io/CN_SO1.bmp)


