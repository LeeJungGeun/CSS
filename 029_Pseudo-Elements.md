# CSS Pseudo-elements
------------------------

CSS의사요소는 요소의 지정된부분에 다른 스타일을 정의한다

예를들어

- 요소의 첫글자, 첫줄
- 머릿말과 맺음말

선택자:의사요소{
  속성:값
}

으로 작성된다

# first-line
----------------
::first-line 의사요소를 사용하면 퍼줄만 다른 스타일링을 할 수 있다

```css
p::first-line {
  color: red;
}
```

# first-letter
-------------------

::first-letter 의사요소는 첫먼째 글자에 스타일을 부여한다

```css
p::first-letter {
  color: red;
  font-size: xx-large;
}
```

의사요소는 CSS클래스와 결합될 수 있다

```css
p.intro::first-letter {
  color: red;
  font-size: 200px;
}
```
해당예시는 intro 클래스에 의사요소를 부여한 경우이다.

여러개의 의사요소도 겹칠 수 있다

```
p::first-letter {
  color: red;
  font-size: 200px;
}

p::first-line {
  color: blue;
}
```
해당예시는 첫글자는 200px크기의 붉은글자 그외 첫번째줄은 파란색을 주었다

# before after
-----------------
::before 의사요소와 ::after의사요소는 각각 요소의 앞과 뒤에 컨텐츠를 추가할 수 있다

```css
h1::before {
  content: url(ex.gif);
}

h2::after {
  content: url(ex.gif);
}
```

# Selection
---------------

::selection 의사요소는 드래그한 부분의 속성을 바꾼다

color background cursor outline이 사용 가능하다

```css
::selection {
  color: red;
  background: yellow;
}
```
해당요소 추가시 페이지 내에서 드래그하면 노란배경에 빨간글자로 바뀐다
