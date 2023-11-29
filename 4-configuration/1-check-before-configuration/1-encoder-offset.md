# 1.5.1 엔코더 점검

협동로봇의 안전 기능은 각 축에 장착된 엔코더 데이터를 기반으로 로봇의 위치와 속도를 진단하므로 엔코더 데이터의 정확성이 중요합니다. 따라서 안전 기능 사용 전 엔코더 값과 실제 값이 일치하는지 점검해야 합니다.

1\. 로봇 각 축의 원점 눈금을 확인하여 축을 이동하십시오.
&#x20;&#x20;

안전 기능 위반으로 정지 발생 시 복구 모드 상태에서 조그로 각 축을 이동시키십시오. 복구 모드에 대한 자세한 내용은 “[**1.10.5 복구 모드**](../1-10-safety-condition-monitoring/5-recovery-mode/)”를 참조하십시오.

2\. 작업 영역의 포즈 정보창에서 로봇의 축좌표 값이 기준 자세(**0, 90 0, 0, 0, 0** \[deg])로 표시되는지 확인하십시오.
_assets
![](../../.gitbook/assets/image13.jpeg)

* 작업 영역에 포즈 정보창이 없으면, 패널 스택 우측 상단의 **\[+]** 버튼을 터치한 후 패널 선택창에서 **\[포즈]**를 터치하십시오.
_assets
![
](../../.gitbook/assets/image14.jpeg)

3\. 각도값의 오차가 0.01 이내이면 다음 단계로 진행하고, 오차가 0.01을 초과하면 엔코더 옵셋을 수행하십시오.

4\. 시스템을 재부팅하십시오.

{% hint style="info" %}
엔코더 옵셋에 대한 자세한 내용은 “[**Hi6 제어기 조작 설명서**](https://hyundai-robotics.gitbook.io/hi6-operation-manual)”의 “[**7.4.4 엔코더 옵셋**](https://hyundai-robotics.gitbook.io/hi6-operation-manual/7-setting/7-4-robot-parameter/encoder-offset)”을 참고하십시오.
{% endhint %}
