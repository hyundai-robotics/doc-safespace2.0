# 3.3.3.5 자가 충돌 검지

자가 충돌 검지 기능은 로봇 2축과 툴의 충돌 여부를 감시하는 기능입니다. 툴과 로봇은 실제 형상에 맞게 모델링이 되어야하고, 모델링 방법에 대한 자세한 내용은 "[3.3.3.2 안전 툴 모델링](../../../3-safety-function/3-safety-function/3-safety-layout/2-safety-tool-modeling.md)"과 "[3.3.3.2 안전 로봇 모델링](../../../3-safety-function/3-safety-function/3-safety-layout/3-safety-robot-modeling.md)"을 참조하십시오.


<p align="center">
<img src="../../../_assets/safety_layout/self_collision.png"></img>
<em><p align="center">자가 충돌 검지 기능</p></em>
</p>



`[시스템 > 10: 안전 시스템 > 2: 파라미터 설정 > 2: 영역 제한 > 5: 자가 충돌 검지]` 메뉴에서 로봇의 자가 충돌 검지 기능을 사용하기 위한 파라미터를 설정할 수 있습니다. 

<p align="center">
<img src="../../../_assets/3/self_collision_param.png"></img>
<em><p align="center">자가 충돌 검지 기능 파라미터 설정 화면</p></em>
</p>

|  **파라미터** |                       **설명**                       |  **기본 설정값**  |
| :-------: | :------------------------------------------------: | :----------: |
| 활성화 | <p>기능 활성화 여부</p><p>(무효 / 유효 / 안전 입출력)</p> |   무효  |
| 정지 방법 |   <p>기능 위반시 정지 방법</p><p>(정지 0 / 정지 1 / 정지 2 / 무정지)</p>  | 정지 1 |
