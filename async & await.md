# async & await



### async & await이란?

##### async와 await은 자바스크립트의 비동기 처리 패턴 문법이다. 기존 비동기 처리 방식인 콜백 함수와 프로미스의 단점을 보완하고 개발자가 읽기 좋은 코드를 작성할 수 있게 도와준다.

> #### + 개발자가 읽기 좋은 코드?
>
> ###### 위에서부터 아래로 한 줄 한 줄 차근히 읽으면서 사고할 수 있는 코드



### async & await 예시

```javascript
var user = {
	id: 1,
	name: 'Josh'
};
```



```javascript
function logName() {
	var user = fetchUser('domain.com/users/1');
	if (user.id === 1) {
		console.log(user.name);
	}
}
```

