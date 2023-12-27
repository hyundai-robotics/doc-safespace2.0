# 1.6.2 SOS monitoring

SOS monitoring is a function that monitors for abnormal movement of each axis during robot stop operation. If a monitoring violation occurs, Stop0 will be actuated immediately.


You can set the parameter values in the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction > Joint SOS]** menu.

![Window for setting joint SOS parameters](<../../../_assets/joint_sos_param.png>)

|  **Parameter** |                       **Description**                       |  **Default setting value**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Activation of function</p><p>(Off/On/Safety Input)</p> |   Off  |
| Joint OnOff |   <p>Activation of each joint</p><p>(On/Off)</p>  |  Off |
| tolerance |   <p>The angle limit value of a joint</p><p>(0.0 ~ 3.0 (deg))</p>  |  0.1 |

{% hint style="warning" %}
**\[Caution]**: Make sure that the robot moves normally before restarting operation if SOS monitoirng is violated.  
{% endhint %}