# CSS Position
------------------

position 속성은 요소의 위치를 지정하는 속성이다

5가지 값이 있다

  - static
  - relative
  - fixed
  - absolute
  - sticky
  
속성값을 준 다음 top bototm left right로 위치를 지정한다

# static
----------------------
정직인 포지션

top bottom right left의 영향을 받지 않는다

position: static 속성은 특별한 값을 받지 않으며 페이지의 흐름에 따라 지정된다

```css
div {
  position: static;
  border: 1px solid black;
}
```

# relative
-------------
상대적 포지션의 요소

top bottom left right 속성을 주게되면 속성을 준 방향으로부터 해당 공간만큼 멀어진다

```css
div {
  position: relative;
  left: 50px;
  border: 1px solid black;
}
```

# fixed
--------------------
뷰포트를 이용한 화면에 고정하는 요소

휠을 돌리거나 해도 위치를 고정시킨다

 top bottom right left 속성을 주게되면
 
 해당방향으로 밀착하며 값을 주게된 거리만큼 떨어져있는다
 
 ```css
 div {
  position: fixed;
  top: 100px;
  right:0px;
  border: 1px solid black;
 }
 ```

# absolute
------------------
절대 위치 요소

절대적인 위치로 자리잡긴 하지만

뷰포트 기준이아닌 가장 가까운 조상 요소에 위치한다

```css
div.relative {
  position: relative;
  width: 400px;
  height: 200px;
  border: 1px solid black;
}

div {
  position: absolute;
  top : 0px;
  right: 0px;
  width: 200px;
  height: 100px;
  border: 1px solid red;
}
```

# sticky
-----------------
스크롤을 기준으로 고정되는 요소

스크롤이 원래의 위치를 보여줄 수 있다면 상대적인 포지션이며

스크롤이 원래의 위치를 보여줄 수 없을땐 고정되는 포지션

고정되는 위치는 top bottom left right중 하나를 지정해야한다

사파리 브라우저에선 -webket-접두사가 필요하다
```css
div {
  posotion: sticky;
  top 0;
  background-color:green;
  border: 1px soild red;
}

```

# z-index
-----------------
요소를 배치하다보면 요소가 겹칠 수 있다

요소가 겹칠 때 z-index 속성을 사용하면 요소를 표시하는 순서를 조정한다

```css
img {
  position: absolute;
  left: 0px;
  top: 0px;
  z-index: -1;
}
```

이미지파일의 z-index값이 -1이므로 다른 요소와 겹쳤을 때 해당 이미지는 다른요소보다 뒤쪽에 
