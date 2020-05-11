# CSS List
--------------------

HTML에선 \<ul>과 \<ol>에 각각 머릿문자가 추가되는 속성이다

CSS에선 머릿문자의 모양을 바꾸거나 배경색을 추가하는 등 스타일을 변경할 수 있다


# list-style-type
-----------

list-style-type 속성을 사용하면 리스트 마커를 바꿀 수 있다

```CSS
ul.a {
  list-style-type: circle;
}
ul.b {
  list-style-type: square;
}
ol.c {
  list-style-type: upper-roman;
}
ol.d {
  list-style-type: lower-alpha;
}
```

ul과 ol은 사용할 수 있는 type 값이 다르다

# list-type-image
---------------------
list-style-image 속성을 사용하면 마커로 이미지파일을 사용할 수 있다

```css
ul {
  list-style-type: url('sqpurple.gif');
}
```

# list-style-position
-----------------------

list-style-position은 마커의 위치를 변경하는 속성이다

값이 outside일 경우 본문과 떨어져있으며 이것이 디폴트값이다

값이 inside일 경우 글과 어울림 속성이 생긴다

```css
ul.a {
  list-style-position: outside;
}
ol.b {
  list-style-position: inside;
}
```

# tyle:none
------------------
list-style-type에 값을 none으로 주면 아이콘을 없앤다

다만 아이콘을 사용한것과 같은크기의 들여쓰기가 들어가므로

들여쓰기도 없애고 싶다면 margin과 padding값을 0으로 설정해야한다

```css
ul {
  list-style-type:none
  margin:0;
  padding:0;
}

# shorthand
------------------
list속성도 다른속성처럼 줄여쓰기가 가능하다

type position image등이 사용된다

```css
ul {
  list-style: square inside url("sqpurple.gif");
}
```

# list-style
------------------
목록에 색상을 주는 등 외적인 스타일링이 가능하다

ol, ul에 속성을 주면 해당 목록 전체가 변경되며

li에 속성을주면 해당 단일 개체만 변경된다

```css
ol {
  background: ##ff0000;
  padding: 20px;
}

ul {
  background:blue;
  padding: 20px;
}
ol li {
  background: #ffe5e5;
  padding: 5px;
  margin-left:35px;
}

ul li {
  background: #cce5ff;
  margin: 5px;
}
```

```
