# 3.3.1 Robot monitoring functions

The robot safety parameters consist of limits to monitor the safety function and stopping methods.

Each safety function can be utilized by storing various sets of activation conditions, limit values and methods of stopping in case of violation.  

You can set parameter values in the following menu.

**\[System]** button > **\[4: Application parameter > 18: SafeSpace2.0 > Parameter setup > Robot restriction]** 
****


The following safety parameters can be set in the robot monitoring menu.

* **Joint position**: This limits the robot’s joint positions so that its axes can move only within the specified ranges.
* **Joint speed**: This limits the robot’s momentum so that its axes cannot move beyond the specified speeds.
* **SOS**: This monitors the robot's stationary state by checking for abnormal movement on each axis after performing stationary 2
* **TCP speed**: This limits the robot's TCP speed so that axes cannot move beyond the specified speeds.
* **Re plan**: This contorls the speed of robot according to external input signal to perform [3.2.2 Speed and separation monitoring](../../2-collaborative-operation-mode/2-speed-separation-monitoring.md) of collaborative operation mode.
* **Power, collision detection**: This limits the force and pressure in case of a collision between the robot and the operator.
* **Momentum**: This limits the energy and impact load in case of a collision between the robot and the operator.


{% hint style="warning" %}
**\[Caution]** : To ensure the safety of personnel and equipment around the robot, operators and users should perform a risk assessment before configuring the robot’s safety function and set the following details according to the assessment result:

* Set passwords and the like so that the safety configuration cannot be modified by unauthorized persons.
* Set safety-related functions and interfaces.
* Check if the settings are correct before running the robot.
* Check if all the safety functions are configured and if the settings conform to the result of the risk assessment.
{% endhint %}

