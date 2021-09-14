# Promise 정리



## 설명

* **Promise는 자바스크립트 비동기 처리에 사용되는 객체이다. 자바스크립트에서의 비동기 처리란 '특정 코드의 실행이 완료될 때까지 기다리지 않고 다음 코드를 먼저 수행하는 자바스크립트의 특성'을 의미한다. **

* **Promise는 주로 서버에서 받아온 데이터를 화면에 표시할 때 사용한다.**

* **Promise는 3가지 상태가 존재한다.**

  * **Pending(대기) : 비동기 처리 로직이 아직 완료되지 않은 상태**
  * **Fulfilled(이행) : 비동기 처리가 완료되어 프로미스가 결과 값을 반환해준 상태**
  * **Rejected(실패) : 비동기 처리가 실패하거나 오류가 발생한 상태**

* #### Pending(대기)

  * ```javascript
    new Promise();
    ```

    **위와 같이 new Promise() 메서드를 호출하면 대기(Pending) 상태가 된다.**

    **new Promise() 메서드를 호출할 때 콜백 함수를 선언할 수 있고, 콜백 함수의 인자는 resolve, reject이다.**

    * ###### #아래는 전체 예제 코드 

  * ```javascript
    const condition = true; //true면 resolve, false면 reject
    const promise = new Promise((resolve, reject) => {
    	if (condition) {
    		resolve('성공');
    	} else {
    		reject('실패');
    	}
    });
    
    promise
    	.then((message) => {
    		console.log(message);
    	})
    	.catch((error) => {
    		console.error(error);
    	})
    	.finally(() => {
        	//끝나고 무조건 실행(이 정리에선 안다룰 예정)
    		console.log('무조건');
    	});
    
    //코드 출처: Node.js 교과서 
    ```



* #### Fulfilled(이행)

  * ```javascript
    new Promise(function(resolve, reject) {
      resolve();//이행
    });
    ```

    **resolve를 위와 같이 실행하면 이행(Fulfilled) 상태가 된다.**

    **이행 상태가 되면 아래와 같이 then()을 사용해 처리 결과 값을 받을 수 있다.**

  * ```javascript
    promise
    	.then((message) => {
    		console.log(message);
    	})
    ```



* #### Rejected(실패)

  * ```javascript
    new Promise(function(resolve, reject)) {
    	reject();//실패
    });
    ```

    **reject를 위와 같이 호출하면 실패(Rejected) 상태가 된다.**

    **그리고, 실패 상태가 되면 실패한 이유(실패 처리의 결과 값)을 catch()로 받을 수 있다.**

  * ```javascript
    promise
    	.catch((error) => {
    		console.error(error);
    	})
    ```

    

P.S.

Promise를 이해하기 위해선 비동기 처리에 대해 알아보는 것을 추천.





reference :

https://joshua1988.github.io/web-development/javascript/promise-for-beginners/

https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Promise