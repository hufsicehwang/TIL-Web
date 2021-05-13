🦄TIL-6🦄

# 블록 레벨 요소
: DIV, H1, P 등이 있다.
1. 사용 가능한 최대 가로 너비를 사용한다.
    - __사용자가 가로,세로를 지정 할 수 있다.__
2. 수직으로 쌓인다.
3. margin, padding을 상,하,좌,우 로 컨트롤 가능
4. 레이아웃 용도로 이용하자!


  - css에서 초기화 시켜줘야함
    - ```css
        body{
         margin: 0;
         padding: 0;
         }
      ```
      
# 인라인 요소
: SPAN, IMG 등이 있다.
1. 필요한 만큼 너비를 사용한다.
    - __사용자가 가로, 세로를 지정 할 수 없다.__
2. 수평으로 쌓인다.
3. margin, padding을 좌,우 만 컨트롤 가능
4. text를 다룰 때 사용하자!

# 요소간 이동하기
: css에서 display 속성을 이용하여 요소를 변경 할 수 있다.
```css
div{
    background: red;
    height: 20px;
    display: inline;
}
```
🔼 블록 요소를 인라인 요소로 변경 할 수 있다.

```css
span{
    background: red;
    height: 20px;
    display: block;
}
```
🔼 인라인 요소를 블록 요소로 변경 할 수 있다.

# Meta data
:  `<base>, <link>, <script>, <style>, <title>`과 같은 다른 메타관련 요소로 나타낼 수 없는 메타데이터를 나타낸다.
- `charset` 속성은 문자 인코딩 방식을 지정하는데, 일반적으로 UTF-8로 사용한다. 다른 인코딩 방식 사용시 한글 깨짐 현상 일어날 수 있음.
- `http-equiv` 속성은 익스플로어에서 뭐 똑같이 보여지는데에 쓰임

# Base tag
: 상대경로의 시작 위치를 지정해주는 태그
- 하나 밖에 사용 못함





## Tip
html 요소 참고 사이트
https://developer.mozilla.org/ko/docs/Web/HTML/Element
