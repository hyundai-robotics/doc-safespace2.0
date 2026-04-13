# 3.3.2.6 Re plan Setting

Re plan is a function that adjusts the robot's speed based on signals received from external safety sensors. The robot's operating speed is adjusted to the deceleration rate corresponding to the input signal, and the TCP speed is monitored at the corresponding speed after a delay time.

If the delay time is insufficient or the robot decelerates insufficiently, resulting in a violation of the TCP speed limit, a safety stop (Stop 0, Stop 1, Stop 2) is immediately activated.

You can set the parameter values   in the `[System > 10: Safety System > 2: Parameter setup > 1: Robot restriction > 6: Re plan]` menu.

<p align="center">
<img src="../../../_assets/3/replan_param.png"></img>
<em><p align="center">Re plan settings screen</p></em>
</p>

|  **Parameter** |                       **Description**                       |  **Default Setting**  |
| :-------: | :------------------------------------------------: | :----------: |
| Re plan | <p>Whether to use the speed control function according to the input signal</p><p>(Enable / Disable)</p> | Disable |
| <p>Delay time</p><p>[ms]</p> | <p>When changing the speed with Re plan, monitor the changed speed limit value after the delay time </p><p>(0 ~ 2000)</p> | 2000 |
| <p>Speed limit value</p><p>[mm/s]</p> | <p>TCP speed limit value after Re plan</p><p>(0 ~ 50000)</p> | 50000 |
| <p>Speed ratio</p><p>[%]</p> | <p>Deceleration ratio to use when Re plan</p><p>(0 ~ 100)</p> | 100 |
| <p>Input signal</p><p>[Type, Number]</p> | <p>Input signal for Re plan</p><p>( [None, -] / [default input, 3] / [additional input, 0~7] / [safety input, 0~63])</p> | 0 |

{% hint style="warning" %}
<strong>[Caution]</strong> When configuring speed limits, always consider stopping time and cover the robot to prevent collisions and injuries.
<strong>[Caution]</strong> High speeds and large payloads, in proportion to the robot's kinetic energy, can increase the robot's impact force. Therefore, a significant impact can occur if the robot collides with an external object. Maintain a safe speed and payload in collaborative spaces.
{% endhint %}
