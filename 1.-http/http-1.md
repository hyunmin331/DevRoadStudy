# 과제) 작은 HTTP 웹 서버 만들기



* ## 요구사항
* Java를 이용해서 HTTP web server를 구현
* &#x20;ServerSocket을 이용해 로우레벨로 구현

### 구현할 기능들

* Todo 목록 얻기 - `GET /tasks`
* Todo 생성하기 - `POST /tasks`
  * Body data가 없을 경우 `400 Bad Request`
* Todo 제목 수정하기 - `PATCH /tasks/{id}`
  * 존재하지 않는 id로 요청하는 경우 `404 Not Found`
  * Body data가 없을 경우 `400 Bad Request`
* Todo 삭제하기 - `DELETE /tasks/{id}`
  * 존재하지 않는 id로 요청하는 경우 `404 Not Found`
