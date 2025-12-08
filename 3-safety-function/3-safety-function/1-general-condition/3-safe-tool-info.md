# 3.3.1.3 Safety Tool Information

Safety tool information is used by the safety board to calculate the robot's speed and position. You must enter the tool information attached to the actual robot. The tool information must be identical to the tool number used for robot control (**\[System > 3: Robot Parameters > 1: Tool Data]**).


You can set safety tool information in the **\[System > 8: Safety System > 1: Basic Settings > 3: Safety Tool Information]** menu, and you can load tool information used for robot control by clicking “Load Tool Data” at the bottom of the menu.

<p align="center">
<img src="../../../_assets/3/tool_info_param.png"></img>
<em><p align="center">안전 툴 정보 설정 화면</p></em>
</p>


|  **Parameter** |                       **Description**                       |  **Default value**  |
| :-------: | :------------------------------------------------: | :-------------: |
| <p>Weight</p><p>[kg]</p> | <p>Weight of the tool</p><p>(0.0 ~ 1000.0)</p> | 0.0 |
| <p>Length</p><p>[mm]</p> | <p>Length of the tool</p><p>(-3000.0 ~ 3000.0)</p> | 0.0 |
| <p>Center</p><p>[mm]</p> | <p>Location of the center of gravity of the tool relative to the center of the flange</p><p>(-3000.0 ~ 3000.0)</p> | 0.0 |
| <p>Inertia</p><p>[㎏·㎡]</p> | <p>Moment of inertia of the tool with respect to the tool coordinates</p><p>(0.0 ~ 2000.000)</p> | 0.0 |
| Load Tool Data | A function to load tool information used for robot control according to the tool number | - |
| Copy | A function to copy the values ​​entered on the corresponding page | - |
| Paste | A function to paste the values ​​of the copied page onto the corresponding page | - |

{% hint style="warning" %}
**\[Caution]**: If the safety tool information does not match the tool information used for robot control, a warning/error will occur and the robot will not operate. Be sure to match the actual tool information with the safety tool information before operating the robot.
{% endhint %}
 
{% hint style="warning" %}
**\[Caution]**: Safety tool numbers 0 to 15 are supported. If your system uses tool information 16 to 31, match safety tool number 0 with the tool information.
{% endhint %}
 