# 3.3.2.1 Safety space

The safety space is a working space or a protected space in which the range of the tool or the robot link is monitored. The working space is a limited space where the monitoring target can move freely but cannot exceed. In contrast, the protected space is a limited space in which the monitoring target cannot move when it intrudes into the space. If the monitoring target moves and exceeds the limit value of a safety condition, a functional safety stop(Stop0, Stop1, Stop2) will be actuated.

![Working space](<../../../_assets/safety_layout/cell_working.PNG>)

![Protected space](<../../../_assets/safety_layout/cell_protected.PNG>)

The safety space constructs the space by setting the position and height of each vertex based on the robot coordinate system. A maximum of 10 vertices can be added. The safety space is activated by parameter settings or safety input signals.

The safety space can be set from each tab of the **\[System > 4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Layout restriction > Cell area]** menu.


*   **General** 

![](../../../_assets/safety_layout/cell_general.PNG)

|  **Parameter** |                       **Description**                       |  **Default setting value**  |
| :-------: | :------------------------------------------------: | :----------: |
| Activation | <p>Activation of function</p><p>(Off/On/Safety Input)</p> |   Off  |
| Stop function |   <p>Stop method</p><p>(Stop0, Stop1, Stop2, Non-stop)</p>  | Stop 1 |
| Type |  <p>Type of space</p><p>(working space/protected space)</p>  | working space |


*   **Target** 

![](../../../_assets/safety_layout/cell_target.PNG)

|  **Parameter** |                       **Description**                       |  **Default setting value**  |
| :-------: | :------------------------------------------------: | :----------: |
| Tool | <p>Monitoring tool model</p><p>(Off/On/Safety Input)</p> |   Off  |
| Lower arm |   <p>Monitoring 2nd axis</p><p>(Off/On)</p>  | Off |
| Upper arm |  <p>Monitoring 3rd axis</p><p>(Off/On)</p>  | Off |


*   **Area** 

![](../../../_assets/safety_layout/cell_working.PNG)

|  **Parameter** |                       **Description**                       |  **Default setting value**  |
| :-------: | :------------------------------------------------: | :----------: |
| Z min/max | <p>Height of space based on robot coordination</p><p>(-5000.0 ~ 5000.0 mm)</p> |   0  |
| Vertex OnnOff |   <p>Activation of vertex</p><p>(Off/On)</p>  | Off |
| X |  <p>Vertex posion of X-direction based on robot coordination</p><p>(-5000.0 ~ 5000.0 mm)</p>  | 0 |
| Y |  <p>Vertex posion of Y-direction based on robot coordination</p><p>(-5000.0 ~ 5000.0 mm)</p>  | 0 |








{% hint style="warning" %}
**\[Caution]**: The safety function is monitored based on the set parameters. In configuring a limit, you must consider the stop reaction time and stopping distance. Before running the robot, verification must be performed.
{% endhint %}