# 9.1 - Moving Workpieces Using Workspace Switching

## 1) Overview

This chapter explains the task of using two workspaces where the robot picks up workpieces coming into the input space, processes them, and then transfers them to the output space. Through this, you can learn the basic usage of safety functions and safety communication.

If a person is in the input space, the robot can only operate within the output space, and if a person is in the output space, the robot can only operate within the input space. Additionally, if the robot goes beyond the allowed workspace (inside the fence), it immediately stops due to the safety function.

In this example, whether a person enters each workspace is detected through two safety mats installed on the floor, and the detected signal is transmitted to the robot controller through safety communication. This example explains how to switch the robot's safety monitoring area according to the transmitted safety signals.

<p align="center">
<img src="../_assets/app_note/two_space/overview1.png"></img>
<em><p align="center">[Workspace Diagram]</p></em>
</p>

<p align="center">
<img src="../_assets/app_note/two_space/safety_mat_diag.png"></img>
<em><p align="center">[Safety Mat Safety Communication Connection]</p></em>
</p>


***[Overall Setup Sequence]***

1. Robot link settings
2. Tool settings
3. Safety I/O settings
4. Workspace settings

{% hint style="info" %}

Overall settings are done through HRSafeSpace2. All settings can also be done through the TP.

"[HRSafeSpace2](https://hrbook-hrc.web.app/#/view/doc-hrsafespace2/ko/README)"



{% endhint %}


### Step 1) Robot Link Settings

Select Layout->robot in HRSafeSpace2. <br>
Refer to the figure below and enter values for links 2 and 3. <br>
When you click the `[Save]` button, you can check changes in capsule size and position in the preview screen.

<p align="center">
<img src="../_assets/app_note/two_space/robot.png"></img>
<em><p align="center">Robot link settings screen</p></em>
</p>

<p align="center">
<img src="../_assets/app_note/two_space/robot_capsule.png"></img>
<em><p align="center">Robot link settings preview</p></em>
</p>

### Step 2) Tool Settings

Select Layout->tools->tool0 in HRSafeSpace2. <br>
The shape of each tool number can be configured by combining up to 10 models. Refer to the figure below and enter the shape of Model 0. <br>
When you click the `[Save]` button, you can check changes in capsule size and position in the preview screen.

<p align="center">
<img src="../_assets/app_note/two_space/tool_capsule.png"></img>
<em><p align="center">Tool settings screen</p></em>
</p>

<p align="center">
<img src="../_assets/app_note/two_space/tool_capsule_preview.png"></img>
<em><p align="center">Tool settings preview</p></em>
</p>

### Step 3) Safety I/O Settings
Select I/O->I/O allocation in HRSafeSpace2. <br>
To activate space1 and space2 through signals input via safety communication, refer to the screen below and configure the Safety comm.input and Safety comm.output settings.


<p align="center">
<img src="../_assets/app_note/two_space/safe_comm_in.png"></img>
<em><p align="center">Safety signal assignment (safety communication input)</p></em>
</p>

<p align="center">
<img src="../_assets/app_note/two_space/safe_comm_out.png"></img>
<em><p align="center">Safety signal assignment (safety communication output)</p></em>
</p>

input bit 0 (exit-side safety mat) : space 1 (input space) activation (0: activated, 1: deactivated)<br>
input bit 1 (entrance-side safety mat) : space 2 (output space) activation (0: activated, 1: deactivated)<br>

output bit 0 : space 1 (input space) (0: area violation, 1: no area violation)<br>
output bit 1 : space 2 (output space) (0: area violation, 1: no area violation)<br>

If a person is on the exit-side safety mat, the input space is set as the workspace. <br>
If a person is on the entrance-side safety mat, the output space is set as the workspace.

<p align="center">
<img src="../_assets/app_note/two_space/safe_mat_bit.png"></img>
<em><p align="center">Safety signal assignment (mat)</p></em>
</p>


- Through the panel selection window, you can check the **safety communication input settings and status**.
<p align="center">
<img src="../_assets/app_note/two_space/widget_in.png"></img>
<em><p align="center">Safety communication input monitoring</p></em>
</p>

- Through the panel selection window, you can check the **safety communication output settings and status**.
<p align="center">
<img src="../_assets/app_note/two_space/widget_in.png"></img>
<em><p align="center">Safety communication output monitoring</p></em>
</p>

