# 4.2 Safety Function Test

When the robot system is installed and configured for the first time, or whenever robot components are replaced or optional devices are added or modified, the relevant safety functions shall be tested and validated in accordance with the procedures described below before the robot system is put into operation.


### 1. Emergency Stop

| Step | Test Procedure                                                                               | Expected Result                                      |
| ---- | -------------------------------------------------------------------------------------------- | ---------------------------------------------------- |
| 1    | Check that there is no visible damage or abnormality on the robot and the robot controller.  | No abnormalities are found.                          |
| 2    | Verify that the Emergency Stop button is released.<br>(Turn it clockwise until it pops out.) | Emergency Stop released.                             |
| 3    | Turn on the power to the robot controller.                                                   | The controller starts up.                            |
| 4    | In Manual mode, operate the Enabling Switch to change to the **Motor ON** state.             | The **Motor ON** indicator on the TP is illuminated. |
| 5    | Press the Emergency Stop button.                                                             | An Emergency Stop input is detected.                 |
| 6    | Verify that the system has changed to the **Motor OFF** state.                               | **Motor OFF** state.                                 |


**Acceptance Criteria**

* Pressing the Emergency Stop button shall cause the system to transition to the **Motor OFF** state.
* The **Motor ON** indicator on the TP shall blink or turn off.
* The robot shall not be operable while the Emergency Stop condition is active.


<br>

### 2. Safeguard General Signal (SGG)

| Step | Test Procedure                                                                              | Expected Result                                                |
| ---- | ------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| 1    | Check that there is no visible damage or abnormality on the robot and the robot controller. | No abnormalities are found.                                    |
| 2    | Verify that the safeguard signal is inactive. (Example: The safety fence door is closed.)   | Safeguard signal is in the normal state. (System Input screen) |
| 3    | Turn on the power to the robot controller.                                                  | The controller starts up.                                      |
| 4    | In Manual mode, operate the Enabling Switch to change to the **Motor ON** state.            | The **Motor ON** indicator on the TP is illuminated.           |
| 5    | Activate the safeguard signal. (Example: Open the safety fence door.)                       | Safeguard signal input is detected.                            |
| 6    | Verify that the system has changed to the **Motor OFF** state.                              | **Motor OFF** state.                                           |

**Acceptance Criteria**

* Activating the safeguard signal shall cause the system to transition to the **Motor OFF** state.
* The **Motor ON** indicator on the TP shall blink or turn off.
* The robot shall not be operable while the safeguard signal is active.


<br>

### 3. Safeguard Automatic Signal (SGA)

| Step | Test Procedure                                                                              | Expected Result                                                |
| ---- | ------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| 1    | Check that there is no visible damage or abnormality on the robot and the robot controller. | No abnormalities are found.                                    |
| 2    | Verify that the safeguard signal is inactive. (Example: The safety fence door is closed.)   | Safeguard signal is in the normal state. (System Input screen) |
| 3    | Turn on the power to the robot controller.                                                  | The controller starts up.                                      |
| 4    | In **Automatic** mode, change to the **Motor ON** state.                                    | The **Motor ON** indicator on the TP is illuminated.           |
| 5    | Open the safeguard. (Example: Open the safety fence door.)                                  | Safeguard signal input is detected.                            |
| 6    | Verify that the system has changed to the **Motor OFF** state.                              | The **Motor ON** indicator on the TP blinks or turns off.      |

**Acceptance Criteria**

* Activating the safeguard signal in **Automatic** mode shall cause the system to transition to the **Motor OFF** state.
* The **Motor ON** indicator on the TP shall blink or turn off.
* The robot shall not be operable while the safeguard signal is active.


<br>

### 4. Enabling Switch

| Step | Test Procedure                                                                                 | Expected Result                                           |
| ---- | ---------------------------------------------------------------------------------------------- | --------------------------------------------------------- |
| 1    | Check that there is no visible damage or abnormality on the robot and the robot controller.    | No abnormalities are found.                               |
| 2    | Turn on the power to the robot controller.                                                     | The controller starts up.                                 |
| 3    | In **Manual** mode, hold the **Enabling Switch** in the middle position (**Enable Position**). | Enabling state is active.                                 |
| 4    | Verify that the system is in the **Motor ON** state.                                           | The **Motor ON** indicator on the TP is illuminated.      |
| 5    | Release the **Enabling Switch**. <br> or  Squeeze the **Enabling Switch** fully.                   | Enabling is deactivated.                                  |
| 6    | Verify that the system has changed to the **Motor OFF** state.                                 | The **Motor ON** indicator on the TP blinks or turns off. |

**Acceptance Criteria**

