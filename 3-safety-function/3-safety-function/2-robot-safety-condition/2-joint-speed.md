# 3.3.2.2 Joint Speed Limit

The Joint Speed ​​Setting parameter is a limit value for monitoring the robot's joint speed. If the limit value is violated, the specified safety stop (Stop 0, Stop 1, or Stop 2) is immediately activated.

<p align="center">
<img src="../../../_assets/joint_speed.PNG"></img>
<em><p align="center">Joint speed setting example</p></em>
</p>

You can set parameter values ​​in the **\[System > 8: Safety System > 2: Parameter Settings > 1: Robot Limits > 2: Joint Speed]** menu.

<p align="center">
<img src="../../../_assets/3/joint_speed_param.PNG"></img>
<em><p align="center">Joint speed setting parameter setting screen</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activate | <p>Whether the function is activated</p><p>(Invalid / Valid / Safe I/O)</p> | Invalid |
| Stop method | <p>Stop method when the function is violated</p><p>(Stop 0 / Stop 1 / Stop 2 / No stop)</p> | Stop 1 |
| Motion Tuning | <p>Tuning to a motion that does not exceed the joint's speed limit</p><p>(Active / Disable)</p> | Disable |
| Joint Activation | <p>Whether each joint is activated</p><p>(Active / Disabled)</p> | Disabled |
| Type | <p>Type of operation for each joint</p><p>(Rotational / Linear)</p> | Rotation |
| <p>Speed</p><p>[mm/s]</p> | <p>Speed ​​limit for each joint</p><p>(0 ~ 10000)</p> | 1000.0 |

{% hint style="warning" %}
**\[Caution]**: When setting the speed monitoring function, be sure to consider the stopping reaction time and cover the cover to prevent collisions and injuries.
{% endhint %}
 
