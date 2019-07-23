## **_common_senses_**

- difference between import and .require
  . equire -> old method / import -> ES6

* middleware
  요청에 대한 응답 과정 중간에 껴서 어떠한 동작을 해주는 프로그램

* routing
  클라이언트에서 보내는 주소에 따라 다른 처리를 하는 것을 의미
  Router 는 요청을 보내는 길(분기)이다. 요청에 대한 응답을 res 로 받을 수 있다.
  익스프레스는 REST API에 따라 처리하는 데 그 방법이 아주 간단하다
  라우팅은 URI(또는 경로) 및 특정한 HTTP 요청 메소드(GET, POST 등)인 특정 엔드포인트에 대한
  클라이언트 요청에 애플리케이션이 응답하는 방법을 결정하는 것을 말한다.
  각 라우트는 하나 이상의 핸들러 함수를 가질 수 있으며, 이러한 함수는 라우트가 일치할 때 실행된다.

  - app = instance of express
  - METHOD = method of HTTP request
  - PATH = path of server
  - HANDLER = function that run when route matchs
