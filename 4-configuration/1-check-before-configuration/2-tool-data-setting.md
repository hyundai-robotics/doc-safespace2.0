# 4.1.3 Tool Data Setting

Safety features monitor the entire robot system, including tools attached to the robot flange. Therefore, the smaller the error between the tool data and actual values, the more accurately the safety function operates. Set the tool length and angle based on the flange coordinate system and enter the tool weight, center of gravity, and inertia information in accordance with individual units.

1. Set the operation mode to manual mode.
2. Press the emergency stop switch to cut off the power to the motors.
3. Touch the `[Settings]` button > `[3: Robot Parameters > 1: Tool Data]` menu.
4. Check the data for each axis and set the tool weight, center of gravity, and inertia, then touch the `[OK]` button to save.

![](../../_assets/image20.jpeg)

* To create new tool data or easily create tool data using an existing program, touch the `[Auto Correction]`.
* To correct the tool angle, touch the `[Angle Correction]` button.
* To add or delete a new user coordinate system, use the `[+]`/`[-]` buttons.
* To check and edit detailed information of tool data, select the desired name from the tool data list.
* To copy tool data information and paste it to other tool data, use the `[Copy Page]`/`[Paste Page]` buttons.

{% hint style="info" %}
* If information about the tool's weight and center of gravity isn't available, you can use the load estimation function to estimate the values. 
* For detailed information on setting tool data, refer to the "[Hi7 Controller Operation Manual](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/ko-tp630/README?cont_model=Hi7)."
{% endhint %}
