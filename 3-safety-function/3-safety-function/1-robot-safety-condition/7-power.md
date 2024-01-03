# 3.3.1.7 Power monitoring

It is a function that monitors whether the robot's power exceeds the allowable value. If a monitoring violation occurs, safety stops (Stop0, Stop1, and Stop2) will be actuated immediately.

You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction > Power]** menu.

![Window for setting power monitoring parameters](../../../_assets/power.PNG)

| **Parameter** | 　　　　　　　　　**Description**                                                  |  **Default setting value** |
| :------: | ---------------------------------------------------------------- | :---------: |
| Activation | <p>Activation of function</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stop method</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Power |   <p>The power limit of robot</p><p>(80 ~ 1000 (W))</p>  | 1000 |

{% hint style="warning" %}
* Because the speed increases in proportion to kinetic energy and a high payload may increase the robot’s momentum, the collision of the robot with an external object may generate significant impact. In the collaborative operation space, operate the robot while maintaining a safe speed and payload.
* If the tool and additional load information are set differently from the actual one, error detection would be occured incorrectly. Please check the information before using the function.
{% endhint %}
