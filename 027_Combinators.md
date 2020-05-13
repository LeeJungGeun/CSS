# CSS Combinator
-----------------------
Combinator는 selector간의 관계를 설명한다

CSS Selector는 간단한 선택기를 포함할 수 있다

combinator는 두 선택기 사이에 포함된다

# Descendant Selector
----------------------------

descendent selector는 지정된 모든 자손요소와 매치한다

```css
div p {
  background-color: red;
}
```
위 예시의 경우 div안에있는 p에 속성이 들어갈 뿐

p가 div밖에 있으면 속성이 안들어간다

# child seletor
-------------------
자식선택자는 지정된 모든 자식요소와 매치된다

```css
div > p {
  background-color: red;
}
```

위 예시의 경우 div 안에있는 p에는 속성이 들어가며

div밖에있으면 속성이 안들어갈 뿐 아니라

div안에있는 section 안에있는 p에도 속성이 안들어간다

# Adjacent Sibling Selector
---------------------------------
근접 형제 선택자의 경우 동일한 부모를가진 가장 가까운 요소에 속성을 준다

```css
div + p {
  background-color: red;
}
```

div내에는속성이 들어가지 않고

div의 밖에서 div가 끝나고 가장 먼저나온 p에 속성을 주며

그 다음에나오는 p에는 속성이 들어가지 않는다

# General Sibiling Selector
-----------------------------
일반 형제선택자의 경우 

같은부모를 가진 요소에 속성을 준다

```css
div ~ p {
  background-color:red;
}
```
div가 끝난 다음 p 요소가오면 모두 속성을 준다
