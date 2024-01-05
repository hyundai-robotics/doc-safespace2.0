# SW651\~SW664

| **Code** |                **Message**               |           **Cause**           | 　　　　**Solutions**                                                                                                                                     |
| :----: | :----------------------------------: | :------------------------: | ----------------------------------------------------------------------------------------------------------------------------------------------- |
|SW651|Robot safety stop violation|Robot motion has been detected in stop state.|<ul><li>Check the brake on each joint.</li></ul>|
|SW652|TCP position violation (Cell)|TCP position is out of the cell area.|<ul><li>Change the mode to manual.</li><li>Jog the robot to safety area.</li><li>Verify the job program.</li></ul>|
|SW653|Robot self collision detection|The collision detected between the robot moel and the tool model.|<ul><li>Change the mode to manual.</li><li>Jog the robot to prevent collsion.</li><li>Verify the job program.</li></ul>|
|SW654|TCP orientation violation ([deg])|TCP orientation exceeded the limits.|<ul><li>Change the mode to manual.</li><li>Jog the robot to safety area.</li><li>Verify the TCP orientation in job program.</li></ul>|
|SW655|TCP speed violation in manual mode([mm/s])|TCP speed exceeded the limits in manual mode.|<ul><li>Check the value set in the safety function menu.</li></ul>|
|SW656|Joint space violation([deg])|Joint position is out of the safe space.|<ul><li>Change the mode to manual.</li><li>Jog the robot to safety area.</li><li>Verify the job program.</li></ul>|
|SW657|Joint speed violation([deg/s])|Joint speed exceeded the limits.|<ul><li>Check the value set in the safety function menu.</li><li>Verify the joint speed in job program.</li></ul>|
|SW658|Robot power violation([N])|Robot power exceeded the limits.|<ul><li>Check the value set in the safety function menu.</li><li>Verify the joint speed and position in job program.</li></ul>|
|SW659|Robot momentum violation([kg m/s])|Robot momentum exceeded the limits.|<ul><li>Check the value set in the safety function menu.</li><li>Verify the TCP speed and position in job program.</li></ul>|
|SW660|Collision detection-safety([Axis])|If a collision occurrs, remove the cause of the collision.|<ul><li>Verify the sensitivity of collision detection.</li><li>Check the value set in the safety function menu.</li></ul>|
|SW661|TCP speed violation in reduced mode([mm/s])|TCP speed exceeded the limits in reduced mode|<ul><li>Check the value set in the safety function menu.</li><li>Verify the TCP speed in job program.</li></ul>|
|SW662|Stopping distance violation|Stopping distance exceeded the limits|<ul><li>Check the value set in the safety function menu.</li><li>Verify the robot's speed in job program.</li></ul>|
|SW663|Stopping time violation|Stopping time exceeded the limits.|<ul><li>Check the value set in the safety function menu.</li><li>Verify the robot's speed in job program.</li></ul>|
|SW664|TCP speed violation([mm/s])|TCP speed exceeded the limits.|<ul><li>Check the value set in the safety function menu.</li><li>Verify the TCP speed in job program.</li></ul>|