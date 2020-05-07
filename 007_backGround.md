# CSS Background
------------------
CSS의 background 속성은 요소의 배경 효과를 정의하는데 사용된다 

# Background Color
------------------

background-color  속성은 요소의 배경색을 지정한다

```CSS
body{
backgorund-colorL lightblue;
}
```

body이외에 다른 HTML요소에서도 배경색을 지정 할 수 있다.

opacity속성은 투명도를 지정한다

1일수록 불투명하고 0일수록 투명해진다

```CSS
body{
background-color:black;
opacity:0.5;
}
```

opacity속성을 사용할 필요 없이 rgba값을 사용하는것도 가능하다

# Background Image
-------------------
background-image 속성은 요소에 삽입할 이미지를 지정한다

```CSS
body{
background-image:url("paper.gif");
```

이미지는 기본적으로 텍스트등 요소를 대부분 가린다

# Background Repeat
-------------------
기본적으로, background-image속성은 가로,세로로 반복한다

일부이미지는 가로,또는 세로방향으로만 반복해야한다

이미지를 가로로만 반복하려면 background-repeat-x; 속성을 추가한다

반대로 세로로만 반복하려면 background-repeat-y; 를 추가한다

배경이미지 반복이 필요 없다면 no-repeat를 추가한다

이미지의 위치를 지정할 때는 background-position속성을 추가한다

```CSS
body{
background-image:url("tree.png");
background-repeat-no-repeat;
background-position: right;
}
```
# Background Attachment
---------------------
Background-attachment속성을 사용하면 이미지를 스크롤할지 고정할지 선택할 수 있다

고정하고싶다면 fixed 스크롤하고싶다면 scroll을 사용하면 된다

```CSS
body{
background-image:url("tree.png");
background-repeat-no-repeat;
background-position: right;
background-attachment:fixed;
}
```

# Background Shorthand
-------------------
하나의 속성에 배경속성을 모두 넣을 수 있다.

```CSS
body{
background-image:url("tree.png");
background-repeat-no-repeat;
background-position: right;
background-attachment:fixed;
}
```

```CSS
body{
background url("tree.png") no-repeat fixed right top ;
}
```

줄여쓰기를 사용할 때 순서는

color > image > repeat > attachment > position 순서다

반드시 5개를 모두 사용해야 하는것은 아니다.
