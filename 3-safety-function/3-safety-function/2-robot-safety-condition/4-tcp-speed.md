# 3.3.2.4 TCP Speed Limit Setting

This function monitors the TCP speed relative to the robot coordinate system. If a monitoring violation occurs, a safety stop (Stop 0, Stop 1, or Stop 2) is immediately activated.

You can set the parameter values   in the `[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 4: TCP Speed]` menu.

<p align="center">
<img src="../../../_assets/3/tcp_speed.png"></img>
<em><p align="center">TCP speed parameter setting screen</p></em>
</p>


| **Parameter** |                                  **Description**                                  |  **Default Setting** |
| :------: | :----------------------------------------------------------------: | :---------: |
| Activation | <p>Whether the function is activated</p><p>(OFF / ON / Safety I/O)</p> | OFF |
| Stop function | <p>Stop method in case of function violation</p><p>(Stop 0 / Stop 1 / Stop 2 / No stop)</p> | Stop 1 |
| Motion tuning | <p>Tuning to a motion that does not exceed the TCP speed limit</p><p>(Enable / Disable)</p> | Disable |
| <p>Limit</p><p>[mm/s]</p> | <p>TCP speed limit value</p><p>(1 ~ 50000)</p> | 50000 |

{% hint style="warning" %}
<strong>[Caution]</strong>: When setting the speed monitoring function, be sure to consider the stopping reaction time and cover the cover to prevent collisions and injuries.
{% endhint %}

{% hint style="warning" %}
<strong>[Attention]</strong> : Lors du réglage de la fonction de surveillance de la vitesse, veillez à tenir compte du temps de réaction à l'arrêt et à couvrir le carter de protection afin d'éviter les collisions et les blessures.
{% endhint %}

 