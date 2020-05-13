# CSS Align
------------------------
\<div>같은 블록요소를 가운데정렬 하려면 margin:auto를 사용한다

```css
div {
  margin: auto;
  width: 50%;
  border: 1px solid black;
}
```
width속성이 없거나 100%라면 세로 가운데정렬은 효과가없다

텍스트를 요소의 가운데에 정렬할때는 text-align: center; 를 사용한다

```css
div {
  text-align: center;
  border: 1px soild black;
}
```

센터에 이미지를 놓으려면 오른쪽과 왼쪽에 margin: auto를 넣고 블록요소로 만든다

```css
img {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width:50%;
}
```
요소를 정리하는 메소드 position: absolute;는 요소의 포지션을 조정한다

```css
div {
  position: absolute;
  right: 0px;
  width: 200px;
  border: 1px solid black;
}
```

비슷한 방법으로는 float속성이 있다

```css
div {
  float: right;
  width: 200px;
  border: 1px solid black;
}
```
요소보다 컨텐츠가 더 많고 부동상태인 경우 오버플로우되며

clearfix를 사용할 수 있다

```css
div {
  overflow: auto;
}
```
css를 사용해 세로정렬 하는방법은 여러가지있다

그중 하나는 padding을 사용하는것이다

또 다른 방법은 line-height속성을 사용하는 것이다

두가지 방법 말고도  transform속성을 사용하는 방법도 있다

```css
p {
  margin: 0px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```

마지막으로  flexbox를 사용하는 방법이 있다

이 방법은 IE10이하버전에선 지원하지 않는다

```css
div {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 200px;
  border: 1px solid black;
}
```
