### 변수의 재할용

변수는 재할당이 가능하기에 값을 재활용 할 수있어서 유용하게 사용 할 수 있다.

```java
    int americano = 1500;
    int cappuccino = 2500;
    int cafeLatte = 3000;
    int cafeMoca = 4000;

    //아메리카노 3잔 가격 출력
    System.out.println(3*americano);
    //카푸치노 3잔 + 아메리카노 2잔 가격 출력
    System.out.println(3*cappuccino + 2*americano);
    //카페모카 1잔 + 아메리카노 3잔 가격 출력
    System.out.println(cafeMoca + 3*americano);

    //아메리카노 가격 변경
    americano = 2000; // 변수 재할당

```