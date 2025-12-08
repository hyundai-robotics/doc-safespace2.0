# 3.3.4.3 安全信号分配

安全信号分配的作用是，将外部信号（如安全输入输出、附加安全输入输出、安全通信输入输出等）与机器人控制器内部的各种逻辑信（系统安全输入输出、安全应用程序的信号）进行连接。
**\[系统 > 8: 安全系统 > 2: 参数设置 > 3: 安全输入输出 > 1: 输入输出分配]** 菜单中，可以设置参数值。

![](../../../_assets/safety_io/SIO_Alloc_diagram1.bmp)

![](../../../_assets/safety_io/SIO_Alloc_diagram2.bmp)

-------------------------------------------------------------------------

### 添加安全信号分配
1) 在左侧输入输出功能列表中选择所需的功能（Function）
2) 按下 **[选择]** 按钮并选择索引（H/W通道或Bit编号）
3) 根据输入输出功能列表选择详细通道，可以选择详细功能编号

<p align="center">
<img src="../../../_assets/safety_io/io_alloc_param1.png"></img>
<em><p align="center">安全信号分配设置界面</p></em>
</p>

<p align="center">
<img src="../../../_assets/safety_io/io_alloc_param2.png"></img>
<em><p align="center">安全信号附加分配详细设置界面</p></em>
</p>


{% hint style="warning" %}
* 单个输入功能项目只能与一个输入通道连接。<br>
* “基本安全输入”、“附加安全输入”、“安全通信输入”不能重复分配。<br>
* 设置重复输入时将发生“E52030（x ch）安全输入分配重复”错误。

{% endhint %}

### 删除安全信号分配
1) 在屏幕右侧选择已设置的分配功能
2) 点击下方的**[废弃]**按钮

---

### 安全信号的默认设定值

|  **通道** |     **功能**                       |
| :-------: | :------------------------------------------------: |
| 安全输入通道1 | 外部紧急停止输入（Emergency） |
| 安全输入通道2 | 安全防护栏普通输入（SGG）| 
| 安全输入通道3 | 安全防护栏自动输入（SGA）|
| 安全输入通道4 | - |
| 安全输出通道1 | 紧急停止激活状态|

### 安全输入信号的功能列表

|  **通道** |     **功能**                       |       **说明**    |
| :-------: | :--------------------------: | :--------------------------------------------------: |
| Emergency | 外部紧急停止输入| OPEN : 紧急停止激活<br>CLOSE : 紧急停止解除 |
| SGG| 安全防护栏普通输入| OPEN : 防护栏打开（危险）<br>CLOSE : 防护栏关闭 （安全） |
| SGA | 安全防护栏自动输入| OPEN : 防护栏打开（危险） <br>CLOSE : 防护栏关闭 （安全） |
| Protective stop | 保护停止输入 | OPEN : 保护停止激活 <br>CLOSE : 保护停止解除 |
| Normal stop | 正常停止输入 | OPEN : 正常停止激活 <br>CLOSE : 正常停止解除 |
| Enable Switch | 外部使能开关 | OPEN : 开关释放 <br>CLOSE : 可运行（尝试电机上电） |
| Motor On | 外部电机上电 | 信号上升时（Rising Edge）尝试电机上电 |
| Remote | 外部模式输入（远程） | OPEN : 通过内部模式信号更改模式 <br>CLOSE : 通过外部模式输入信号更改模式
| Manual | 外部模式输入（手动）  | OPEN : 无动作 <br>CLOSE : 外部手动模式输入 |
| Auto | 外部模式输入（自动）  | OPEN : 无动作 <br>CLOSE : 外部自动模式输入 |
| Arm Limit | 机械臂限位输入| OPEN : 限位信号输入（危险） <br>CLOSE : 限位信号关闭（安全） |
| Primary axis Limit | 主轴限位输入 | OPEN : 限位信号输入（危险） <br>CLOSE : 限位信号关闭（安全） |
| Additional axis Limit | 附加轴限位输入 | OPEN : 限位信号输入（危险） <br>CLOSE : 限位信号关闭（安全） |
| External axis Limit | 扩展轴限位输入 | OPEN : 限位信号输入（危险） <br>CLOSE : 限位信号关闭（安全） |
| Monitored standstill #1 ~ #8 | 停止监控<br>(sos_0~sos_7) | OPEN : 功能启用<br>CLOSE : 功能禁用 |
| Joint speed set #1 ~ #8 | 关节速度<br>(speed_0~speed_7) | OPEN : 功能启用<br>CLOSE : 功能禁用 |
| TCP speed set #1 ~ #16 | TCP速度<br>(speed_0~speed_15) | OPEN : 功能启用<br>CLOSE : 功能禁用 |
| Joint angle #1 ~ #8 | 关节区域<br>(space_0~space7) | OPEN : 功能启用<br>CLOSE : 功能禁用 |
| TCP position(space) #1 ~ #16 | TCP区域<br>(space_0~space15) | OPEN : 功能启用<br>CLOSE : 功能禁用 |
| TCP orientation #1 ~ #8 | 工具方向<br>(orient_0~orient7) | OPEN : 功能启用<br>CLOSE : 功能禁用 |
| Self collision | 自碰撞 | OPEN : 功能启用<br>CLOSE : 功能禁用 |
| Power #1 ~ #16 | 功率<br>(power_0~power_15) | OPEN : 功能启用<br>CLOSE : 功能禁用 |
| Momentum #1 ~ #16 | 动量<br>(mmt_0~mmt_15) | OPEN : 功能启用<br>CLOSE : 功能禁用 |
| Collision detection #1 ~ #16 | 碰撞检测<br>(coldet_0~coldet_15) | OPEN : 功能启用<br>CLOSE : 功能禁用 |
| Speed & separation #1 ~ #84 | RePlan | OPEN : 功能启用<br>CLOSE : 功能禁用 |
| Mastering test switch | 标定测试开关 | OPEN : 功能启用<br>CLOSE : 功能禁用 |

