# 3.3.1.9 Safety Stop

Set an adequate safety stop type for each safety stop function. The safety stop functions, which stop the robot under a safe condition in case of a safety violation, include the following three types. All types of safety stop functions meet the requirements of Clause 4.2.2.4 of IEC 61800-5-2.

* **Stop0**: The power of the motors of all the joint modules will disconnect immediately, and the motors will stop.
* **Stop1**: The power of the motors of all the joint modules will decelerate, and the motors will stop. Then, the power of the motors will be disconnected.
* **Stop2**: The motors of all the joint modules will decelerate, and the safe operating stop (SOS) function will take effect. The power supply status of all the motors will be retained.

The stop type due to a safety function violation is set in the parameter setting menu for each function.
The stop type settings for stops required by ISO 10218-1 are as follows.

You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction > Safety stop]** menu.

![](../../../_assets/safety_stop.PNG)

|  **Parameter** |                       **Description**                       |  **Default setting value**  |
| :-------: | :------------------------------------------------: | :----------: |
| EM stop |  <p>Emergency stop</p><p>(Stop 0, Stop 1)</p>  | Stop 0 |
| Protective stop | <p>Protective stop</p><p>(Stop 0, Stop 1, Stop 2)</p> |   Stop 0 |
| Normal stop |   <p>Normal stop</p><p>(Stop 0, Stop 1)</p>  | Stop 0 |
| Manual stop |   <p>Speed violation stop in manual mode</p><p>(Stop 0, Stop 1)</p>  |  Stop 0 |


{% hint style="warning" %}
**\[Caution]**: You should set an adequate stopping method for each function based on the result of the risk assessment.
{% endhint %}
