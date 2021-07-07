🦁TIL-15🦁

# HTML에 Animation 적용 하는 방법!
### 1. https://animate.style/ 접속
### 2. head 태그에 link 연결하기
```html
<head>
  <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css"/>
</head>
```
### 3-1. 클래스 이름으로 설정하기
```html
<h1 class="animate__animated animate__bounce">An animated element</h1>
```
- `animate__animated animate__bounce`와 같이 class를 정의 해야한다.
- 마지막의 `bounce` 부분을 원하는 animation으로 적용한다. 

### 3-2. CSS로 적용하기
```css
.my-element {
  display: inline-block;
  margin: 0 0.5rem;

  animation: bounce; /* 애니메이션 종류 설정 */
  animation-duration: 2s; /* 지속시간 설정 */
  animation-delay: 1s; /* 지연시간 설정 */
}
```
- 지연, 지속 기간을 설정 할 수 있다.
