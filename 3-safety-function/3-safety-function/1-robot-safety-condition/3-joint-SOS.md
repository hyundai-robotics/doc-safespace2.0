# 1.6.2 Stoppüberwachung

Die Stoppüberwachung ist eine Funktion, die überwacht, ob während des Roboter-Stoppbetriebs ungewöhnliche Bewegungen der einzelnen Achsen auftreten. Stopp 0 wird sofort aktiviert, wenn der Schwellenwert verletzt wird.

Über das Menü \[System > 4: Anwendungsparameter > 18: SafeSpace2.0 > Parametereinstellungen > Roboterbeschränkung > Gelenk-SOS]* können Sie die Parameterwerte festlegen.

![!Bildschirm zur Einstellung der Stoppüberwachungsparameter](<../../../_assets/joint_sos_param.png>)

|  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |** |                       **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**                       |  **|  Parameter |                       Beschreibung                       |  Standardeinstellung  |**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Funktionsaktivierungsstatus</p><p>(Off/On/Safety Input)</p> |   Off  |
| Joint OnOff |   <p>Aktivierungsstatus jedes Gelenks</p><p>(On/Off)</p>  |  Off |
| tolerance |   <p>Winkelgrenzwert für jedes Gelenk</p><p>(0.0 ~ 3.0 (deg))</p>  |  0.1 |

{% hint style="warning" %}
*\[Achtung]**: Wenn die Stoppüberwachungsparameter verletzt werden, überprüfen Sie vor dem Neustart unbedingt, ob die Bewegung des Roboters normal ist.
{% endhint %}