# 자바 기초

## Variables And Types

## 변수 - 데이터를 담는 상자와 같은 역할
```java
    public static void main(String[] args){
        int a = 300;
        System.out.println("a = " + a);
        String b = "Hello";
        System.out.println("b = " + b);
    }
```
위에서 a와 b는 변수이다.

### 변수
- 할당 연산자를 이용하여 값을 할당 할 수 있다.
- <자료형><이름> = <값>
- 변수를 만드는 것을 선언 이라고 부른다.
- [변수의 값은 다시 할당 할 수 있다.](./Reallocation.md)  

변수의 선언과 할당은 반드시 한번에 이뤄질 필요가 없다.
```java
    int date;
    ~~~
    //작업 후
    ~~~
    date = 100;
```
한 줄에 여러 변수를 동시에 선언도 가능하다.
 ```java
    int month = 11, day = 20;
```

### 변수 이름 규칙
- 문법적인 관념
    1. 숫자로 시작할 수 없다.
    2. _ 와 $ 외의 특수문자를 사용할 수 없다.(#등등)
    3. int, class, return 등의 예약어를 사용할 수 없다.

- Naming Convention
    1. 서로 다른 개발자가 보았을 때, 그것이 무엇인지 알아볼 수 있도록 상호 합의된 규칙
    2. Java에서 변수 이름을 정할 때는 일반적으로 camelCase로 짓는다.
        - 기본적으로 소문자 사용
        - 여러 단어를 변수 이름에 쓰고 싶다면 , 단어가 바뀌는 시점에 대문자 사용
        ```java
        int 1stVar  //문법적 오류
        int second_var // 오류는 없지만 camelCase가 아님
        int thrVar // 옳은 방법
        ```


## 자료형 - 데이터의 종류
어떤 변수를 선언하면서, 해당 변수가 어떤 데이터를 저장할 수 있는지 정의

### 정수 자료형
|  자료형 |  최대 |  최소 |
|---|---|---|
|  int |  -2147483638 | 2147483637  |
| long  |  -9,223,372,036,854,775,808 | 9,223,372,036,854,775,807  |
| short  | -32768  | 32767  |
| byte  |  -128 |  127 |

주로 int와 long을 쓴다. ~~short와 byte는 잘 사용하지 않는다.~~
```java
int intNum = 1726314;
long longNum = 10000000000L;
short shortNum = 32000;
byte byteBum = 120;
```

### 실수 자료형
|  자료형 |  최대 |  최소 |  유효자리수 |
|---|---|---|---|
|  flaot |  1.175494351 E - 38 | 3.402823466 E + 38  | 7|
| double  |  2.2250738585072014 E - 308 | 1.7976931348623158 E + 308  | 16 |

기본적으로 소숫점을 사용해 숫자를 표현하면 double이 된다.
```java
flot folatPoint = 3.141592f;
double doublenum = 3.1415926535;
```




