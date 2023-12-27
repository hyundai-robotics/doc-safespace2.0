# 6.1	Recovery in case of robot position violations

Robot position violations are situations in which the robot’s position exceeds a safety space, and these include TCP position, TCP orientation, and joint monitoring violations. When a robot position violation occurs, you can only clear the error by moving the robot’s physical position.

1.  Change the mode switch to manual mode.


2.  Turn on the motor by using the enabling switch on the teach pendant.


3.  Use the teaching device to move the robot back to a safety space.


4.  On the safety condition monitoring window, check if the status of each space is displayed as **SAFE**.


{% hint style="warning" %}
**\[Caution]**: After clearing the violation, recheck the safety layout setting and the teaching position of the operating program.
{% endhint %}
