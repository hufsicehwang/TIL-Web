🦁TIL-16🦁

# 중앙 정렬하는 두가지 방법

# 1
```css
  display: flex;
  justify-content: center;
  align-items: center;
```
- `justify-content` = 수평 정렬, ` align-items` = 수직 정렬
- 하지만 display가 flex이기 때문에 요소가 많을 수록 원하는 것과 다르게 정렬된다.

# 2
```css
  display: inline-block;
  text-align: center;
```
- ` text-align`는 text만 해당하는 속성 같지만 이미지에도 적용 된다.
- div의 한 계단 한 계단 속성에 부여하면 중앙 정렬이 가능하다.
   
