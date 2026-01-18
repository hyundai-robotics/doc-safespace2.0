# 3.3.2.9 Stop Settings

Set the appropriate safe stop type for each safety function. Safe stop functions stop the robot to a safe state when a safety violation occurs. There are three types: All types of safe stop functions comply with Requirement 4.2.2.4 of IEC 61800-5-2.

* **Stop 0**: Immediately remove power from all motors in the joint modules and stop.
* **Stop 1**: All motors in the joint modules decelerate and then stop. Power is then removed from the motors.
* **Stop 2**: All motors in the joint modules decelerate and SOS (Safe Operating Stop) is activated. Power is maintained to all motors.

The stop type due to a safety function violation is set in the function-specific parameter settings menu.
The stop type settings for the stops required by ISO 10218-1 are as follows:

Parameter values   can be set in the **\[System > 8: Safety System > 1: Basic Settings > 2: Stop Settings]** menu.

<p align="center">
<img src="../../../_assets/safety_stop_param.png"></img>
<em><p align="center">Stop setting screen</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Emergency Stop | <p>Select the stop type to apply during an emergency stop</p><p>(Stop 0, Stop 1)</p> | Stop 1 |
| Protective Stop | <p>Select the stop type to apply during a protective stop</p><p>(Stop 0, Stop 1, Stop 2)</p> | Stop 1 |
| Normal Stop | <p>Select the stop type to apply during a normal stop</p><p>(Stop 0, Stop 1)</p> | Stop 1 |
| Manual Mode Stop | <p>Stop when speeding in manual mode</p><p>(Stop 0, Stop 1)</p> | Stop 1 |


{% hint style="warning" %}
**\[Caution]**: You should establish an appropriate stopping method for each function through a risk assessment.
{% endhint %}
