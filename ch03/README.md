# 변수와 데이터 입력
- l-value(공간), r-value(값)
- 문자는 따옴표, 문자열은 쌍따옴표
- 문자열 배열 크기는 문자열보다 1많게 설정해야 한다..
- 실수 - 실수형은 꼭 필요한 경우만 쓰고, 기본 double로 쓰는 것이 좋다.
    - f 를 붙여 4바이트 크기 상수로 처리되도록 작성
- 배열에는 대입 연산자를 사용할 수 없다. → strcpy() 를 사용해야 함.
## 예약어와 식별자
    - 예약어(reserved word;key word)
    - 식별자(identifier)의 종류
        - 변수명, 배열명, 함수명, 구조체명

## 추가공부
### short형 변수에 %d를 쓰면 안되는 이유
- overflow난다
    
    ```c
    short sh;
    scanf("%d",&sh); //sh는 2바이트만 확보했는데, sh 주소시작부터 4바이트에 넣기 때문에
    ```
    
### scanf() 입력 변환문자열 붙여서 받아도 된다?

```c
scanf("%d%d",&a,&b); //정상입력
scanf("%d %d", &a, &b); //중간에 다른 구분자를 넣을 수 있다.
```

- 입력시 구분자 이후의 공백은 무시한다.