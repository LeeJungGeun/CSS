# CSS Inline- block
-------------------------

inline과  inline-block의 가장 큰 차이점은 크기를 조절할 수 있는지 없는지의 차이일 것이다

또한, inlink-block은 top과 bottom의 margin/padding이 존중받는다, inline은 그렇지 않다

block과 inline-block의 가장 큰 차이점은 강제 줄바꿈을 하지 않는다는 점이다

```css
span.a {
  display: inline; 
  width: 100px;
  height: 100px;
  padding: 5px;
  border: 1px solid blue;
  background-color: yellow;
}

span.b {
  display: inline-block; 
  width: 100px;
  height: 100px;
  padding: 5px;
  border: 1px solid blue;
  background-color: yellow;
}

span.c {
  display: block; 
  width: 100px;
  height: 100px;
  padding: 5px;
  border: 1px solid blue;
  background-color: yellow;
}
```

inline은 크기조절이 불가능하며

block은 줄바꿈이 불가능

inline-block은 줄바꿈과 크기조절 둘 다 가능하다

inline-block은 항상 항목을 가로로 표시한다
