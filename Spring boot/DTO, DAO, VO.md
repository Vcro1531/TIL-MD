# DTO(Data Transfer Object)

* 계층간(Controller, View, Service) 데이터 교환을 위한 Java Beans를 의미

* 로직을 가지지 않는 데이터 객체이고 getter/setter 메소드만 갖음

* 주로 비동기 처리를 할 때 사용

* Controller Layer에서 Response DTO 형태로 Client에 전달

* 예제코드

  * ```null
    @Getter @Setter
    class ArticleDTO {
      private String title;
      private String content;
      private String writer;
    }
    ```

* **하지만 DB에서 꺼낸 값을 임의로 변경할 필요가 없기 때문에 DTO클래스에는 setter가 없음** 





# DAO(Data Access Object)

* DB의 data에 접근하기 위한 객체
* 직접 DB에 접근하여 데이터를 삽입, 삭제, 조회 등 조작할 수 있는 기능을 수행
* DB 접근을 하기 위한 로직과 비즈니스 로직을 분리하기 위해 사용



# VO(Value Object)

* DTO와 동일한 개념이지만 Read-Only 속성을 갖음
  * DTO는 Layer간의 통신 용도로 오고가는 객체를 말하고, VO는 특정한 비즈니스 값을 담는 객체



reference :

> https://lemontia.tistory.com/591
>
> https://velog.io/@ha0kim/DAO-DTO-VO-%EC%B0%A8%EC%9D%B4