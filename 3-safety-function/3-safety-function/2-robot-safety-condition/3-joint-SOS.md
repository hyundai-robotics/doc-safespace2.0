# 3.3.2.3 Joint Stop Monitoring

Stop monitoring monitors each axis for abnormal movement during robot stop operations. If a set limit is violated, a safety stop (Stop 0) is immediately activated.

Parameter values   can be set in the **\[System > 8: Safety System > 1: Parameter Settings > 1: Robot Limits > 3: Joint Stop]** menu.

<p align="center">
<img src="../../../_assets/3/joint_sos_param.PNG"></img>
<em><p align="center">Stop Monitoring Parameter Setting Screen</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Whether the function is activated</p><p>(Invalid / Valid / Safe I/O)</p> | Invalid |
| Joint Activation | <p>Whether each joint is activated</p><p>(Active / Disabled)</p> | Disabled |
| <p>Allowable Range</p><p>[deg]</p> | <p>Angle Limit Value for Each Joint</p><p>(0.0 ~ 3.0)</p> | 0.001 |

{% hint style="warning" %}
**\[Caution]**: If the stop monitoring parameters are violated, be sure to check that the robot's movement is normal before restarting.
{% endhint %}