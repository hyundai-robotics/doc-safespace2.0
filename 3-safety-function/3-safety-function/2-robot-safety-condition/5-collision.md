# 3.3.2.5 Collision Detection

When the external force applied to the robot exceeds the allowable value, it is recognized as a collision. You can adjust the sensitivity of each axis, and the higher the sensitivity, the more even a small external force is recognized as a collision. When the monitoring is violated, a safety stop (Stop 0, Stop 1, and Stop 2) is immediately activated.

`[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 5: Collision detection]` menu allows you to set the parameter values.

<p align="center">
<img src="../../../_assets/3/collision.png"></img>
<em><p align="center">Collision detection parameter setting screen</p></em>
</p>

| **Parameter** |                                  **Description**                                  |  **Default Setting** |
| :------: | :----------------------------------------------------------------: | :---------: |
| Activation | <p>Function activation status</p><p>(OFF/ON/Safety Input)</p> |   OFF  |
| Stop function |   <p>Stop method when the function is violated</p><p>(Stop 0, Stop 1, Stop 2, Non-stop)</p>  | Stop 1 |
| Joint ON/OFF |   <p>Activation status of each joint</p><p>(ON/OFF)</p>  |  OFF |
| Sensitivity |   <p>Detection sensitivity for each joint</p><p>(0 ~ 200(%))</p>  |  100 |

{% hint style="warning" %}
<strong>[Caution]</strong> Since the robot's impact force can increase in proportion to kinetic energy when the speed is high and the payload is large, considerable impact may occur if the robot collides with an external object. In the collaborative space, operate while maintaining the safe speed and payload.
<strong>[Caution]</strong> False detection may occur if the tool information and additional weight are set differently from actual values. Check each information before using the collision detection function.
{% endhint %}
