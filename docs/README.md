## 🛠기능목록

---

- **컴퓨터 숫자 생성 (model & Controller & Service)**
    - 1~9 랜덤 숫자 세개 배열에 저장
    - 배열에 중복된 수 유무 확인
- **유저 숫자 받기 (model & Controller & Service)**
    - 유저에게 숫자 받기
        - [예외] input길이 ≠ 3
        - [예외] input 속 문자 중 숫자가 아닌 경우
        - [예외] input 속 문자 중 0이 있는 경우
        - [예외] input 속 문자 중 중복된 수가 있는 경우

      ⇒ `IllegalArgumentException`을 발생시킨 후 애플리케이션 종료

- **입력값에 따른 힌트 (Controller & Service)**
    - 같은 수가 같은 자리 => 스트라이크
    - 같은 수가 다른 자리=> 볼
    - 같은 수 존재X => 낫싱
- **사용자에게 출력 (View)**
    - 사용자에게 숫자를 입력받는 메세지 출력
    - 스트라이크/볼/낫싱 여부 출력
    - 3스트라이크 승리 출력과 게임 종료
    - 재시작 여부 메세지 출력
- **게임 반복 여부 (Controller & Service)**
    - 유저에게 인풋 받기 (1이면 재시작, 0이면 종료)
        - [예외] ‘1’, ’0’ 외의 문자열
    - 게임 재시작/ 종료
