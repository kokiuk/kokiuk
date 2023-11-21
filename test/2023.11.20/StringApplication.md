## 문자열 응용

### 특수문자 사용
Escape Sequence – 키보드로 입력하기 어려운 특수한 문자를 표현하기 위해 사용되는 문자 조합
- Escape Character – Escape Sequence를 만들기 시작한다는 의미의 특수문자, 주로 \가 활용됨

```java
// " 표현
System.out.println("\"");
// ' 표현
System.out.println("\'");
// \표현
System.out.println("\\");
```


|  Escape Sequence |  결과 |
|---|---|
|  \n |  다음 줄 |
| \t  |  탭 |
| ~~\r~~  | ~~캐리지리턴~~  |
| ~~\b~~  | ~~백스페이스~~ |

~~\r 과 \b는 잘 사용하지 않는다.~~

```java
//엔터키(개행문자), 백스페이스, 텝키
System.out.println("개행문자 : \n 다음 줄에 표시");
System.out.println("name\tscore");
System.out.println("Alex\t3.5");
System.out.println("Thomas\t4.5");

/* 결과

개행문자 : 
 다음 줄에 표시
name	score
Alex	3.5
Thomas	4.5

*/
```

### String Fomattion
어떤 문구를 문자열로 나타낼 떄, 상황에 따라 일부분만 바꾸어서 표현하고 싶은 경우  

```java
String msg = "미세먼지 농도 : 10 -> 좋음";
```
위에서 농도 수치와 상태('좋음')을 변수에 저장한다면 ?

```java
int dust = 10;
String state = "좋음";
```

위의 변수의 값을 문자열 안에 표현하는 방법 
- 여러가지 방법이 있지만, **String.fomat**을 많이 활용

|  코드 |  자료형 |
|---|---|
| %s |  문자열 (String) |
| %c  |  문자 (Char) |
| %d  | 정수 (Int)  |
| %f  | 부동소수 (Float,Double) |

```java
System.out.println(String.format("미세먼지 농도 : %d -> %s", dust, state));
```

