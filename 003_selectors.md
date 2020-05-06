# CSS 선택자
------------------
CSS선택자는 원하는 스타일의 HTML요소를 찾는데 사용된다

CSS선택자를 5개 범주로 나눌 수 있다.

- simple selectors (이름 아이디 클래스기준으로 요소선택)
- combinator selectors (요소사이에 특정 관계에 따라 요소 선택)
- pseudo-class selectors (특정 상태에 따라 요소 선택)
- pseudo-elements seletors (요소의 일부를 선택하고 스타일 지정)
- attribute selectors (속성이나 속성값에 따라 요소 선택)

# CSS 요소 선택자
-------------------

요소 이름을 기반으로 요소를 선택

# CSS id 선택자
-------------------
id 선택자는 HTML 요소의 id 속성을 사용하여 특정 요소를 선택

요소의 id는 페이지내에서 무이한 값을 갖고있으며 id선택자는 고유id값을 선택한다

특정 id를 가진 요소를 선택하려면 '#'을 사용한다

```CSS
#para1 {
  text-align: center;
  color: red;
}
```

# CSS class 선택자
------------------------

클래스 선택자는 특정 클래스의 HTML요소를 선택한다

특정 크래스를 가진 요소를 선택하려면 '.'을 사용한다

``` CSS
.center {
  text-align: center;
  color: red;
}
```

특정 요소만 지정받도록 할 수 있다.

```CSS
p.center {
  text-align: center;
  color: red;
}
```

둘 이상의 클래스를 참조할 수 있다.

```CSS
<p class="center large">This paragraph refers to two classes.</p>
```

# 유니버셜 선택자

'*'을 사용하면 페이지 내의 모든 요소를 선택 할 수 있다.

```CSS
* {
  text-align: center;
  color: blue;
}
```

# CSS 그룹 선택기
--------------------

그룹선택기는 동일한 스타일정의를가진 요소를 선택한다

```CSS
h1 {
  text-align: center;
  color: red;
}

h2 {
  text-align: center;
  color: red;
}

p {
  text-align: center;
  color: red;
}
```

```CSS
h1, h2, p {
  text-align: center;
  color: red;
}
```

두개의 예시는 결과가 같다.
