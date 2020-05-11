# CSS Table
-----------------------

CSS속성을 사용하면 테이블에 스타일링이 가능하다

# Table border
----------------

border속성으로 테이블의 테두리에 속성을 줄 수 있다

```css
table. th. td {
  border: 10px double black;
}
```

# border-collapse
-------------------
설정이 없으면 2중으로 되있는 사이 테두리를

하나로 합치는 속성

```css
table{
  border-collapse: collapse;
}
```

# Table width, height
------------------------

width와 height속성으로 테이블의 높이, 넓이 조절이 가능하다

```css
table {
  width: 100%
}

th {
  height: 50px;
}
```

# text-align
-------------------

text-align 속성으로 가로 정렬을 할 수 있다

디폴트는 \<th>는 center \<td>는 left이다

```css
th, td{
  text-align: center;
}

# vertical-align
-------------------

vertical-align 속성으로 세로 정렬을 할 수 있다

디폴트값은 th와 td 모두 middle 이다

```css
th, td{
  height: 50px;
  vertical-align:bottom;
}
```

# Padding
--------------
테이블 내에서 padding을 주면 글자와 테두리사이마다 여백이 주어진다

```css
th, td{
  padding: 15px;
  text-align: center;
}
```
# Horizontal dividers
--------------------
세로선없이 가로선만 사용하여 가로분배형 테이블을 만들 수 있다

```css
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  padding: 8px;
  text-align: left;
  border-bottom: 1px solid #ddd;
}
```

\<tr>에서 hover속성을 추가하면 마우스를 올렸을 때 하이라이트가 나온다

```css
tr:hover {background-color:#f5f5f5;}
```

\<tr>에 nth-child()을 추가하고 background-color속성을 추가하면 줄무늬 테이블을 만들 수 있다

```css
tr:nth-child(even) {background-color: #f2f2f2;}
```

\<th>,\<td> 등에서 background-color속성을 사용해 배경색을 넣을 수 있다

```css
th {
  background-color: #4CAF50;
  color: white;
}
```
