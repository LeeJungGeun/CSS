# CSS Text
-------------------
CSS에서 Text에 줄수 있는 속성은 6가지가 있다

- color : 색상
- alignment : 정렬
- decoration : 장식
- transfomation : 영대소문자 
- spacing
- shadow

# Text Color
------------------

color속성을 사용하면 문자에 색을 입힐 수 있다

색을 입히는 방법은 rgb방식, 16진수방식, 사전정의된 이름 방식이 있다

```CSS
body {
  color: blue;
}

h1 {
  color : #FF0000
}
```

문자에 배경색을 줄 경우 문자가 있는 부분에만 배경색이 들어간다
```CSS
body {
  backgrond-color: red;
  color:  #000000;
}
```

# Text Alignment
--------------------
text-alignment속성은 텍스트를 가로정렬 하는데 사용된다

left, right, center값으로 각 좌정렬, 우정렬, 가운데정렬이 가능하다

```CSS
p1 {
  text-alignment: center;
}
```
justflt 값을 사용하면 모든 줄의 넓이가 같은 직사각형 형태로 텍스트가 정렬된다

```CSS
div {
  text-alignment: justfly;
}
```

vertical-align 속성을 사용하면 세로 정렬이 가능하다

```CSS
img {
  vertical-align: top;
}
```
텍스트를 입력하기에 위,아래 여백이 많을 경우에 그 여백공간을 활용할 뿐

페이지 전체에서 세로정렬 하는 기능은 아니다.

# Text Decoration
------------------
텍스트에 장식을 넣는 속성

```CSS
h1 {
  text-decoration: overline;
}

h2 {
  text-decoration: underline;
}
```

각각 윚줄, 아랫줄의 장식을 넣은 예시이다

# Text Transfomation
----------------------
text-transformation은 영대,영소문자를 바꾸는 기능이다

```CSS
p.uppercase {
  text-transform: uppercase;
}

p.lowercase {
  text-transform: lowercase;
}

p.capitalize {
  text-transform: capitalize;
}
```

각각 영대문자로 변환, 영소문자로변환, 각 단어의 첫글자를 대문자로 변환 

# Text Spacing
---------------
text-indent속성을 이용하면 들여쓰기를 할 수 있다

```CSS
p {
  text-indent: 50px;
}
```

letter-spacing 속성은 문자간의 가로 간격을 조절하는 속성이다

음수가 가능하며 음수로 설정하면 글자가 겹친다

```CSS
h1 {
  letter-spacing: 3px;
}

h2 {
  letter-spacing: -3px;
}
```

line-height 속성을 사용하면 줄 높이 간격을 조정할 수 있다

h1 {
  line-height: 0.8;
}

h2 {
  line-height: 1.8;
}
참고로 위에 값은 백분율이다

word-spacing속성을 사용하면 단어 사이의 간격을 조정 할 수 있다

```CSS
h1 {
  word-spacing: 50px;
}
```

# Text Shadow
----------------

문자에 그림자를 추가하는 속성이다

W3스쿨에선 가로세로 2px이 가장 무난하다고 한다

```CSS
h1 {
  text-shadow: 2px 2px;
}
```

그림자에 색을 입힐 수 있다

```CSS
h1 {
  text-shadow: 2px 2px red;
}
```

픽셀 3개를 지정하면 그림자가 번지는 범위를 지정할 수 있다

색이 멀리번지면 색이 옅어진다
```CSS
h1 {
  text-shadow: 2px 2px 10x red;
}
```
