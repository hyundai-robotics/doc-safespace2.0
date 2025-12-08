# 3.3.2.4 TCP Speed ​​Limit Setting

This function monitors the TCP speed relative to the robot coordinate system. If a monitoring violation occurs, a safety stop (Stop 0, Stop 1, or Stop 2) is immediately activated.

You can set the parameter values ​​in the **\[System > 8: Safety System > 2: Parameter Settings > 1: Robot Limits > 4: TCP Speed]** menu.

<p align="center">
<img src="../../../_assets/tcp_speed_param.png"></img>
<em><p align="center">TCP speed parameter setting screen</p></em>
</p>


| **Parameter** |                                  **Description**                                  |  **Default Setting** |
| :------: | :----------------------------------------------------------------: | :---------: |
| Activate | <p>Whether the function is activated</p><p>(Invalid / Valid / Safe I/O)</p> | Invalid |
| Stop method | <p>Stop method in case of function violation</p><p>(Stop 0 / Stop 1 / Stop 2 / No stop)</p> | Stop 1 |
| Motion tuning | <p>Tuning to a motion that does not exceed the TCP speed limit</p><p>(Enable / Disable)</p> | Disable |
| Speed ​​readjustment | <p>Whether to use the speed adjustment function according to the input signal</p><p>(Enable / Disable)</p> | Disable |
| <p>Speed ​​limit value</p><p>[mm/s]</p> | <p>TCP speed limit value</p><p>(0 ~ 50000)</p> | 50000 |
| <p>Deceleration ratio</p><p>[%]</p> | <p>Deceleration ratio to use when readjusting speed</p><p>(0 ~ 100)</p> | 100 |
| <p>Delay time</p><p>[ms]</p> | <p>When changing speed through readjustment, monitor with the changed speed limit value after the delay time </p><p>(0 ~ 1000)</p> | 1000 |
| <p>Input signal</p><p>[Type, Number]</p> | <p>Input signal for speed readjustment</p><p>( [None, -] / [Safety input, 1~8] / [PROFIsafe, 1~64] )</p> | 0 |

{% hint style="warning" %}
**\[Caution]**: When setting the speed monitoring function, be sure to consider the stopping reaction time and cover the cover to prevent collisions and injuries.
{% endhint %}
 