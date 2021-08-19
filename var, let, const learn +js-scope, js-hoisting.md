# var, let, const 차이점

> ## + scope, hoisting 설명



## 1. 변수 선언 방식

### ◈ var 

```javascript
var variable = '변수선언함';
console.log(variable); //변수선언함

var variable = '또 변수선언함';
console.log(variable); //또 변수선언함
```

* ##### 변수 선언을 여러 번해도 에러 없이 각기 다른 값을 출력할 수 있다.
* ##### 필요할 때 마다 변수를 사용할 수 있다는 장점이 될 수도 있다.

* ##### 같은 이름의 변수명을 남용해 또 다른 문제를 일으킬 수 있기 때문에 단점이 더 크다.



### ◈ let

```javascript
let variable = '변수선언함';
console.log(variable); //변수선언함

variable = '변수 재할당함';
console.log(variable); //변수 재할당함

let variable = '또 변수선언함';
console.log(variable); //또 변수선언함
```

* ##### var의 단점을 보완하여, 변수의 재선언을 불가능하게 만들었다.

* ##### 변수의 재할당은 가능하다.



### ◈ const

```javascript
const variable = '변수선언함';
console.log(variable); //변수선언함

variable = '변수 재할당함';
console.log(variable); //변수 재할당함(에러)

const variable = '또 변수선언함';
console.log(variable); //또 변수선언함(에러)
```

* ##### constant(상수)를 의미하며 let과 같이 재선언은 불가하고, let과는 다르게 재할당을 통해 바꿀 수도 없다.



### ▣ JS Scope(스코프)

* ##### 우리말로 '범위'라는 뜻을 갖고 있으며, Java Script에서는 '변수에 접근할 수 있는 범위'라고 나타낼 수 있다.

* ##### Java Script에서는 Global Scope와 Local Scope 두 가지가 있다.

  * #### Global Scope(전역 변수)

    >##### 전역 범위에서 선언된 변수이다.
    >
    >##### 웹 페이지의 모든 스크립트와 함수가 액세스 할 수 있다.

  

  * #### Local Scope(지역 변수)	

    >##### 블록 내부에서 선언된 변수이다.
    >
    >##### 함수 내에서만 액세스 할 수 있다.
    >
    >##### 함수 내에서만 인식되기 때문에 같은 이름의 변수를 다른 함수에서 사용할 수 있다.
    >
    >##### 함수가 시작될 때 생성되고 함수가 완료되면 삭제됩니다.



### ▣ JS Hoisting(호이스팅)

* ##### 함수 안에 있는 선언들을 모두 끌어올려서 해당 함수 유효 범위의 최상단에 선언하는 것.
  
  * ##### 주의점 : var 변수 선언과 함수 선언문에서만 호이스팅이 일어난다.
    
    * ##### var 변수/함수의 선언만 위로 끌어올려지며, 할당은 끌어 올려지지 않는다.
    * ##### let/const 변수 선언과 함수표현식은 호이스팅이 발생하지 않는다.
  * ##### 실제 메모리는 변화가 없다.
* ##### 사용 시 주의점
  
  * ##### 코드의 가독성, 유지보수를 위해 호이스팅이 일어나지 않도록 한다.
  * ##### var를 사용하기 때문에 혼란스럽고 쓸모없는 코드가 생길 수 있다.







reference

https://backstreet-programmer.tistory.com/76

https://velog.io/@xedni/Scope

https://www.w3schools.com/js/js_scope.asp

https://gmlwjd9405.github.io/2019/04/22/javascript-hoisting.html