* Releasing the **Enabling Switch** shall cause the system to transition to the **Motor OFF** state.
* The **Motor ON** indicator on the TP shall blink or turn off.
* The robot shall not be operable while the **Enabling Switch** is released.


<br>

### 5. Emergency Stop Output

| Step | Test Procedure                               | Expected Result       |
| -- | ----------------------------------- | ----------- |
| 1  | Check that there is no visible damage or abnormality on the robot and the robot controller. | No abnormalities are found       |
| 2  | Verify that all Emergency Stop buttons (TP, OP) are released.  | Emergency Stop released  |
| 3  | Turn on the power to the robot controller.                    | Controller starts up      |
| 4  | Verify that the Emergency Stop output is in the active state.             | Emergency Stop output active (output LED confirmed on)  |
| 5  | Press the Emergency Stop button on the TP.                   | An Emergency Stop input occurs  |
| 6  | Verify that the Emergency Stop output switches to the inactive state.       | Emergency Stop output inactive (output LED confirmed off) |

**Acceptance Criteria**

* While all Emergency Stop buttons remain in the released state, the Emergency Stop output shall be active.
* Pressing the Emergency Stop button on the TP or OP shall cause the Emergency Stop output to become inactive.
* The Emergency Stop output shall remain inactive for as long as the Emergency Stop condition is maintained.

<br>

### 6. Basic and Additional Safety Input

**Pre-condition**

* The Emergency Stop (E-Stop) function must be assigned to the input channel under test in the safety function assignment settings.

| Step | Test Procedure                                         | Expected Result                              |
| -- | --------------------------------------------- | ---------------------------------- |
| 1  | Check that there is no visible damage or abnormality on the robot and the robot controller.           | No abnormalities are found                              |
| 2  | Verify that the Emergency Stop button is in the released state.                       | Emergency Stop released                         |
| 3  | Turn on the power to the robot controller.                              | Controller starts up                             |
| 4  | In Manual mode, operate the Enabling Switch to switch to the Motor ON state. | The Motor ON indicator on the TP is illuminated                |
| 5  | Press the Emergency Stop button connected to the safety input under test.                | An Emergency Stop input occurs                         |
| 6  | Check whether the motor turns OFF.                              | The Motor ON indicator on the TP blinks or turns off |

**Acceptance Criteria**

* When an Emergency Stop signal is applied to the safety input under test, motor power shall be cut off.
* The Motor ON indicator on the TP shall blink or turn off.
* The robot shall not operate while in the Emergency Stop state.

<br>

### 7. Basic and Additional Safety Output

**Pre-condition**

* The Emergency Stop Output (E-Stop Output) function must be assigned to the output channel under test in the safety function assignment settings.

| Step | Test Procedure                               | Expected Result          |
| -- | ----------------------------------- | -------------- |
| 1  | Check that there is no visible damage or abnormality on the robot and the robot controller. | No abnormalities are found          |
| 2  | Verify that all Emergency Stop buttons (TP, OP) are in the released state.<br>(Turn clockwise to confirm they pop out.)   | Emergency Stop released     |
| 3  | Turn on the power to the robot controller.                    | Controller starts up         |
| 4  | Verify that the safety output under test is in the active state.         | Emergency Stop output active state (output LED confirmed on)  |
| 5  | Press the Emergency Stop button on the TP.                   | An Emergency Stop input occurs     |
| 6  | Verify that the safety output under test switches to the inactive state.   | Emergency Stop output inactive state (output LED confirmed off) |

**Acceptance Criteria**

* While all Emergency Stop buttons remain in the released state, the safety output under test shall be in the active state.
* When the Emergency Stop button on the TP or OP is pressed, the safety output under test shall switch to the inactive state.
* The safety output under test shall remain inactive for as long as the Emergency Stop state is maintained.

<br>

### 8. Brake Test

| Step | Test Procedure                               | Expected Result              |
| -- | ----------------------------------- | ------------------ |
| 1  | Check that there is no visible damage or abnormality on the robot and the robot controller. | No abnormalities are found              |
| 2  | Turn on the power to the robot controller.                    | Controller starts up             |
| 3  | Load the brake test job program.            | Program loads normally         |
| 4  | Change the operating mode to Automatic mode.                 | Automatic mode change confirmed        |
| 5  | Press the Motor ON button.                     | Switches to the Motor ON state      |
| 6  | Press the Start button.                        | The brake test program runs |
| 7  | Check whether the program has ended.                   | Brake test ends normally     |

**Acceptance Criteria**

* The Motor ON state must be maintained while the brake test program is running.
* No error shall occur while the brake test program is running.
* The brake test program must end normally.
<br>Refer to "[Robot Language HRScript](https://hrbook-hrc.web.app/#/view/doc-hrscript/ko/10-etc/1-proc/16-brake_check?cont_model=Hi7)."
