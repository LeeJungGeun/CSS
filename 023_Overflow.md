# Overflow
---------------
overflow속성은 영억보다 크기가 컨텐츠를 제어하는 속성이다

overflow는 내용이 너무 클때 자를것인지 스크롤을 만들것인지 지정한다

overflow는 4가지 값을 사용 가능하다

  - visible
  - hidden
  - scroll
  - auto

# visible
-------------------

디폴트값이며 요소의 밖에서도 표시되는 속성

```css
div {
  width: 200px;
  height: 100px;
  overflow: visible;
}
```

# hidden
---------------------
요소의 크기를 초과하는 부분은 숨김처리하는 속성

```css
div {
  overflow: hidden;
}
```

# scroll
--------------------------

요소의 크기를 고정시킨채 스크롤바를 만들어 요소의 크기를 초과하면 스크롤을 조정하는 방식의 속성

```css
div {
  overflow: scroll;
}
```

# auto
----------------

요소의 내용이 적으면 상관없으며 요소의 내용이 요소보다 커지면 스크롤을 만드는 속성

```css
div {
  overflow: auto;
}
```

# overflow-x, -y
------------------
overflow를 x축과 y축으로 따로 조정하는 속성

x는 가로로 조절 y는 세로로 조절한다

```css
div {
  overflow-x: hidden;
  overflow-y: scroll;
}
```