### 安全输出信号的功能列表
|  **通道** |     **功能**                       |       **说明**    |
| :-------: | :--------------------------: |  :--------------------------------------------------: |
| Emergency stop activation status | 紧急停止状态 | OPEN : TP、OP、外部紧急停止中至少一个被按下 <br> CLOSE : TP、OP、外部紧急停止均未被按下  |
| Protective stop activation status | 保护停止状态 | OPEN : 非保护停止状态<br> CLOSE : 保护停止状态 |
| Normal stop activation status | 正常停止状态 | OPEN : 非正常停止状态<br> CLOSE : 正常停止状态 |
| Remote mode status | 外部操作状态 | OPEN : 内部操作模式<br> CLOSE : 外部操作模式 |
| Manual mode status | 手动模式状态 | OPEN : 非手动模式状态 <br> CLOSE : 手动模式状态 |
| Auto mode status | 自动模式状态 | OPEN : 非自动模式状态 <br> CLOSE : 自动模式状态|
| Motor Off status | 电机断电状态 | OPEN : 电机上电状态<br> CLOSE : 电机断电状态|
| Safety Function activation status | 安全功能启用状态 | OPEN : 安全功能禁用<br> CLOSE : 安全功能启用 |
| Monitord standstill activation status | 安全停止监控启用状态 | OPEN : 安全停止监控禁用<br> CLOSE : 安全停止监控启用 |
| Replan activation status | RePlan启用状态 | OPEN : RePlan禁用<br> CLOSE : RePlan启用 |
| Violation alarm | 安全功能违规状态 | OPEN : 安全功能违规<br> CLOSE : 无安全功能违规 |
| Monitord standstill #1~#8 violation | 安全停止违规<br>(sos_0~sos_7) | OPEN : 安全停止违规<br> CLOSE : 无安全停止违规 |
| Joint speed set #1~#8 violation | 关节速度违规<br>(speed_0~speed_7) | OPEN : 关节速度违规<br> CLOSE : 无关节速度违规 |
| TCP speed set #1~#16 violation | TCP速度违规<br>(speed_0~speed_15) | OPEN : TCP速度违规<br> CLOSE : 无TCP速度违规 |
| Joint angle #1~#8 violation | 关节区域违规<br>(space_0~space7) | OPEN : 关节区域违规<br> CLOSE : 无关节区域违规 |
| TCP position #1~#16 violation | TCP区域违规<br>(space_0~space15) | OPEN : TCP区域违规<br> CLOSE : 无TCP区域违规 |
| TCP orientation #1~#8 violation | 工具方向<br>(orient_0~orient7) | OPEN : 工具方向违规<br> CLOSE : 无工具方向违规 |
| Self collision detection | 自碰撞检测| OPEN : 检测到自碰撞<br> CLOSE : 无自碰撞 |
| Power #1~#16 violation | 功率违规<br>(power_0~power_15) | OPEN : 功率违规<br> CLOSE : 无功率违规 |
| Momentum #1~#16 violation | 动量违规<br>(mmt_0~mmt_15) | OPEN : 动量违规<br> CLOSE : 无动量违规 |
| Collition detection #1~#16 violation | 碰撞检测 <br>(coldet_0~coldet_15) | OPEN : 检测到碰撞<br> CLOSE : 无碰撞 |
| Mastering test error | 标定测试错误 | OPEN : 发生标定测试错误<br> CLOSE : 无标定测试错误 |
| Brake test error | 制动器测试错误 | OPEN : 发生制动器测试错误<br> CLOSE : 无制动器测试错误 |

{% hint style="info" %}
* 安全通信中，定义为 **OPEN = Bit 0**，**CLOSE = Bit 1**

{% endhint %}
