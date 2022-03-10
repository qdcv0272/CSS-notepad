# Css 선택자 알아보기 Part1
___

* 기본 선택자
* 복합 선택자
___
# ex) HTML
```html
<div>
    <ul>
      <li>강아지</li>
      <li class="cat">고양이</li>
      <li>거북이</li>
    </ul>
    <div>까치</div>
    <p id="fish" class="fish">물고기</p>
    <span class="tiger">호랑이</span>
</div>
```
___
```html
<div>
  <ul>
    <li >강아지</li>
    <li class="cat">고양이</li>
    <li>거북이</li>
  </ul>
  <div>호랑이</div>
  <p>사지</p>
  <span class="cat">고양이</span>
</div>
<span class="cat">고양이</span>
```


___
# 기본 선택자

### * (에스터리크) : Universal Selector

```
* {}
```
HTML 에서 모든 요소를 선택
___
### Type Selector : 태그 이름인 li 인 요소 선택
```
li {}
```
___
### Class Selector : HTML **class 속성의 값이** fish 인 요소 선택
```
.fish {}
```
___
### ID Selector : HTML id 속성의 값이 fish 인 요소 선택 
```
#fish {}
```
___
# 복합 선택자

### Basic Combinator : 선택자 span와 tiger 를 동시에 만족하는 요소 선택
```
span.tiger {}
```
___
### Child Cpmbinator : 선택자 ul 의 자식 요소 .fish 를 선택 

```
ul.cat {}
```
___
### Descendant Combinator : 선택자 div의 하위 요소 cat 을 선택 ✩ 띄어쓰기가 선택자의 기호 !✩
```
div .cat{}
```
___
### Adjacent Sibling Combinator : 선택자 .cat 의 다음 형제 요소 li 하나를 선택
```
.cat + li{}
```
___
### General Sibling Combinator : 선택자 .cat 의 다음 형제 요소 li 모두를 선택
```
.cat ~ li{}
```
