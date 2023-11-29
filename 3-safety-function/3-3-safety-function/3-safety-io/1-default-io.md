# 1.8 안전 I/O 신호

Default Safety I/O의 파라미터를 설정합니다.
입력 신호는 4개, 출력 신호는 1개 이며 모두 이중신호로 동작 됩니다.

**1. Default Safety Input**

![Default Input Image](../../../_assets/safetyio_profisafe/default_in.PNG)

 - Pulse Test : 각 채널별로 Pulse Test의 사용 여부를 선택할 수 있습니다.
 - Error Latch Time : 해당 채널에 에러가 발생하면 에러가 복구 되더라도 **Error Latch Time** 시간 이후에 Fail-Safe 값에서 현재 입력된 신호로 변경됩니다.
 - Filter Time : 각 채널별로 Filter Time 동안 일정한 신호가 입력되어야 유효한 신호로 처리됩니다.
 - Discrete Time :  Default Safety Input 은 2개의 이중 신호가  같은 값일때 유효한 신호로 처리되고 이 2개의 신호가 **Discrete Time** 시간 보다 큰 시간 동안 다르게 되면 알람이 발생하게 됩니다.
 
**2. Safety Output**

![Default Output Image](../../../_assets/safetyio_profisafe/default_out.PNG)

 - Pulse Test : 각 채널별로 Pulse Test의 사용 여부를 선택할 수 있습니다.
 - Error Latch Time : 해당 채널에 에러가 발생하면 에러가 복구 되더라도 **Error Latch Time** 시간 이후에 Fail-Safe 값에서 현재 입력된 신호로 변경됩니다.


