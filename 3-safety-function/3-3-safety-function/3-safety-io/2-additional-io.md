# 3.3.2 Additional Safety I/O

Additional Safety I/O의 파라미터를 설정합니다.
입력 신호는 8개, 출력 신호는 4개 이며 모두 이중신호로 동작 됩니다.

**1. Additional Safety Input/Output**

![Additional Input Image](../../../_assets/add_io.PNG)

 - Enable : Additional Safety I/O의 사용 유무를 결정합니다.
 - 필터 시간 : 각 입력 채널별로 필터 시간 동안 일정한 신호가 입력되어야 유효한 신호로 처리됩니다. (Unit : msec)
 - Discrete 시간 :  Additional Safety Input 은 2개의 이중 신호가  같은 값일때 유효한 신호로 처리되고 이 2개의 신호가 **Discrete 시간** 보다 큰 시간 동안 다르게 되면 알람이 발생하게 됩니다. (Unit : msec)
 - Input Error Latch 시간 : 해당 채널에 에러가 발생하면 에러가 복구 되더라도 **Input Error Latch 시간** 이후에 Fail-Safe 값에서 현재 입력된 신호로 변경됩니다. (Unit : msec)
 - Output Error Latch 시간 : 해당 채널에 에러가 발생하면 에러가 복구 되더라도 **Output Error Latch 시간** 이후에 Fail-Safe 값에서 출력 하려는 신호 레벨로 변경됩니다. (Unit : msec)
 
 

