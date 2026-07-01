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

### 5. 비상정지 출력

| 단계 | 시험 절차                               | 예상 결과       |
| -- | ----------------------------------- | ----------- |
| 1  | 로봇 및 로봇제어기에 외관상의 손상이나 이상이 없는지 확인한다. | 이상 없음       |
| 2  | 모든 비상정지 버튼(TP, OP)이 복귀된 상태인지 확인한다.  | 비상정지 해제 상태  |
| 3  | 로봇제어기의 전원을 투입한다.                    | 제어기 기동      |
| 4  | 비상정지 출력이 활성화 상태인지 확인한다.             | 비상정지 출력 활성(출력 LED 점등 확인)  |
| 5  | TP의 비상정지 버튼을 누른다.                   | 비상정지 입력 발생  |
| 6  | 비상정지 출력이 비활성화 상태로 전환되는지 확인한다.       | 비상정지 출력 비활성(출력 LED 소등 확인) |

**합격 기준**

* 모든 비상정지 버튼이 복귀된 상태에서는 비상정지 출력이 활성화되어야 한다.
* TP 또는 OP의 비상정지 버튼을 누르면 비상정지 출력이 비활성화되어야 한다.
* 비상정지 상태가 유지되는 동안 비상정지 출력은 비활성 상태를 유지하여야 한다.

<br>

### 6. 기본 및 부가 안전 입력

**사전 조건 (Pre-condition)**

* 안전기능 할당 설정에서 시험 대상 입력 채널에 비상정지(E-Stop) 기능이 할당되어 있어야 한다.

| 단계 | 시험 절차                                         | 예상 결과                              |
| -- | --------------------------------------------- | ---------------------------------- |
| 1  | 로봇 및 로봇제어기에 외관상의 손상이나 이상이 없는지 확인한다.           | 이상 없음                              |
| 2  | 비상정지 버튼이 복귀된 상태인지 확인한다.                       | 비상정지 해제 상태                         |
| 3  | 로봇제어기의 전원을 투입한다.                              | 제어기 기동                             |
| 4  | 수동 모드에서 Enabling Switch를 조작하여 모터 ON 상태로 전환한다. | TP의 Motor ON 표시등 점등                |
| 5  | 시험 대상 안전 입력에 연결된 비상정지 버튼을 누른다.                | 비상정지 입력 발생                         |
| 6  | 모터 OFF 여부를 확인한다.                              | TP의 Motor ON 표시등이 점멸 또는 소등 상태로 변경됨 |

**합격 기준**

* 시험 대상 안전 입력에 비상정지 신호가 입력되면 모터 전원이 차단되어야 한다.
* TP의 Motor ON 표시등이 점멸 또는 소등 상태로 변경되어야 한다.
* 비상정지 상태에서는 로봇이 구동되지 않아야 한다.

<br>

### 7. 기본 및 부가 안전 출력

**사전 조건 (Pre-condition)**

* 안전기능 할당 설정에서 시험 대상 출력 채널에 비상정지 출력(E-Stop Output) 기능이 할당되어 있어야 한다.

| 단계 | 시험 절차                               | 예상 결과          |
| -- | ----------------------------------- | -------------- |
| 1  | 로봇 및 로봇제어기에 외관상의 손상이나 이상이 없는지 확인한다. | 이상 없음          |
| 2  | 모든 비상정지 버튼(TP, OP)이 복귀된 상태인지 확인한다.<br>(시계방향 회전 시켜 돌출 확인)   | 비상정지 해제 상태     |
| 3  | 로봇제어기의 전원을 투입한다.                    | 제어기 기동         |
| 4  | 시험 대상 안전 출력이 활성화 상태인지 확인한다.         | 비상정지 출력 활성 상태(출력 LED 점등 확인)  |
| 5  | TP의 비상정지 버튼을 누른다.                   | 비상정지 입력 발생     |
| 6  | 시험 대상 안전 출력이 비활성화 상태로 전환되는지 확인한다.   | 비상정지 출력 비활성 상태(출력 LED 소등 확인) |

**합격 기준**

* 모든 비상정지 버튼이 복귀된 상태에서는 시험 대상 안전 출력이 활성화 상태여야 한다.
* TP 또는 OP의 비상정지 버튼이 눌리면 시험 대상 안전 출력이 비활성화 상태로 전환되어야 한다.
* 비상정지 상태가 유지되는 동안 시험 대상 안전 출력은 비활성 상태를 유지하여야 한다.

<br>

### 8. 브레이크 테스트

| 단계 | 시험 절차                               | 예상 결과              |
| -- | ----------------------------------- | ------------------ |
| 1  | 로봇 및 로봇제어기에 외관상의 손상이나 이상이 없는지 확인한다. | 이상 없음              |
| 2  | 로봇제어기의 전원을 투입한다.                    | 제어기 기동             |
| 3  | 브레이크 테스트 Job 프로그램을 불러온다.            | 프로그램 정상 로드         |
| 4  | 조작 모드를 자동 모드로 변경한다.                 | 자동 모드 변경 확인        |
| 5  | 모터 ON 버튼을 입력한다.                     | 모터 ON 상태로 전환됨      |
| 6  | 시작 버튼을 입력한다.                        | 브레이크 테스트 프로그램이 실행됨 |
| 7  | 프로그램 종료 여부를 확인한다.                   | 브레이크 테스트 정상 종료     |

**합격 기준**

* 브레이크 테스트 프로그램 실행 중 모터 ON 상태가 유지되어야 한다.
* 브레이크 테스트 프로그램 실행 중 에러가 발생하지 않아야 한다.
* 브레이크 테스트 프로그램이 정상적으로 종료되어야 한다.
<br>"[로봇언어 HRScript](https://hrbook-hrc.web.app/#/view/doc-hrscript/ko/10-etc/1-proc/16-brake_check?cont_model=Hi7)" 참고




