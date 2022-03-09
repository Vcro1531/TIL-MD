# React 다운로드 방법

> #### In MacOS

* [Node.js](https://nodejs.org/ko/)에서 최신 버전 다운로드
  * 오류가 일어날 수 있기 때문에 전에 다운로드를 했더라도 다시 하는걸 추천
* 폴더 하나 생성

* 만들어놓은 폴더를 열고 (Vscode 기준) 터미널에서 **npx create-react-app (프로젝트명)**
* 왼쪽 상단 File -> Open Folder -> 자신이 만든 폴더에 (프로젝트명)을 선택
  * 제일 처음 만든 폴더에서는 React가 안켜짐

* 터미널에서 npm start를 입력
  * localhost:3000(기본)으로 열리며 Vscode에서 저장하면 페이지가 바로바로 반응함



# React

> ## 사용자 인터페이스를 만들기 위한 JavaScript 라이브러리
>
> (React 공식 홈페이지 문구)

* 유저 인터페이스를 만들기 위한 오픈 소스 자바 스크립트 라이브러리
* AngularJS, VueJS와 함께 가장 많은 인기를 얻고 있음
* Meta(전 facebook)가 개발한 라이브러리

### 장점 :

* SPA(Single Page Application) : HTML, CSS, JavaScript 파일을 최초 1회만 로드하고, 이후에는 자바스크립트 파일을 통해
  DOM 또는 필요한 HTML 파일을 조작하는 방식.
  이전에는 동적인 웹 페이지를 위해서는 모든 페이지마다 HTML, CSS, JS 파일을 각기 가지고 있어야 해서 페이지 이동마다 속도가 느렸음.

* CSR(Client Side Rendering) : 서버로부터 데이터를 받아서 바뀐 부분의 데이터가 있는 화면만 새롭게 랜더링하는 방식.
  효율적으로 클라이언트 리소스를 사용하게 한다.
  서버가 HTML, CSS, JS파일을 랜더링하는 대신 데이터를 보내줄 경우, 안드로이드, IOS, 웹 모바일 등 다양한 플랫폼이 서버를 공유할 수 있게 되어 효율적으로 서버를 운영할 수 있게 된다.
* 컴포넌트(Component) : 프로그래밍에 있어 재사용이 가능한 독립적 관리 가능 모듈.
  대규모 웹 애플리케이션에서 컴포넌트는 역할과 기능에 따라 따로 관리하기 용이함.
  반복되는 부분을 대체할 수 있게 해주어서 **코드 재사용성을 높여줌**.
* 다양한 라이브러리 : AngularJS, VueJS에 비해 사용자가 많기 때문에 다양한 자료와 커뮤니티가 있음.
* 가상 돔(Virtual DOM) : 실제 돔에 적용시키기 전 가상의 DOM을 만들어 적용시키고, 최종 완성된 결과만 DOM으로 적용시킴.
  브라우저가 실행하는 연산의 양을 줄일 수 있음.

### 단점 :

* View 이외 : 프레임워크의 MVC와 비교하였을 때 View 부분만 관리하기 때문에 다른 부분은 써드파티 라이브러리를 이용하거나 직접 구현해야함.

* JSX : JavaScript를 확장한 문법으로 React에서 HTML 대신 사용한다. 필수는 아니지만 대부분의 사람들이 이용하고 React에서도 지원하기 때문에 배움. 처음 배울 때는 익숙치 않을 수 있다.



reference : 

> https://youtu.be/nahwuaXmgt8
>
> https://velopert.com/3612
>
> https://url.kr/vfagmr (단축 url)
>
> https://url.kr/izogdb (단축 url)
>
> https://hanamon.kr/%EC%BB%B4%ED%8F%AC%EB%84%8C%ED%8A%B8-component%EB%9E%80/
>
> https://helloworld-88.tistory.com/350
>
> https://developerntraveler.tistory.com/54





