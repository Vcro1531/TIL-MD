# @Not ◦ Null, Empty, Blank 정리



#### @NotNull, @NotEmpty, @NotBlank

#### 위 3가지 어노테이션은 Bean Validation에서 제공하는 표준 Validation이다.

(Bean Validation = Java에서 제공하는 데이터 유효성 검사 프레임워크)

#### 사용 방법은 유사하지만 잘못 사용했다간 완전 다른 결과를 초래할 수 있다.



## @NotNull

* 이름 그대로 Null만 허용하지 않는다.
  * 따라서, "" 또는 " " 은 허용하게 된다.
* Null이 들어오게 되면 로직에 예상치 못한 오류가 발생하거나 문제가 생길 경우 사용해야 한다.



### @NotEmpty

* NotNull과 똑같이 null 허용 X, "" 또한 허용하지 않는다.
* String과 collection 타입에만 적용된다.



### @NotBlank

* 세개 중 가장 Validation 강도가 높다.
* null, "", " " 모두 허용하지 않는다.





reference :

> https://sanghye.tistory.com/36
>
> https://itcoin.tistory.com/499