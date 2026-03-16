# 3.3.1.1 General

Set the thresholds for essential functions (manual mode speed monitoring, stop time, and stop distance monitoring) required for robot operation. Additionally, configure whether the robot monitoring and area monitoring functions are fully enabled. Even if the robot monitoring and area monitoring functions are enabled, if the safety function is disabled, the monitoring function will not operate. If a monitoring violation occurs, the configured safety stop (Stop 0, Stop 1) will be immediately activated.


You can set parameter values in the `[System > 10: Safety System > 1: General setup > 1: General]` menu.

<p align="center">
<img src="../../../_assets/3/general_param.png"></img>
<em><p align="center">General parameter setting screen</p></em>
</p>


|  **Parameter** |                       **Description**                       |  **Default setting**  |
| :-------: | :------------------------------------------------: | :-------------: |
| Safety function | <p>Whether robot monitoring and area monitoring functions are enabled</p><p>(Enable / Disable)</p> | Disable |
| Use T/P | <p>Enables or disables the use of the TP</p><p>(Enable / Disable)</p> | Disable |
| <p>Manual mode speed</p><p>[mm/s]</p> | <p>Whether the function is enabled</p><p>(10 ~ 250)</p> | 250 |
| <p>Stop time</p><p>[ms]</p> | <p>Stop method when the function is violated</p><p>(100 ~ 2000)</p> | 2000 |
| - Motion Tuning | <p>Tuning to a motion that satisfies the stopping time limit</p><p>(Enable / Disable)</p> | Disable |
| <p>Stopping Distance</p><p>[mm]</p> | <p>Whether each joint is activated</p><p>(50 ~ 2000)</p> | 2000 |
| - Motion Tuning | <p>Tuning to a motion that satisfies the stopping distance limit</p><p>(Enable / Disable)</p> | Disable |

{% hint style="warning" %}
<strong>[Caution]</strong>: Even if the safety function is set to disabled, the functions that are essential for robot use (manual mode speed, stop time, stop distance monitoring) are not disabled.
{% endhint %}

{% hint style="warning" %}
<strong>[Caution]</strong>: The stop time and stop distance are the time and distance until the robot actually stops when stop1 is executed, and if the set value is exceeded, stop0 is activated immediately.
{% endhint %}
 