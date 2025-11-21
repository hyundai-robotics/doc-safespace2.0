# 3.3.3.3 安全信号分配

安全信号分配的作用是，将外部信号（如安全输入输出、附加安全输入输出、安全通信输入输出等）与机器人控制器内部的各种逻辑信号或状态变量进行连接。

![!Additional Input Image](../../../_assets/safety_io/io_alloc.PNG)

### 添加安全信号分配
1) 在左侧I/O function list中选择所需功能（Function）
2) **2) 按下[PICK]按钮并选择索引（H/W通道或Bit编号）** 버튼을 누르고 인덱스(H/W 채널 또는 Bit 번호)를 선택
3) 根据I/O function list选择Subset可以选择详细功能编号

![!Additional Input Image](../../../_assets/safety_io/io_alloc2.PNG)

### 删除安全信号分配
1) 在屏幕右侧选择已设置的分配功能
2) 아래에 보이는 **2) 点击下方的[Discard]按钮** 버튼을 누름

---

### 安全信号的默认设定值

|  **|  通道 |     功能                       |** |     **|  通道 |     功能                       |**                       |
| :-------: | :------------------------------------------------: |
| 安全输入通道1 | 外部紧急停止输入（Emergency） |
| 安全输入通道2 | 安全防护栏普通输入（SGG） |
| 安全输入通道3 | 安全防护栏自动输入（SGA） |
| 安全输入通道4 | - |
| 安全输出通道1 | 紧急停止激活状态 |

### 安全信号的功能列表

|  **|  通道 |     功能                       |** |     **|  通道 |     功能                       |**                       |
| :-------: | :------------------------------------------------: |
| Emergency | 外部紧急停止输入 |
| SGG | 安全防护栏普通输入 |
| SGA | 安全防护栏自动输入 |
| Protective stop | - |
| Normal stop | - |
| Enable Switch | 外部使能开关 |
| Motor On | 外部电机开启 |
| Remote | 外部模式输入（远程） |
| Manual | 外部模式输入（手动） |
| Auto | 外部模式输入（自动） |
| Arm Limit | 机械臂限位输入 |
| Primary axis Limit | 主轴限位输入 |
| Additional axis Limit | 附加轴限位输入 |
| External axis Limit | 扩展轴限位输入 |
| Monitored standstill #1 ~ #8 | - |
| Joint speed set #1 ~ #8 | - |
| TCP speed set #1 ~ #16 | - |
| Joint angle #1 ~ #8 | - |
| TCP position(cell) #1 ~ #16 | - |
| TCP orientation #1 ~ #8 | - |
| Self collision | - |
| Power #1 ~ #16 | - |
| Momentum #1 ~ #16 | - |
| Collision detection #1 ~ #16 | - |
| Speed & separation #1 ~ #84 | - |
| Mastering test switch| - |