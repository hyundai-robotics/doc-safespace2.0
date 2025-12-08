# 6.4 	Recovery from Safe Operating Stop (SOS) Violation

Safe Operating Stop (SOS) violation occurs when movement is detected while the robot motor is on and in a stopped state. In case of safe operating stop violation, the robot detects momentary movement and generates an error, so the error can be cleared without moving the robot's position.

1. Change the mode switch to manual to enter manual mode.


2. Remove external factors that apply force to the robot.


3. In the safety status monitoring screen, verify that the status of each area is displayed as **SAFE**.


{% hint style="warning" %}
**[Caution]**

* After clearing the error, check the safe operating stop monitoring parameters.
* Turn on the motor in auto mode and check whether the error recurs.
* If the same error occurs again, inspect the motor and reducer of the corresponding axis.
{% endhint %}
