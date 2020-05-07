# CSS Color
------------------
색상은 사전정의된 색상의 이름이나 RGB, HEX, RGBA, HSLA값으로 정의된다

```CSS
<h1 style="background-color:Tomato;">Tomato</h1>
<h1 style="background-color:Orange;">Orange</h1>
<h1 style="background-color:DodgerBlue;">DodgerBlue</h1>
<h1 style="background-color:MediumSeaGreen;">MediumSeaGreen</h1>
<h1 style="background-color:Gray;">Gray</h1>
<h1 style="background-color:SlateBlue;">SlateBlue</h1>
<h1 style="background-color:Violet;">Violet</h1>
<h1 style="background-color:LightGray;">LightGray</h1>
```
CSS에서 지원하는 색상의 갯수는 140가지이다

# Background
--------------
html요소의 배경색을 지정 할 수 있다.

```CSS
<h1 style="background-color:DodgerBlue;">DodgerBlue</h1>
<p style="background-color:Red;">Red</p>
```

# CSS TextColor
--------------------
텍스트의 컬러를 지정 할 수 있다

```CSS
<h1 style="color=Tomato;">Textcolor</h1>
<p style="color=Blue;">Textcolor</p>
```

# CSS BorderColor
-----------------
테두리의 색을 지정할 수 있다

```CSS
<h1 style="border:2px solid red;"> border</h1>
<p style="border 2px solid blue;"> bordercolor</p>
```

# colorvalue
----------------
RGB, HEX, HSL, RSBA, HSLA값을 직접 줄 수 있다

투명도 조절도 가능하다

```CSS
<h1 style="background-color:rgba(255,0,0,0.5);">0.5 red</h1>
<p style="background-color:hsla(0,0,100%,0.5);">color 0.5</p>
```

# RGB
-----------------
rgb값을 줄땐 색상을 입력하는 부분에 rgb(r:g:b)에 값을 주면 된다

```CSS
<h1 style="background-color:rgb(255.255.0);">RGB</h1>
```

회색 음영계열은 rgb값이 모두 같을 때 자주 나타난다

```CSS
<h1 style="background-color:rgb(120,120,120);">background</h1>
```

투명도를 줄 때는 rgba를 사용한다

color:(r,g,b,투명도) 형식으로 사용되며

투명도는 0에서 1 사이의 숫자가 사용된다

```CSS
<h1 style="background-color:rgba(255,0,0,0.5);">투명도 0.5</h1>
```

# HEX
-----------------
rgb값을 0-255가 아닌 16진수로 나타낸 방식이다

color:#rrggbb 형식으로 사용된다

```CSS
<h1 style="background-color:#ff0000;">style</h1>
```
# HSL
--------------------
HSL 방식으로 색상을 나타내는것도 가능하다

HSL(색조,채도%,밝기%) 형식으로 사용된다

```CSS
<h1 style="background-color:HSL(180,100%,50%);"> HSL </h1>
```

색조는 0에 가까울수록 회색빛이 나고

밝기는 0일경우 검정 100일경우 흰색이 된다

채도와 색조를 0으로하고 밝기만 조절하면 회색음영색을 만들 수 있다

HSL도 RGB와같이 투명도 조절이 가능하며

HSML을 사용한다

HSML(색조, 채도%, 밝기%, 투명도) 형식을 사용하며

투명도는 0에서 1사이의 숫자를 사용한다

```CSS
<h1 style="background-color:HSLA(0,100%,50%,0.5);"> 0.5 hsla</h1>
```
