# 3.3.4.1 Default Safety Input/Output Signals

Set the parameters for safety input/output signals.
There are 4 input signals and 1 output signal, all operating as dual signals.
You can set the parameter values in the `[System > 8: Safety System > 2: Parameter Settings > 3: Safety I/O > 2: Default I/O]` menu. 

## 1) Default Input Signal Settings

<p align="center">
<img src="../../../_assets/safety_io/def_input.png"></img>
<em><p align="center">Default Input/Output Settings Screen (Input)</p></em>
</p>

| Parameter <br>[Unit]          | Description                                                                                                                                       | Input Range       | Default |
|:------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|:--------------:|:------:|
| Pulse Test                 | Set whether to use the Pulse Test for each channel.                                                                                                     | Enable / Disable | Disable |
| Error Latch Time <br>[msec] | When an error occurs in a channel, even if the error is resolved, the system transitions from the Fail-Safe state to the current input state only after the **Error Latch Time** has elapsed.<br>Only values divisible by 10 can be entered. | 0 ~ 65530      | 1000   |
| Filter Time <br>[msec]      | The same signal should be input during the **Filter Time** set for each channel for it to be processed as a valid signal.<br>Only values divisible by 10 can be entered.                       | 0 ~ 500        | 100    |
| Discrete Time <br>[msec] | Basic input signals are processed as valid signals when two dual signals are identical.<br>An alarm is triggered if the two signals are different from each other for longer than the set **Discrete Time**.<br>Only values divisible by 10 can be entered. | 0 ~ 5000       | 1000   |

### Wiring Example)
![](../../../_assets/safety_io/CN_SI1.bmp)


## 2) Output Signal Settings

<p align="center">
<img src="../../../_assets/safety_io/def_output.png"></img>
<em><p align="center">Default I/O Settings Screen (Output)</p></em>
</p>

| Parameter <br>[Unit]          | Description                                                                                                                                       | Input Range       | Default |
|:------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|:--------------:|:------:|
| Pulse Test                 | Set whether to use the Pulse Test for each channel.                                                                                                     | Enable / Disable | Disable |
| Error Latch Time <br>[msec] | When an error occurs in a channel, even if the error is recovered, the system maintains the **Open (Fail-safe)** state during the **Error Latch Time**. Afterward, it  transitions to normal output.<br>Only values divisible by 5 can be entered. | 0 ~ 65530      | 1000   |

### Wiring Example)
![](../../../_assets/safety_io/CN_SO1.bmp)


