# CSS Box Model
-------------
모든 HTML의 요소는 상자로 간주될 수 있다.

CSS에서 box model 은 디자인과 레이아웃에서 사용되는 말이다.

CSS box model은 HTML요소를 둘러싼 상자다

margin, border, padding, 컨텐츠가 포함된다

- 컨텐츠 : 주요내용
- padding : 컨텐츠와 테두리 사이의 여백
- border : 테두리
- margin : 해당 테두리와 다른 테두리 사이의 여백

모든 브라우저에서 요소의 넓이와 높이를 표현하기 위해선 box model의 작동방식을 알아야한다

```CSS
div {
  width: 320px;
  padding: 10px;
  border: 5px soild black;
  margin: 5px;
}
```
해당 예시에서 컨텐츠의 넓이는 320 px

테두리는 5px의 검정색실선이고

컨텐츠와 테두리 사이엔 10px의 여백이있으며

다른 컨텐츠의 테두리와의 여백은 최소 5px이 주어진다
