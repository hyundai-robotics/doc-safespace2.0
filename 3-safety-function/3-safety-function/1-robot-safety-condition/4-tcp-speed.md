# 3.3.1.4 TCP speed monitoring

This function monitors the TCP speed based on the robot coordinate system. If a monitoring violation occurs, safety stops (Stop0, Stop1, and Stop2) will be actuated immediately.

You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction > TCP speed]** menu.

![Window for setting TCP speed parameters](../../../_assets/tcp_speed_param.PNG)

| **Parameter** | 　　　　　　　　　**Description**                                                  |  **Default setting value** |
| :------: | ---------------------------------------------------------------- | :---------: |
| Activation | <p>Activation of TCP speed monitoring function</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stop method</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Replan |   <p>Activation of RePlan function</p><p>(On/Off)</p>  |  Off |
| Limit |   <p>TCP speed limit</p><p>(0 ~ 50000 (mm/s))</p>  | 50000 |
| Rate |   <p>Deceleration ratio for Replan</p><p>(0 ~ 100 (%))</p>  | 0 |
| Delay time |   <p>Monitor changed speed limit after delay time due to RePlan</p><p>(0 ~ 1000(ms))</p>  | 0 |
| Input signal setting |   <p> Input signal assignment for replan</p><p>(0 ~ 16)</p>  |  0 |

{% hint style="warning" %}
**\[Caution]**: The safety function is monitored based on the set parameters. In configuring a limit, you must consider the stop reaction time and stopping distance. Before running the robot, verification must be performed.
{% endhint %}
 