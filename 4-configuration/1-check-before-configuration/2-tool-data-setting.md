# 4.1.3 Tool Data Setting

Safety features monitor the entire robot system, including tools attached to the robot flange. Therefore, the smaller the error between the tool data and actual values, the more accurately the safety function operates. Set the tool length and angle based on the flange coordinate system and enter the tool weight, center of gravity, and inertia information in accordance with individual units.

1. Set the operation mode to manual mode.
2. Press the emergency stop switch to cut off the power to the motors.
3. Touch the `[Settings]` button > `[3: Robot Parameters > 1: Tool Data]` menu.
4. Check the data for each axis and set the tool weight, center of gravity, and inertia, then touch the `[OK]` button to save.
5. Apply the updated tool data to the safety tool data. For more information about safety tool data, see "[3.3.1.3 Safety Tool Information](../../3-safety-function/3-safety-function/1-general-condition/3-safe-tool-info.md)".

{% hint style="info" %}
* If information about the tool's weight and center of gravity isn't available, you can use the load estimation function to estimate the values. 
* For detailed information on setting tool data, refer to the "[7.4.1 Tool Data](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/en-tp630/7-system/4-robot-parameter/1-tool-data/README?cont_model=Hi7)" in the "[Hi7 Controller Operation Manual](https://hrbook-hrc.web.app/#/view/doc-hi6-operation/en-tp630/README?cont_model=Hi7)."
{% endhint %}
