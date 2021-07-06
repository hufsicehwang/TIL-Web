🐼TIL-13🐼

# px, em, rem 단위
- px: 고정적인 단위로써 최상위 부모에게 부여하자
- em: 부모에게 상속 받은 px 크기 만큼에서 `배수`를 한다.
- rem: root em으로써 가장 조상 즉, `html`태그의 폰트 사이즈를 기준으로 `em(배수)` 한다.

# width, heigth 기본값
```css
div{
width : auto;   // 100%
height: auto;     //  0
}
```
- div는 디자인적으로 사용하자.
```css
span{
width : auto;   // 0
height: auto;     //  0
}
```
- span은 width, height를 가질수 없다. 텍스트적으로 사용하자.

# margin
- margin: 10px;  -> 위,아래,좌,우 10px
- margin: 20px 10px;   ->  [위,아래]:20p ,  [좌,우]: 10px

# border
- `border: 두께 종류 색상`
```css
.box{
border: 1px solid red
border-radius: 10px // 모서리 깍임
}
```
: 1px 두께로 실선을 빨간색으로 만든다.
- 종류 속성의 값들 : solid(실선), groove(파여있는 선), ridge(솟은 모양 선), inset(요소 전체가 들어간 모양), outset(요소 전체가 나온 모양)
- 색상 속성의 값 : transparent (투명한 실선)

# box -shadow
: 그림자 만들어주는 
 
