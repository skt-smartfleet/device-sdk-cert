# SDK DVT(Development Validation Test) 검수 프로그램

본 인증프로그램은 SKT의 Smart[Fleet] 플랫폼 프로토콜을 따르는 ``GPS``, ``OBD`` 단말의 In/Out값이 명세에 맞게 데이터를 전송하는지 테스트하는 웹 기반의 프로그램입니다.

본 인증프로그램은 Smart[Fleet] 플랫폼의 [기술문서](http://smart-fleet-docs.readthedocs.io/ko/latest/)를 기반으로 구성되어 있습니다. 상세한 프로토콜은 상기 기술문서를 참고하세요.
<br>
<br>

## 실행방법
* 윈도우/리눅스/맥OS 버전의 바이너리 실행파일 형태로 제공됩니다.
* 리눅스와 맥OS는 `chmod 775 SmartFleet-linux` 또는 `chmod 775 SmartFleet-macos` 명령어를 사용하여 실행가능 상태로 변경해야합니다.

#### 인증프로그램 사용 포트 정보

포트    |  설명       |
--------------------|-----------------------------------------|
3001 | 웹 서버 접속을 위한 포트
1883 | MQTT 접속을 위한 포트
1884 | 웹소켓 기반의 MQTT접속을 위한 포트 (웹서버에서 사용)
8883 | MQTTS 접속을을 위한 포트

1. OS에 맞는 인증프로그램 다운로드후 실행
2. [http://localhost:3001](http://localhost:3001) 주소를 통해 인증 프로그램 접속
3. 장비의 사용자 인증키를 입력후 테스트 시작