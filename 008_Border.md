# CSS Border
--------------

CSS border의 속성을 사용하면 선스타일, 색상, 굵기 등을 설정할 수 있다

# border Style
-----------------
border-style 속성으로 선 스타일을 정의할 수 있다.

- dotted : 점선
- dashed : 파선
- solid : 선
- double : 이중선
- groove : 3D 그루브 효과
- ridge : 3D 바깥테두리 효과
- inset : 음푹 파인 효과
- outset : 튀어 나와있는 효과
- none : 효과 없음
- hidden : 투명선
- mix : 상 우 하 좌 순서로 지정하며 위에 속성들을 섞는 효과

```CSS
p.one {
  border-style:solid;
}

p.two {
  border.style:dashed;
}
```

# Border Width
-----------------
border-width속성을 사용하면 선의 굵기를 조절 가능하다

in. px. pt. cm, em, etc의 단위를 사용하거나 thin, medium, thick의 사

```CSS
p.one {
  border-style:solid;
  border-width:5px;
}

p.two {
  border style : solid;
  border-width:thin;
}
```

border-width 속성은 상 우 하 좌 순서로 섞어서 사용 가능하다

```CSS
p.border {
  border-style:solid;
  border-width: 5px 10px 15px 20px;
}
```

# border color
-------------------
border-color 속성을 사용해 테두리의 색상을 지정할 수 있다

색상은 사전정의된 이름, hex, rgb, hsl 값을 사용 가능하다

```CSS
p.one {
  border-style:solid;
  border-color:red;
}

p.two {
  border-style:dotted;
  border-color:hsl(0,0%,0%);
}

p.three {
  border-style:double;
  border-color:#ffff00;
}
```

# Border Sides
---------------
mix속성으로 선을 섞을 수도 있지만

테두리의 각각의 부분을 위한 속성도 있다.

```CSS
p {
  border-top-style:dotted;
  border-right-style:solid;
  border-bottom-style:none;
  border-left-style:solid
}
```

각각의 속성을 저장할 때 반드시 4가지를 모두 적용할 필요는 없다

```CSS
p {
  border-style: dotted solid double dashed;
}

p {
  border-style: dotted solid double;
}

p {
  border-style: dotted solid;
}

p {
  border-style: dotted;
}
```
위를 예로들어

4가지 모두 작성괸경우 상 우 하 좌 순서로 적용되며

3가지가 작성된경우 상 좌우 하 로 적용

2가지가 작성된경우 상하,좌우로 적용되고

1가지가 작성된경우 상하좌우전부 적용된다.

# Border- shorthand
-------------------
테두리도 배경과같이 속성 줄여쓰기가 가능하다

```CSS
p {
  border: 5px solid red;
}
```

# Rounded Border
---------------------

border-radius 속성을 사용하면 테두리를 둥그렇게 만드는것이 가능하다

```CSS
p {
  border: 5px solid red;
  border-radius: 12px;
}
```
