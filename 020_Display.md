# CSS Pisplay
-----------------
display 속성은 가장 중요한 CSS 레이아웃 컨트롤속성이다

display속성은 요소들이 화면에 어떻게 나오는지 결정한다

모든 html 요소는 요소 유형에 따라 display 디폴트값을 가지고있다

대부분의 디폴트값은 block과 inline이다

# block-level Elements
--------------------
block-level의 요소는 항상 새로운 줄에서 시작하며

사용 가능한 가로넓이 전체를 사용한다

block-level 요소는 다음과같다

- \<div>
- \<h1> ~ \<h6>
- \<p>
- \<form>
- \<header>
- \<footer>
- \<section>

# inline Elements
----------------------

인라인 요소는 새로운줄에서 시작하지 않으며 필요한 만큼의 가로넓이만 사용한다

inline 요소는 다음과 같다

- \<span>
- \<a>
- \<img>

# Display: none
----------------------
Display: none; 명령어는 자바스크립트를 사용해 요소를 삭제하거나 다시만들지 않고 그것들을 보이지않게 감추는 역할을 한다

\<script>요소는 기본적으로 display:none; 이 사용된다

# Override Default Value
----------------------
모든 요소에는 디폴트값이 정해져있지만 이것을 무시하는것도 가능하다

block요소를 inline 요소로 바꾸거나 반대로 inline요소를 block요소로 변경하면

페이지를 특정 방식으로 보이는데 유용하게 할 수 있으며, 웹 페이지의 표준을 지킬 수 있다.

```css
li {
  display: inline;
}
```

```css
a {
  display: block;
}

```

\<li>를 인라인요소로 만들거나

\<a>를 블록요소로 만드는 것이 가능하다

# display:none, visible:hidden
----------------------------

요소를 숨기는 방법은 visible:hidden과 display:none; 이 있다

visible:hidden 은 요소를 숨지만 요소가 사용하던공간은 빈공간으로 두어서 레이아웃을 계속 차지한다

display:none; 은 요소를 숨기며 해당 요소가 없는것처럼 페이지를 사용한다

```css
h1.none {
  display: none;
}

h1.hidden {
  visibility: hidden;
}
```