### Step 4) Workspace Settings

<p align="center">
<img src="../_assets/app_note/two_space/space_all.png"></img>
<em><p align="center">Space overall preview</p></em>
</p>

4.1) Fence Area Settings (Space 0)

Select Layout->spaces->space 0 in HRSafeSpace2.<br>
Set Space 0 as the internal space of the fence. Set it so that the robot body or tool can stop immediately before exiting this space.

<p align="center">
<img src="../_assets/app_note/two_space/space_0.png"></img>
<em><p align="center">Space 0 preview</p></em>
</p>


[General Tab Settings]

|  **Function** |     **Setting Value**   |   **Description**   |
| :-------: | :---------------: | :---------------: |
| Activation | Always ON | Always remains in an activated state |
| Stop Function | Stop 0 | Immediately stops and motor off when target exceeds the set range |
| Type | Workspace | Set as workspace |

<br>

<p align="center">
<img src="../_assets/app_note/two_space/space0_config_0.png"></img>
<em><p align="center">Space 0 general settings</p></em>
</p>

[Target Settings]

Set the space monitoring target to **Tool + Lower Arm + Upper Arm**.

<p align="center">
<img src="../_assets/app_note/two_space/space0_config_1.png"></img>
<em><p align="center">Space 0 target settings</p></em>
</p>

[Origin Settings] <br>
Do not change.

<p align="center">
<img src="../_assets/app_note/two_space/space0_config_2.png"></img>
<em><p align="center">Space 0 origin settings</p></em>
</p>

[Area Setting Method]

There are two methods for setting the area. <br>
① Enter coordinates directly <br>
② Press the input start button to click X, Y coordinates directly on the HRSpace screen, then set the z min & max values

Refer to the figure below to set the working area.

<p align="center">
<img src="../_assets/app_note/two_space/space0_config_3.png"></img>
<em><p align="center">Space 0 area settings</p></em>
</p>


4.2) Input Space Settings (Space 1)

Select Layout->spaces->space 1 in HRSafeSpace2.<br>
Space 1 sets the right input space in the diagram. When a person is on the left safety mat, the right input space is activated, and if the robot or tool exits this space, the robot decelerates and stops.

<p align="center">
<img src="../_assets/app_note/two_space/space_1.png"></img>
<em><p align="center">Space 1</p></em>
</p>

[General Tab Settings]

|  **Function** |     **Setting Value**   |   **Description**   |
| :-------: | :---------------: | :---------------: |
| Activation | Safety Signal | Activated when safety signal input becomes 0, deactivated when it becomes 1 |
| Stop Function | Stop 1 | Deceleration stop and motor off when target exits the workspace |
| Type | Workspace | Set as workspace |

<br>

<p align="center">
<img src="../_assets/app_note/two_space/space1_config_0.png"></img>
<em><p align="center">Space 1 general settings</p></em>
</p>

<p align="center">
<img src="../_assets/app_note/two_space/space1_config_1.png"></img>
<em><p align="center">Space 1 area settings</p></em>
</p>

4.3) Output Space Settings (Space 2)

Select Layout->spaces->space 2 in HRSafeSpace2.<br>
Space 2 sets the left output space in the diagram. When a person is on the right safety mat, the left output space is activated, and if the robot or tool exits this space, the robot decelerates and stops.

<p align="center">
<img src="../_assets/app_note/two_space/space_2.png"></img>
<em><p align="center">Space 2</p></em>
</p>

[General Tab Settings]

|  **Function** |     **Setting Value**   |   **Description**   |
| :-------: | :---------------: | :---------------: |
| Activation | Safety Signal | Activated when safety signal input becomes 0, deactivated when it becomes 1 |
| Stop Function | Stop 1 | Deceleration stop and motor off when target exits the workspace |
| Type | Workspace | Set as workspace |

<br>

<p align="center">
<img src="../_assets/app_note/two_space/space2_config_0.png"></img>
<em><p align="center">Space 2 general settings</p></em>
</p>

<p align="center">
<img src="../_assets/app_note/two_space/space2_config_1.png"></img>
<em><p align="center">Space 2 area settings</p></em>
</p>




