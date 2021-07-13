🐳TIL-5🐳

## 🦁여러가지 속성
```css
.box{
    width: 100px;
    height: 70px;
    background: red;
    font-size: 16px;
    margin: 20px;
    padding: 20px;
}
```
- .box는 클래스 이름으로 찾는 방법임!
- 단위는 px
- 그냥color 속성이 텍스트 색깔임!! (HTML의 content 부분)

## 🦁코드 확인 방법

![image](https://user-images.githubusercontent.com/67450413/117403217-cb649100-af42-11eb-9210-d7ac829e38b4.png)

- 이와 같이 live server를 이용한 후 웹에서 `F12` 개발자 모드 누르면 확인 가능!
- 내가 평상시 보고 괜찮다고 생각한 디자인이나 색상 조합 확인 가능하다는게 최대 장점!

## 🦁특이한 속성
### 1. 수평
```css
.clearfix::after{
    content: "";
    display: block;
    clear: both;
}    
```
얘를 하고 `1. HTML 클래스에 clearfix 추가` , `2. css 선택자 안에 float: left;` 하면 수평으로 보이게 만들 수 있음

### 2. 실선
`border-bottom: 1px solid lightgray;`

### 3. 특이하게 선택자 선택하는 법
```css
.logo img {
    display: block;
}
```
-> .logo 클래스 안에 있는 img 태그만 지정해 줌!
