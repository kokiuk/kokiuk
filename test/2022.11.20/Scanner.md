## Scanner

```java
import java.util.Scanner;

Scanner scanner = new Scanner(System.in);
```

### 스케너로 다양한 데이터 받기
- 기본적으로 받고자 하는 자료형의 이름이 담긴 메서드를 사용한다
```java
//scanner.next<자료형>();
int scannedInt = scanner.nextInt();
long scannedLong = scanner.nextLong();
System.out.println(scannedInt);
System.out.println(scannedLong);

float scannedFloat = scanner.nextFloat();
double scannedDouble = scanner.nextDouble();
System.out.println(scannedFloat);
System.out.println(scannedDouble);

boolean scannedBool = scanner.nextBoolean();
System.out.println(scannedBool);
```

- float 데이터를 받는다고 굳이 입력에 F를 넣지 않는다 - 오히려 에러
- boolean 형은 true, flase 를 대소문자 구분하지 않고 넣어줄 수 있다
```java
String scannerLine = scanner.nextLine();
System.out.println(scannerLine)
```
- line형은 엔터 입력까지 한 줄의 문자열을 입력 받는다.

### 스케너 사용시 주의사항
```java
byte scanByte = scanner.nextByte();
short scanShort = scanner.nextShort();
int scanInt = scanner.nextInt();
long scanLong = scanner.nextLong();
```
위와 같은 코드에서, 1 1 1 1 처럼 공백으로 구분된 정수 넷이 입력되면?
- 네 줄의 코드가 동시에 동작한다.
- Scanner는 한 줄의 입력에 대해서 동작하는게 아니라, 입력된 모든 내용에서 일치하는 데이터를 찾는다.


