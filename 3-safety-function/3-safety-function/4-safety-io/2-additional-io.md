# 3.3.4.2 Erweiterte Sicherheits-Eingangs-/Ausgangssignale

Legen Sie die Parameter für zusätzliche Sicherheits-Eingangs-/Ausgangssignale fest. Es besteht aus 8 Eingangssignalen und 8 Ausgangssignalen, die alle als Doppelsignale fungieren.
**\[System > 8: Sicherheitssystem > 2: Parametereinstellungen > 3: Sicherheitsein-/ausgänge > 3: Erweiterte Ein-/Ausgänge]** In diesem Menü können Sie die Parameterwerte einstellen. 

## 1. Zusätzliche Sicherheits-Eingangs-/Ausgangssignale

<p align="center">
<img src="../../../_assets/safety_io/add_io.png"></img>
<em><p align="center">Bildschirm „Erweiterte Ein-/Ausgangseinstellungen“</p></em>
</p>

| Parameter [Einheit]          | Beschreibung                                                                                                                                       | Eingangsbereich       | Standard |
|:---------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------:|:--------------:|:------:|
| Aktivieren                      | Legen Sie fest, ob die erweiterten Sicherheits-Ein-/Ausgangssignale aktiviert oder deaktiviert werden sollen.                                                                                       | Aktivieren/Deaktivieren | Deaktivieren |
| Filterzeit <br>[msec]          |  Für jeden Eingangskanal müssen während der **Filterzeit** konstante Signale eingegeben werden, damit die Signale als gültige Signale verarbeitet werden. <br>Es können nur durch 5 teilbare Werte eingegeben werden.                           | 0 ~ 500        | 100    |
| Diskrepanzzeit <br>[msec]     | Erweiterte Sicherheits-Eingangs-/Ausgangssignale werden als gültige Signale verarbeitet, wenn die beiden dualen Signale denselben Wert haben. <br>Ein Alarm wird ausgelöst, wenn die beiden Signale länger als die **Diskrepanzzeit** voneinander abweichen. <br>Es können nur durch 5 teilbare Werte eingegeben werden. | 0 ~ 5000       | 1000   |
| Haltezeit für Eingangsfehler <br>[msec] | Wenn in einem Kanal ein Fehler auftritt, wechselt das System erst nach Ablauf der eingestellten Zeit vom Fail-Safe-Zustand in den aktuellen Eingangsstatus, selbst wenn der Fehler behoben wurde. <br>Es können nur durch 5 teilbare Werte eingegeben werden.             | 0 ~ 65530      | 1000   |
| Haltezeit für Ausgangsfehler <br>[msec] | Wenn in einem Kanal ein Fehler auftritt, bleibt das System während der eingestellten Zeit im Zustand **„Offen” (Fail-Safe)**, auch wenn der Fehler behoben wurde.<br>Danach wechselt es zum normalen Ausgangszustand.<br>Es können nur durch 5 teilbare Werte eingegeben werden.   | 0 ~ 65530      | 1000   |

### Beispiel für die Verdrahtung eines zusätzlichen Sicherheitseingangs)
![](../../../_assets/safety_io/CN_SI2.bmp)
### Beispiel für die Verdrahtung eines zusätzlichen Sicherheitsausgangs)
![](../../../_assets/safety_io/CN_SO2.bmp)

