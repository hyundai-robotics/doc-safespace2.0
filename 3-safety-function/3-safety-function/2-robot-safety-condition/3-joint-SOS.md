# 3.3.2.3 Joint Stop Monitoring

Stop monitoring monitors each axis for abnormal movement during robot stop operations. If a set limit is violated, a safety stop (Stop 0) is immediately activated.

Parameter values   can be set in the `[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 3: Joint SOS]` menu.

<p align="center">
<img src="../../../_assets/3/joint_sos.png"></img>
<em><p align="center">Stop Monitoring Parameter Setting Screen</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Whether the function is activated</p><p>(OFF / ON / Safety I/O)</p> | OFF |
| Joint ON/OFF | <p>Whether each joint is activated</p><p>(ON / OFF)</p> | OFF |
| <p>Tolerance</p><p>[deg]</p> | <p>Angle Limit Value for Each Joint</p><p>(0.0 ~ 3.0)</p> | 0.100 |

{% hint style="warning" %}
<strong>[Caution]</strong>: If the stop monitoring parameters are violated, be sure to check that the robot's movement is normal before restarting.
{% endhint %}