# CSS Opacity
---------------
CSS에서 Opacity 속성은 해당 요소의 투명도/불투명도를 정의한다

투명도는 0부터 1 사이의 숫자로 조정할 수 있다

```css
img {
  opacity: 0.5;
}
```

hover의사클래스를 사용하여 마우스 위치에 따라 투명도를 조절하는것도 가능하다

```css
img {
  opacity: 0.5;
}

img:hover {
  opacity: 1;
}
```
opacity속성을 자식요소에 상속시키면 해당 요소도 투명도를 부여받는다

```css
div {
  background-color: #4CAF50;
  padding: 10px;
}

div.first {
  opacity: 0.1;
}
```

이렇게 작성할 경우 first클래스에선 텍스트까지 투명해진다

그걸 원치 않을경우 opacity속성보단 background에 rgba속성을 넣자

```css
div {
  background: rgba(76, 175, 80, 0.1)
}
```
rgba는 배경색만 투명하며 나머진 변하지않는다

div자체에 opacity속성을 줄 경우 컨텐츠까지 모두 투명해지기에 주의가 필요하다
