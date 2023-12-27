# 6.3	Recovery in case of robot force violations

Robot force violations are situations in which external force is applied on the robot or in which the amount of the force used by the robot internally exceeds a safety limit, and these include collision detection, power, and momentum monitoring violations. You can clear errors depending on the causes of the violations.


1.  Remove the external factor that is applying force on the robot.


2.  Change the mode switch to manual mode.


3.  On the safety condition monitoring window, check if the status of each space is displayed as **SAFE**.


{% hint style="warning" %}
**[Caution]**

* After clearing the violation, recheck safety function setting, tool data, the teaching position and speed of the operating program.
{% endhint %}
