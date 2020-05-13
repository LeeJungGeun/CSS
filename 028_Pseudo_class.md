# Pseudo class
-------------------

pseudo class는 요소의 특수상ㅇ태를 정의하는데 사용된다

- 마우스를 가져가면 스타일이 바뀜
- 들어간링크와 안들어간링크가 스타일이 다름
- 초점을맞출때 스타일이 바뀜

선택자: 클래스{
  속성: 값
}

형태로 작성한다

# link
---------------
링크 방문상태와 마우스위치에 따라 스타일변경 가능

```css
a:link {
  color: #FF0000;
}

a:visited {
  color: #00FF00;
}

a:hover {
  color: #FF00FF;
}

a:active {
  color: #0000FF;
}
```

hover는 link 와 visited 뒤에와야 효과적이다

active는 hover뒤에와야 효과적이다

pseudo-class는 대소문자를 구별하지 않는다

hover를 link가 아닌 div에 설정하는것도 가능하다

display:none으로 설정한 내용을

다른 요소에 hover속성으로 마우스를 올린동안만 block으로 만드는식으로 활용 가능하다

```css
p {
  display: none;
  background-color: yellow;
  padding: 20px;
}

div:hover p {
  display: block;
}
```

# first-child
-----------------------
combinator를 사용할 때 해당되는 첫번째 요소에 적용된다

```css
p:first-child {
  color: blue;
}
```
해당 예시에서는 처음으로나온 p에 속성이 부여된다

```css
p i:first-child {
  color: blue;
}
```

해당 예시의 경우 p속에서 처음으로나온 i에 속성이부여된다

```css
p:first-child i {
  color: blue;
}
```
이 예시의 경우 처음으로 나온 p의 모든 i에 속성이부여된다

# lang
--------------------
lang 을 사용하면 다른 문자에 특별한 규칙을 추가한다

```css
q:lang(A) {
  quotes: "~" "!";
}
```
위의 예시를 추가한 뒤

```html
<p>예시<q lang="A">문장</A>이다</p>
```
해당 문장을 입력할 경우

A태그가 선언된 자리와 끝나는 자리에 각각 ~와 ! 가 남게된다
