# CSS Margin
------------------

CSS margin은 border바깥의 여백이다

margin속성을 사용하면 여백을 조정할 수 있다.

#Individula side
-------------------
margin도 border처럼 개별 면만 속성을 지정하는것이 가능하다

-margin-top
-margin-right
-margin-bottom
-margin-left

참고로 음수값이 허용된다

```CSS
p {
  margin-top: 100px;
  margin-bottom: 100px;
  margin-right: 150px;
  margin-left: 80px;
}
```

# margin Shorthand
---------------------

margin도 border처럼 줄여쓰기가 가능하며 순서도 border와 동일하다

4가지일땐 상 우 하 좌 순서

3가지일땐 상 좌우 하 순서

2가지일땐 상하 좌우 순서

1가지일땐 모든면 에 적용된다

# auto
--------------
margin에 값을 auto로 주게될 경우

좌 우 여백을 균등하게 맞춘다

```CSS
body {
  width:300px;
  margin: auto;
  border:2px solid black;
}
```

# margin Collapse
-------------------
상단여백과 하단여백이 만나는 경우 두 여백중 큰 여백만 남고 작은 여백은 붕괴한다

좌 우 여백에는 붕괴가 일어나지않는다

```CSS
h1 {
  margin-bottom:200px;
}

h2 {
  margin-top:300px;
}
```
```html
<h1> h1 </h1>
<h2> h2 </h2>
```

위의 예시의경우 정상적으로라면 두 사이의 여백은 500px이겠지만

여백붕괴가 일어나서 두 사이의 여백은 300px만 표시된다
