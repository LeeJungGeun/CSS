# CSS Padding
----------------

CSS Padding 속성을 사용하면 요소의 컨텐츠와 border사이의 공간을 만들 수 있다

CSS padding 속성을 활용하면 이 공간을 제어할 수 있다.

# Individual Side
------------------

padding도 border나 margin처럼 개별 면만 제어하는것이 가능하다

```CSS
div {
  padding-top: 50px;
  padding-right: 30px;
  padding-bottom: 50px;
  padding-left: 80px;
}
```

# padding- Shorthand
------------------
마찬가지로 border와 margin처럼 줄여쓰는것 또한 가능하다

```CSS
div {
  padding: 50px 30px;
}
```

4자리 모두 입력시 상 우 하 좌 순서

3자리 입력시 상 좌우 하 순서

2자리 입력시 상하 좌우 순서

1자리 입력시 4면 전부 적용된다

# padding and width
----------------

width속성으로 넓이를 주었을 때 padding을 주게되면

요소의 총 넓이에 padding의 값이 추가된다

예상과는 다른 결과가 나올 수 있으니 주의가 필요하다

```CSS
div {
  width: 300px;
  padding: 25px;
}
```
위처럼 사용시 넓이 300에 padding 25가 양쪽에 추가되어

350px의 넓이를 갖게된다

box-sizing 속성을 사용하면 이것을 방지할 수 있다

```CSS
div {
  width: 300px;
  padding: 25px;
  box-sizing: border-box;
}
```
box-sizing 속성을 사용하면 넓이는 그대로 유지한 채 25px의 여백을 주는것이 가능하다
