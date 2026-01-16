# 3.3.2.5 Collision Detection

When the external force applied to the robot exceeds the allowable value, it is recognized as a collision. You can adjust the sensitivity of each axis, and the higher the sensitivity, the more even a small external force is recognized as a collision. When the monitoring is violated, a safety stop (Stop 0, Stop 1, and Stop 2) is immediately activated.

**\[System > 8: Safety System > 2: Parameter Settings > 1: Robot Limits > 5: Collision Detection]** menu allows you to set the parameter values.

<p align="center">
<img src="../../../_assets/col-det.png"></img>
<em><p align="center">Collision detection parameter setting screen</p></em>
</p>

| **Parameter** |                                  **Description**                                  |  **Default Setting** |
| :------: | ---------------------------------------------------------------- | :---------: |
| Activation | <p>Function activation status</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stop method when the function is violated</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Joint OnOff |   <p>Activation status of each joint</p><p>(On/Off)</p>  |  Off |
| Sensitivity |   <p>Detection sensitivity for each joint</p><p>(0 ~ 200 (%))</p>  |  100 |

{% hint style="warning" %}
* Since the robot's impact force can increase in proportion to kinetic energy when the speed is high and the payload is large, considerable impact may occur if the robot collides with an external object. In the collaborative space, operate while maintaining the safe speed and payload.
* False detection may occur if the tool information and additional weight are set differently from actual values. Check each information before using the collision detection function.
{% endhint %}
