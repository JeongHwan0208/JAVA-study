# Chapter 01 자바를 시작하기 전에

### 1.1 자바란?

 자바는 썬 마이크로시스템즈(Sun Microsystems)에서 개발하여 1996년 1월에 공식적으로 발표한 객체지향 프로그래밍 언어이다.

### 1.2 자바 언어의 특징

- **운영체제에 독립적이다.** 작성된 프로그램은 운영체제와 하드웨어에 관계없이 실행 가능
- **객체지향언어이다.** 자바는 객체지향개념의 특징인 상속,캡슐화, 다양성이 잘 적용되어 있다.
- **비교적 배우기 쉽다.**
- **자동 메모리 관리(Garbage Collection)** 자동적으로 메모리 관리를 해준다.
- **네트워크와 분산처리를 지원한다.** 
- **멀티쓰레드를 지원한다.**
- **동적 로딩(Dynamic Loading)을 지원한다.**

### 1.3 JVM(Java Virtual Machine)

  '자바를 실행하기 위한 가상 컴퓨터'라고 할 수 있다. 자바로 작성된 애플리케이션은 모두 이 가상 컴퓨터에서만 실행된다.

![1](https://github.com/JeongHwan0208/JAVA-study/blob/main/Java/Java%20image/1.jpg)

 일반 애플리케이션의 코드는 os만 거치고 하드웨어로 전달되는데 Java 애플리케이션은 JVM을 거치고 하드웨어로 가기때문에 OS와 하드웨어에 독립적이다. 단, JVM은 OS에 종속적이기 때문에 해당 OS에서 실행가능한 JVM이 필요하다.

![2](https://github.com/JeongHwan0208/JAVA-study/blob/main/Java/Java%20image/2.jpg)

 이렇게 함으로써 자바의 중요한 장점인 "Write once, run anywhere(한 번 작성하면 어디서든 실행된다.)"이 가능하게 된다.

### 2. 자바로 프로그램작성하기

 자바의 모든 코드는 반드시 클래스 안에 존재해야 한다.

```  java
   class 클래스이름{
        public static void main(String[] args) // main메서드의 선언부 'java.exe'에                                               의해 호출될 수 있도록 미리 약속된 부분
        {   
          // 실행될 문장들을 적는다.
        }
   }
```

 main메서드의 선언부 다음에 나오는 괄호{}는 메서드의 시작과 끝을 의미한다. Java 애플리케이션은 main메서드의 호출로 시작해서 첫 문장부터 마지막 문장까지 수행을 마치면 종료한다.

***      주의***

- *** 하나의 Java 애플리케이션에는 main메서드를 포함한 클래스가 반드시 하나는 있어야 한다.***
- ***public class가 있다면 소스파일의 이름은 public class의 이름과 일치해야 한다.***

### 2.1 자주 발생하는 에러와 해결방법

1. ***cannot find symbol 또는 cannot resolve symbol*** 변수 또는 메서드의 이름을 잘 못 사용한 경우
2. ***';'expected*** 세미콜론이 필요한 곳에 없는 경우
3. ***Exception in thread "main" java.lang.NoSuchMethoodError: main*** main메서드를 찾을 수 없는 경우
4. ***Exception in thread"main"java.lang.NoClassDefFoundError:Hello*** Hello라는 클래스를 찾을 수 없는 경우
5. ***illegal start tof expreesion*** 문법적 오류가 있는 경우
6. ***class, interface, or enum expected*** 보통 괄호의 개수가 일치하지 않는 경우

### 2.2 자바프로그램의 실행과정

```
     1. 프로그램의 실행에 한 클래스(*.class파일)를 로드한다.
     2. 클래스파일을 검사한다.(파일형식, 악성코드 체크) 
     3. 지정된 클래스에서 main(String[] args)를 호출한다.
```

### 2.3 주석(comment)

 주석을 이용해서 프로그램 코드에 대한 설명을 적절해 덧붙여 놓으면 프로그램을 이해하는 데 많은 도움이 된다. 그 외에도 주석은 프로그램의 작성자, 작성일시, 버전과 그에따른 변경이력 등의 정보를 제공할 목적으로 사용된다.

```
     범위주석: /*와 */사이의 내용을 주석으로 간주한다.
     한 줄 주석: //부터 라인 끝까지의 내용은 주석으로 간주된다.
```

***주의***

- ***문자열을 의미하는 큰따옴표(") 안에 주석이 있을 때에는 주석이 아닌 문자열로 인식된다.***





 





