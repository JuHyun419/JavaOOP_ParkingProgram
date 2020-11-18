## Java 주차장 관리 프로그램

### 승용차, 버스, 트럭 3종류가 있음.

  - **승용차**: 일반 차량 , 전기차(충전 가능)<br><br>

### 주차 요금
  - **승용차**: 최초 30분 2000원, 추가 10분당 1000원
  - **버스**: 승객수에 따라 대형(40인승↑) , 중형(24 ~ 40인승) , 소형(24인승↓) 으로 나뉨
    - **대형**: 최초 1시간 5000원, 추가 30분당 3000원
    - **중형**: 최초 1시간 4000원, 추가 30분당 2000원
    - **소형**: 최초 1시간 3000원, 추가 30분당 1000원
  - **트럭**: 중량에 따라 대형(10톤↑) , 중형(5 ~ 10톤) , 소형(5톤↓) 으로 나뉨
    - **대형**: 시간당 4000원
    - **중형**: 시간당 3000원
    - **소형**: 시간당 2000원

※ 전기차량의 충전요금 : 1kwh당 200원(소수점 X)<br><br>

### 요구사항
  - **입차**: 차량의 입차 정보(차량 번호, 차량 종류, 입차 시간)
  - **출차**: 차량의 출차 정보(차량 번호, 출차 시간), 총 요금 계산
  - **주차 차량확인**: 주차되어 있는 모든 차량의 종류별 입차시간을 정렬하여 보여줌
    - 차량은 승용차, 버스, 트럭 순으로 보여줌.
    - 출력할 차량 정보는 차량 종류, 차량 번호, 입차 시간
  - **총 수입**: 입차 후 출차한 차량에 대한 총 수입<br><br>

### 조건
  - 프로그램은 메뉴(Menu) 형식으로 작동하며, 무한 반복함
  - 차량 번호 - 4자리의 정수
  - 시간 정보 - 연,월,일,시,분 
    - ex) 202011171210
  - 주차시간의 계산은 전부 올림 처리하여 계산함
    - 승용차의 경우 30분 미만 -> 30분으로 처리하며, 1분~9분 -> 10분으로 처리함
  - 충전기의 출력은 12KW이고, 승용차 용량은 60Kwh라고 가정함
    - 배터리 완충시 걸리는 시간: 5시간이 소요됨
    - 1분에 충전할 수 있는 용량은 0.2kWh 임
  - 전기차는 완충될 때 까지 충전한다고 가정함
  
