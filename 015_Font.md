# CSS Font
--------------

글꼴 속성은 글자의 글꼴, 굵기, 크기, 스타일을 정의한다

# Font Family
----------------
텍스트의 글꼴은 font-family속성으로 설정한다

이 속성에는 대체시스템으로 여러 글꼴을 가지고 있어야 한다

브라우저가 글꼴을 가지고있지 않으면 다음 글꼴을 시도한다

글꼴을 사용할 수 없는경우 일반 글꼴을 사용한다

# Font style
---------------

font-style 속성은 글자를 기울이는데 사용한다

값에 normal을주면 기울이지 않고 italic을 주면 기운다
```CSS
p {
  font-style: italic;
}
```

font-weight 속성은 글자의 굵기를 조정한다

```css
p {
  font-weight: bold;
}
```

font-variant 속성은 대문자를 작게 나타내는데 사용한다

첫글자는 일반적인 크기이며 2번째 글자부터 글자가 작아진다

값은 small-cap을 사용한다

```CSS
p {
  font-variant: small-cap
}
```

# font size
------------------
font-size속성은 텍스트의 크기를 설정한다

크기를 조정 할 수는 있지만 제목에는 <h>태그 내용에는 <p>태그가 권장된다

```CSS
h1 {
  font-size 40px;
}

p {
  font-size: 14px;
}
```

HTML은 글꼴을 em단위를 권장하며 백분율도 사용 가능하다

font-size를 vw단위로 사용할 경우

웹 브라우저 크기에 따라 다른 글자 크기가 나온다

```CSS
<h1 style="font-size:10vw">
```

# 구글 폰트
----------------

<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">

위 링크를 추가하면

구글이 지원하는 수백가지 글꼴을 불러 올 수 있다.

```HTML
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
<style>
body {
  font-family: "Sofia";
  font-size: 22px;
}
```

# font shorthand
--------------
폰트도 다른 속성들처럼 줄여쓰기가 가능하다

style, variant, weight, size, line-height, family값이 조정 가능하다
