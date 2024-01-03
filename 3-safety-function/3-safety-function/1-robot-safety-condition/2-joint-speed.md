# 3.3.1.2 Joint speed monitoring

These parameters are the limit values for monitoring the safety functions relating to the speed in which the robot’s joints move. If a monitoring violation occurs, safety stops (Stop0, Stop1, and Stop2) will be actuated immediately.

![An example of joint speed setting](../../../_assets/joint_speed.png)

You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction > Joint speed]** menu.

![Window for setting joint speed parameters](../../../_assets/joint_speed_param.PNG)

|  **Parameter** |                       **Description**                       |  **Default setting value**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Activation of function</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stop method</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Joint OnOff |   <p>Activation of each joint</p><p>(On/Off)</p>  |  Off |
| speed |   <p>The speed limit value of a joint</p><p>(0 ~ 5000 (mm/s))</p>  |  5000.0 |

{% hint style="warning" %}
**\[Caution]**: The safety function is monitored based on the set parameters. In configuring a limit, you must consider the stop reaction time and stopping distance. Before running the robot, verification must be performed.
{% endhint %}
 
