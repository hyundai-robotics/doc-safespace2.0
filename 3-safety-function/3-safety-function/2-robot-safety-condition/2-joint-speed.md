# 3.3.2.2 Joint Speed Limit

The Joint Speed Setting parameter is a limit value for monitoring the robot's joint speed. If the limit value is violated, the specified safety stop (Stop 0, Stop 1, or Stop 2) is immediately activated.

<p align="center">
<img src="../../../_assets/joint_speed.PNG"></img>
<em><p align="center">Joint speed setting example</p></em>
</p>

You can set parameter values   in the `[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 2: Joint speed]` menu.

<p align="center">
<img src="../../../_assets/3/joint_speed_set.png"></img>
<em><p align="center">Joint speed setting parameter setting screen</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Whether the function is activated</p><p>(OFF / ON / Safety I/O)</p> | OFF |
| Stop function | <p>Stop method when the function is violated</p><p>(Stop 0 / Stop 1 / Stop 2 / No stop)</p> | Stop 1 |
| Motion Tuning | <p>Tuning to a motion that does not exceed the joint's speed limit</p><p>(Active / Disable)</p> | Disable |
| Joint ON/OFF | <p>Whether each joint is activated</p><p>(ON / OFF)</p> | OFF |
| <p>Speed</p><p>[mm/s]</p> | <p>Speed limit for each joint</p><p>(10 ~ 10000)</p> | 1000.0 |

{% hint style="warning" %}
<strong>[Caution]</strong>: When setting the speed monitoring function, be sure to consider the stopping reaction time and cover the cover to prevent collisions and injuries.
{% endhint %}
 
{% hint style="warning" %}
<strong>[Attention]</strong> : Lors du réglage de la fonction de surveillance de la vitesse, veillez à tenir compte du temps de réaction à l'arrêt et à couvrir le carter de protection afin d'éviter les collisions et les blessures.
{% endhint %}
