# # Copy (Shallow/Deep)

## Shallow copy (얕은 복사)

```javascript
const obj1 = { a : 1, b : 2 };
const obj2 = obj1;

console.log( obj1 === obj2 ); // true
```

```javascript
const obj1 = { a:1, b:2 };
const obj2 = obj1;

obj2.a = 100;

console.log( obj1.a ); // 100
```

* 얕은 복사라는 이름이지만 정확히는 **값을 복사하는 것이 아닌 주소값을 복사**하여 같은 메모리를 가르킨다.
  * 해당 메모리 주소의 값이 변경되면 원본 객체 및 복사 객체의 인스턴스 변수 값도 변경된다.
* [인스턴스](https://github.com/dsmjimin/TIL-MD/blob/main/Spring%20boot/Class%2C%20Object%2C%20Instance.md)가 메모리에 새로 생성되지 않는다.



## Deep copy (깊은 복사)

```javascript
const obj1 = { name : "test1" };
const obj2 = { Object.assign( {} , obj1);

obj1.name = "test2";

// result

obj2.name	// 'test1'
obj1 === obj2	// false
```

* 원본 객체를 복사할 때, 해당 객체와 인스턴스 변수까지 복사하는 방식이다.
  * 복사된 객체는 완전히 독립적인 메모리를 차지한다. (복사한 후 값을 수정해도 기존 객체에는 영향을 끼치지 않음)
* 전부를 복사하여 새 주소에 담기 때문에 참조 공유를 하지 않는다.



reference :
> https://han.gl/PGijR  
> https://url.kr/ybz53s  
> https://velog.io/@ellyheetov/Shallow-Copy-VS-Deep-Copy  
> https://url.kr/obzxg7  
> https://hanamon.kr/javascript-shallow-copy-deep-copy/  
> https://url.kr/opd9a6  
> Object.assign : https://pro-self-studier.tistory.com/21  