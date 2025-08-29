# 3.3.3 안전 입/출력

안전 입출력의 기본 정보

Hi6a의 안전 입출력은 다음과 같이 나뉠 수 있습니다.

1) 기본 안전 입력 (4ch x 이중입력)
2) 확장 안전 입력 (8ch x 이중입력)
3) 기본 안전 출력 (1ch x 이중입력)
4) 확장 안전 출력 (8ch x 이중입력)
5) PROFIsafe 통신 안전 입력 (64 점)
6) PROFIsafe 통신 안전 출력 (64 점)
7) CIP Safety 통신 안전 입력 (64 점)
8) CIP Safety 통신 안전 출력 (64 점)

![커넥터 위치](../../../_assets/safety_io/CommFront.png)

### 각각의 안전 입출력은 안전신호 할당(SIO Allocator)의 기능을 통해 제어기 내부에서 쓰이는 시스템 안전 입출력 또는 안전 응용프로그램의 신호들과 연결하여 사용할 수 있습니다.<br>


![안전 입력 할당의 예](../../../_assets/safety_io/SIO_Alloc_diagram1.bmp)

![안전 출력 할당의 예](../../../_assets/safety_io/SIO_Alloc_diagram2.bmp)