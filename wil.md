<1주차 스터디를 통해 배운 내용>

1. 웹(Web):

웹은 여러 컴퓨터가 서로 연결되어 클라이언트-서버 모델을 기반으로 정보를 주고받는 공간이다. 

2. 클라이언트-서버 모델:

클라이언트는 데이터의 생성, 조회, 수정, 삭제를 요청하는 쪽이고, 서버는 그 요청을 처리하여 응답을 보내는 역할을 한다.
ex) 브라우저에서 네이버에 접속하면, 클라이언트가 네이버 서버에 데이터를 요청하고 서버가 응답을 보낸다.

3. HTTP (HyperText Transfer Protocol):

웹에서 클라이언트와 서버가 통신할 때 사용하는 프로토콜로, HTTP 메소드와 URL을 통해 요청이 이루어지고, 서버는 이에 대해 응답을 보냅니다.
<HTTP 메소드>
-GET: 데이터를 조회
-POST: 데이터를 생성
-PUT/PATCH: 데이터를 수정
-DELETE: 데이터를 삭제
-URL은 데이터를 어디서 가져올지 나타내고, 응답은 HTTP 상태 코드로 처리 결과를 알려준다 ( ex) 200 OK, 404 Not Found ).

4. 프론트엔드 - 백엔드:

프론트엔드는 사용자에게 보이는 화면을 구성하고, 백엔드는 서버 측에서 데이터 처리를 담당한다.
프론트엔드는 백엔드에 데이터를 요청하고, 백엔드는 데이터베이스에서 데이터를 가져와 응답하는데, 이때 주고받는 데이터는 JSON 형식을 주로 사용한다.

5. API (Application Programming Interface):

API는 응용 프로그램들이 서로 소통하기 위한 규칙을 정의한 인터페이스로 웹에서는 클라이언트가 백엔드 서버에 요청을 보낼 때 API를 사용한다.
REST API는 자원을 URL로 나타내고, HTTP 메소드로 작업을 지정하는 방식이다.

***API 명세서 작성***

<할 일 관련 API>

1. 할 일 전체 조회
HTTP Method: GET
URL: /todo/list

2. 할 일 생성
HTTP Method: POST
URL: /todo

3. 할 일 수정
HTTP Method: PATCH
URL: /todo/{todoId}

4. 할 일 삭제
HTTP Method: DELETE
URL: /todo/{todoId}

5. 할 일 체크
HTTP Method: POST
URL: /todo/{todoId}/check

6. 할 일 체크 해제
HTTP Method: POST
URL: /todo/{todoId}/uncheck

<유저 관리 API>

1. 회원 가입 (회원 정보 생성):
HTTP Method: POST
URL: /user/register

2. 로그인 (인증):
HTTP Method: POST
URL: /user/login

<친구 관련 API>

1. 친구 추가:
HTTP Method: POST
URL: /friend/{friendId}

2. 친구 목록 조회:
HTTP Method: GET
URL: /friend/list

3. 특정 친구 정보 조회:
HTTP Method: GET
URL: /friend/{friendId}

4. 특정 친구의 할 일 목록 조회:
HTTP Method: GET
URL: /friend/{friendId}/todo/list

5. 친구 삭제:
HTTP Method: DELETE
URL: /friend/{friendId}

