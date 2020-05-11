# CSS Link
-----------------

CSS에서는 링크에 다양한 스타일을 줄 수 있다

# Style link
-------------------

링크는 CSS속성으로 스타일될 수 있다

```css
a {
  color : red;
}
```

링크 상태에 따라 링크를 다르게 스타일링 할 수 있다

- a:link - 아무것도 아닐 때의 링크
- a:visited - 한번 들어갔단 링크
- a:hover - 마우스를 올려놓은 상태
- a:active - 마우스 버튼을 누르고 있는 상태

```css
a:link {
  color:red;
}

a: visited {
  color:pink;
}

a:hover {
  color:blue
}

a:active {
  color:green
}
```
active는 반드시 마지막에 와야하고

hover는 link,visited보다 늦게 와야한다

# Text=decoration
-----------------------
text-decoration 속성을 사용할 수 있으며

주로 밑줄을 지우는데 사용한다

```css
a:link {
  text-decoration: none;
}

a: visit {
  text-decoration: none;
}
```

# background color
----------------------
링크의 배경색을 지정하는데 사용되는 속성

```css
a:link {
  background-color: yellow;
}

a:visited {
  background-color: cyan;
}
```

# link button
-------------------
링크를 상자,버튼등으로 스타일하여 만들 수 있다

```css
 a:link, a:visited {
  background-color: red;
  color: white;
  padding: 20px. 30px;
  text-align: center;
  text-decoration:none;
}
```
