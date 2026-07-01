# 1.6 Response Time


* **Stop Response Time**

The response time to be taken from safety function violation to stop execution is 9.8ms. The response time should be reflected when calculating the robot's stop time and stop distance.


* **Safety Input Response Time (Safety Input)**

The maximum response time from the receipt of a stop signal through a safety input (**Default** or **Additional**) until the stop action is initiated is **11 ms**. This value does not include the input signal filter time, nor does it include the robot stopping time or stopping distance.

* **Safety Input Response Time (Safety Communication)**

The maximum response time from the receipt of a stop signal through safety communication until the stop action is initiated is **42 ms**. To obtain the total time required for the robot to come to a complete stop, the safety communication cycle time and the robot stopping time and stopping distance shall be taken into account.

* **Safety Output Response Time (Safety Communication)**

The maximum response time from the generation of a safety output by the safety application until the signal is transmitted through safety communication is **28 ms**. To calculate the total transmission time to the safety PLC, the safety communication cycle time shall be added.


