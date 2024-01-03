# 4.1.2 Setting of tool data

The safety functions monitor the entire robot system including the tool attached to the robot’s tool flange. Therefore, the smaller the difference between the tool data and its actual value, the more accurately the safety functions will work. Set the length and angle of the tool based on the flange coordinate system and input the information on the weight, center of gravity, and inertia of the tool in the applicable units.

1. Set the operating mode to the manual mode.
2. Disconnect the power of the motor by pressing the emergency stop button.
3. Select the **\[Configure]** > **\[3: Robot parameter > 1: Tool data]** menu.
4. Check the data of each axis, set the weight, center of gravity, and inertia of the tool, and save the values by clicking the **\[OK]** button.

![](../../_assets/image20.jpeg)

* To easily create new tool data from scratch utilizing the current program, click the \[Auto calibration] button.
* To correct the tool angle, click the \[Angle calibration] button.
* To add a new user coordinate system or delete one, use the \[+] or \[-] buttons, respectively.
* To view and edit the detailed information of tool data, select a tool data name to be viewed and edited.
* To copy the information on tool data and paste it to that of another, use the \[Copy page] and \[Paste page] buttons, respectively.

{% hint style="info" %}
* When there is no information on the weight and center of gravity of a tool, you can estimate the values using the load estimation function.
* For more details on tool data setting, see “[**Operation Manual for Hi6 Controllers.**](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/english-tp630/7-system/4-robot-parameter/1-tool-data/README)”
{% endhint %}
