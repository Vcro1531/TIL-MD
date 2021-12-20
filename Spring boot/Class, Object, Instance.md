# Class, Object, Instance



> ## 기본적인 개념



### 클래스(Class)

* #### 개념

  * ##### 객체를 만들어 내기 위한 **설계도**

  * ##### 연관되어 있는 변수와 메서드의 집합
  
  * ##### Object에 대한 template



### 객체(Object)

* #### 개념

  * ##### 소프트웨어 세계에 구현할 대상

  * ##### 클래스에 선언된 모양 그대로 생성된 실체

  * ##### 현실세계의 모든 실체

* #### 특징

  * ##### 모든 인스턴스를 대표하는 포괄적인 의미를 갖는다.

  * ##### '클래스의 인스턴스(instance)'라고도 부른다.



### 인스턴스(Instance)

* #### 개념

  * ##### 설계도를 바탕으로 소프트웨어 세계에 구현된 <u>구체적인 실체</u>

  * ##### Object를 소프트웨어에 실체화 하면 그것을 '인스턴스'라고 부른다.

  * ##### 실체화된 인스턴스는 메모리에 할당된다.

  * ##### Memory에 생성된 Object

* #### 특징

  * ##### 인스턴스는 객체에 포함된다고 볼 수 있다.

  * ##### 추상적인 개념(또는 명세)과 구체적인 객체 사이의 관계에 초점을 맞출 경우에 사용한다.

```java
/* Class */
public class Animal {
    ...
}
/* Object & Instance */
public class Main {
    public static void main(String[] args) {
        Animal cat, dog; // 'Object'
        
        //Instance
        cat = new Animal(); //cat(Object)는 Animal(Class)의 Instance
        dog = new Animal();
    }
}
```



> ## 차이점



### 클래스(Class) Vs 객체(Object)

* ##### 클래스는 '설계도', 객체는 '설계도로 구현한 모든 대상'을 의미한다.

  * ##### ![클래스와 객체? - 그림으로 배우는 자바, 객체지향!](https://i.imgur.com/GAhMIfG.png)



#### 객체(Object) Vs 인스턴스(Instance)

* ##### 클래스의 타입으로 선언되었을 때 객체라고 부르고, 그 객체가 메모리에 할당되어 실제 사용될 때 인스턴스라고 부른다.

* ##### 객체는 현실 세계에 가깝고, 인스턴스는 소프트웨어 세계에 가깝다.



reference :

> https://gmlwjd9405.github.io/2018/09/17/class-object-instance.html
>
> https://youtu.be/XBG6CUtVCIg
>
> https://opentutorials.org/course/1223/5400
> https://gmlwjd9405.github.io/2018/09/17/class-object-instance.html