# STUDY FOR TEAM PROJECT



## API

* #### Application Programming Interface. 애플리케이션 소프트웨어를 구축, 통합하기 위한 정의 및 프로토콜 세트를 나타낸다.

* #### API를 사용하면 구현 방식을 알지 못해도 제품 또는 서비스가 서로 커뮤니케이션 할 수 있으며, 애플리케이션 개발을 간소화하여 시간과 비용을 절약할 수 있다.

* #### 클라우드 네이티브 애플리케이션 개발을 통해 자체 인프라를 연결하는 간소화된 방식이다.

* API는 사람을 위한 인터페이스가 아니라 프로그램 간의 커뮤니케이션을 위한 기능이다.

  ```
  API 에 날짜/지역 정보를 전달 > API에서 날씨 정보를 응답
  ```

  

  reference

  https://www.a-mean-blog.com/ko/blog/%ED%86%A0%EB%A7%89%EA%B8%80/_/API

  https://steemit.com/kr/@yahweh87/it-api

  https://moonspam.github.io/What-is-an-API/

  https://dev-dain.tistory.com/50



## REST API(=RESTful API)

#### REST는 REpresentational State Transfer의 약자로, REpresentational은 어떤 리소스의 특정 시점의 상태를 반영하고 있는 정보, State는 웹 애플리케이션의 상태를 의미, Transfer는 이 상태의 전송을 의미한다.



#### REST API는 3가지의 구성으로 이루어져 있다.

* 자원(RESOURCE) - URI
* 행위(Verb) - HTTP METHOD
* 표현(Representations)



#### REST API 디자인 가이드

* REST API 설계 시 가장 중요한 항목은 2가지이다.
  * 첫 번째, URI는 정보의 자원을 표현해야 한다.

  * 두 번째, 자원에 대한 행위는 HTTP Method(GET, POST, PUT, DELETE)로 표현한다.

    

* REST API  중심 규칙

  * URI는 정보의 자원을 표현해야 한다.

    ```
    Get/members/delete/1
    ```

    위와 같은 방식은 REST를 제대로 적용하지 않은 URI. URI는 자원을 표현하는데 중점을 두어야 한다.

    

  * 자원에 대한 행위는 HTTP Method로 표현.

    위의 잘못 된 URI를 HTTP Method를 통해 수정하면,

    ```
    DELETE/members/1
    ```

    로 수정할 수 있다.



###### [참고]HTTP METHOD

POST, GET, PUT, DELETE 4가지 Method를 가지고 CRUD를 할 수 있다.

| METHOD |                             역할                             |
| :----: | :----------------------------------------------------------: |
|  POST  |        POST를 통해 해당 URI를 요청하면 리소스를 생성.        |
|  GET   | GET을 통해 해당 리소스를 조회. 리소스를 조회하고 해당 문서(Document)에 대한 자세한 정보를 가져옴. |
|  PUT   | PUT을 통해 해당 리소스를 수정.(자원의 전체를 교체, 자원교체시 모든 필드 필요) |
| DELETE |              DELETE를 통해 해당 리소스를 삭제.               |

###### ※ PATCH : 자원의 부분 교체, 자원교체시 일부 필드가 필요함.



reference

https://papababo.tistory.com/entry/HTTP-METHOD-PUT-vs-PATCH-%EC%B0%A8%EC%9D%B4%EC%A0%90

https://blog.npcode.com/2017/04/03/rest%EC%9D%98-representation%EC%9D%B4%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80/

https://meetup.toast.com/posts/92

https://www.redhat.com/ko/topics/api/what-is-a-rest-api