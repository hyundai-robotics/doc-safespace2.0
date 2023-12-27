# 6.2	Recovery in case of robot speed violations

Robot speed violations are situations in which the robot’s speed exceeds a safety limit, and these include TCP speed, joint speed, power, and momentum monitoring violations. Because the robot detects the instantaneous speed in the case of robot speed violations, you can clear the error without moving the robot’s position.

1.  Change the mode switch to manual mode.


2.  On the safety condition monitoring window, check if the status of each space is displayed as **SAFE**.


{% hint style="warning" %}
**[Caution]**

* After clearing the violation, make sure to recheck all speed-related safety parameters and the speed displayed on the operating program.
{% endhint %}
