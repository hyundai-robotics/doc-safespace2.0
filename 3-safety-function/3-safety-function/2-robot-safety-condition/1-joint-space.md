# 3.3.2.1 Joint Angle Limit Setting

The Joint Area Setting parameter is a limit value for monitoring safety functions in the robot's joint space. If the monitoring is violated, the specified safety stop (Stop 0, Stop 1, or Stop 2) is immediately activated.

<p align="center">
<img src="../../../_assets/joint_space.PNG"></img>
<em><p align="center">Joint area setting example (S-axis)</p></em>
</p>

You can set parameter values   in the `[System > 8: Safety System > 2: Parameter Settings > 1: Robot Limits > 1: Joint Area]` menu.

<p align="center">
<img src="../../../_assets/3/joint_space.png"></img>
<em><p align="center">Joint area parameter setting screen</p></em>
</p>


|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Type | <p>Safety Area Type</p><p>(Work Area / Protection Area)</p> | Work Area |
| Activation | <p>Whether the function is activated</p><p>(Invalid / Valid / Safe I/O)</p> | Invalid |
| Stop Method | <p>Stop method in case of function violation</p><p>(Stop 0 / Stop 1 / Stop 2 / No Stop)</p> | Stop 1 |
| Joint Activation | <p>Whether each joint is activated</p><p>(Active / Inactive)</p> | Inactive |
| <p>Minimum</p><p>[deg]</p> | <p>Angle limit value for each joint</p><p>(-360.0 ~ 360.0)</p> | -360.0 |
| <p>Maximum</p><p>[deg]</p> | <p>Angle limits for each joint</p><p>(-360.0 ~ 360.0)</p> | 360.0 |

{% hint style="warning" %}
*\[Caution]**: The safety function monitors based on the set area. The set area should be configured considering the stop distance, and verification must be performed before operation.
{% endhint %}
 