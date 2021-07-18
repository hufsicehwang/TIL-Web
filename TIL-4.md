🐳TIL-4🐳

## 🐬CSS 기본 문법 (속성:값)
```css
div {
  font-size: 20px;
  color: red;
}

/* 다음과 같이 이해할 수 있습니다. */
선택자 {
  속성: 값;
  속성: 값;
}
```
1. __선택자는 태그를 뜻함!!__
2. 속성은 부여하고 싶은 특징을 뜻함!!
3. 값은 특징의 범위 해당 값을 뜻함!!

## 🐬HTML에 적용 예시
```HTML
// HTML 코드 부분
<div>
  <h1>제목..</h1>
  <p>본문..</p>
</div>

// CSS 코드 부분
h1 {
  color: red;
}
p {
  color: blue;
}
```
동일하게 CSS 선택자 = HTML 태그

## 🐬CSS 선언 방식
### 1.태그에 직접 작성하기 (비추x)
```html
<div style="color: red;">태그에 직접 작성1</div> <!-- red -->
```

### 2.HTML에 포함하기 


![image](https://user-images.githubusercontent.com/67450413/117167484-41151380-ae02-11eb-8bde-b31e063c4f94.png)


__head는 정보의 범위인데, <style>은 css 정보를 나타내는 태그 임으로 head 안에 포함!!!__
  
### 3.HTML 외부애서 불러오기 (추천, 가장많이 쓰임)
```html
<head>
  <link rel="stylesheet" href="/css/main.css">
</head>
<body>
  <div>HTML에 외부에서 불러오기1</div> <!-- red -->
</body>
```
link는 외부에서 파일 불러오기, __rel="stylesheet"__ 는 CSS를 뜻함, __href="/css/main.css"__ 는 해당 CSS파일 경로
-> <div>의 컨텐트의 텍스트를 빨간색으로 하고 싶다면 해당 CSS 파일의 형태는?? 충분히 유추가능~
  
## 🐬CSS 선택자
### 1. 태그로 찾기
```CSS
/*<h1>은 글자색이 빨강이야!*/
h1 {
  color: red;
}
/*<p>는 글자색이 파랑이야!*/
p {
  color: blue;
}
------------------
<h1>제목1</h1> <!--red-->
<p>본문2</p> <!--blue-->
```
단순 태그 이름으로 적용하기-> 가능은 하지만 특정 태그를 지정하는데 한계가 있음

### 2. 클래스로 찾기
```css
/*class="title"은 글자색이 빨강이야!*/
.title {
  color: red;
}
/*class="main-text"는 글자색이 파랑이야!*/
.main-text {
  color: blue;
}
----------------------------
<h1 class="title">제목1</h1> <!--red-->
<h1>제목2</h1>
<p class="main-text">본문1</p> <!--blue-->
<p>본문2</p>
```
태그에 클래스(별칭)을 부여함으로써 좀더 개별적으로 인식 가능!    
