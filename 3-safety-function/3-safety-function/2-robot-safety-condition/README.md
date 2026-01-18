# 3.3.2 Robot Monitoring Function

Robot safety parameters consist of limit values   and stop methods for monitoring safety functions.

Each safety function can be configured with various activation conditions, stop methods upon violation, and limit values.

To configure robot safety parameters, access the menu as follows:

* **\[System > 8: Safety System > 2: Parameter Settings > 1: Robot Limits]**
****

The following safety features can be configured in the Robot Limits menu:

* **Joint Area**: Limits the robot's range of motion for each axis to a specific range.
* **Joint Speed**: Limits the robot's motion by preventing it from exceeding the speed limit for each axis.
* **Joint Stop**: Monitors the robot's stopped state by checking for abnormal movement for each axis after performing Stop 2.
* **TCP Speed**: Limits the robot's speed to a specified speed based on TCP standards.
* **Collision Detection**: Limits the force in the event of a collision between the robot and the worker.
* **RePlan**: Adjusts the robot's speed according to external input to perform [3.2.2 Speed   and Position Monitoring](../../2-collaborative-operation-mode/2-speed-separation-monitoring.md) during collaborative operation mode.
* **Power Detection**: Limits the force in the event of a collision between the robot and the worker.
* **Momentum**: Limits the energy and impact load in the event of a collision between the robot and the worker.


{% hint style="warning" %}
**\[Caution]**: Operators and users must perform a risk assessment before configuring robot safety functions to ensure the safety of personnel and equipment surrounding the robot. Based on the assessment results, configure the following:

* Set a password, etc. to prevent unauthorized changes to the safety configuration.
* Configure safety-related functions and interfaces.
* Verify the accuracy of settings before operating the robot.
* Verify that all safety function configurations and settings comply with the risk assessment.
{% endhint %}

