## 배열
하나의 변수에 여러개의 데이터를 정리하여 저장하기 위해 사용
```java
int[] score = {10,20,30};
```
- 변수를 선언할 때, 자료형 뒤에 [] 를 덧붙여 선언, 그 뒤 {}를 이용해 저장할 값들을 나열한다.
- 이후 다시 가져올 때는 변수에 [] 를 이용하며, [] 안에 몇번째 값을 가져올지를 지정한다.
- **첫번째 아이템은 0이다**.
- 배열에 들어갈 데이터가 정해지기 전이라면, 크기를 먼저 결정해서 할당할 수 있다.
    ```java
    String[] name = new String[3];
    name[0] = "고기욱";
    ```
- 크기를 정할 때, 그 크기도 마찬가지로 변수로 둘 수 있다.
    ```java
    int count = 10;
    String[] name = new String(count);
    int[] socres = new int(count);
    ```

- 만약 이미 존재하는 배열의 크기를 이용하고 싶으면
**배열.length**를 활용하자
    ```java
    int numOfStudents = studentsNames.length;
    ```

