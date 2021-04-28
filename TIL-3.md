🐳TIL-3🐳

## HTML 기초 문법

# TAG
- 태그는 각자의 의미를 가지고 있으며 
```html
<TAG></TAG>
<TAG>CONTENT</TAG>
```
다음과 같이 표현된다.
- 태그는 /(슬래시)가 붙은 것과 붙지 않은 한 쌍의 태그를 가지는 것이 일반적이다.

# Enpty Tag
- 태그가 한쌍으로 이루어지지 않고 하나의 형태로만 이루어 져 있을때를 말한다.
```html
<!-- `/`가 없는 빈 태그 -->
<TAG>

<!-- `/`가 있는 빈 태그 -->
<TAG/>
<TAG />
```
- 버전마다 빈태그의 형식이 다르지만 HTML5부터는 모두 사용가능하다.
- 다만 html5로 사용시 빈태그를 하나의 형식으로 작성해 주는게 제일 좋다!

# 속성(Attributes)과 값(Value)
- tag의 형태를 변형해 추가적인 확장 기능을 수행 할 수 있다.
```html
<img src="./my_photo.jpg" alt="내 프로필 사진" />
<div class="name">홍길동</div>
```
- 1. img는 src,alt와 같은 속성을 가지고 해당 값을 가진다.
- 2. div는 class라는 속성과 값을 가지고, 홍길동이라는 content를 가진다.

# HTML 구조
### head, body, DOCTYPE
```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="author" content="홍길동">
    <meta name="description" content="우리 사이트가 최고!">
    <title>내 사이트</title>
    <link rel="stylesheet" href="./css/main.css">
    <script src="./js/main.js"></script>
</head>
<body>
    <section>
      <h1></h1>
      <div>
      </div>
    </section>
</body>
</html>
```
- DOCTYPE은 웹 브라우저에 제공할 HTML버전을 설정하는 것으로 `<!DOCTYPE html>` 은 가장 최신 HTML5를 제공한다.
- `<html>`은 웹브라우저가 해석할 HTML의 가장 큰 범위를 말한다.
- `<head>`는 HTML 문서의 정보 범위를 지정한다. 쉽게 말해 화면을 구성하기 위한 기본 설정이다.
- `<body>`는 HTML 문서의 구조 범위를 지정한다. 쉽게 말해 내용적인 content를 지정한다.

# HTML 문서의 정보 (head)
- head 부분에 쓰는 정보(태그)들을 알아보자
  - ' <title>네이버</title>' 웹 브라우저의 각 사이트 탭에서 이름을 나타낸다.
  - '<meta charset="UTF-8">' 문자 인코딩 방식을 말하는데, 그냥 무조건 써야한다.
  - '<meta name="author" content="홍길동">' name은 검색 엔진을 제공하는 정보, content는 해당 name의 값을 제공한다.
  - '<link rel="stylesheet" href="./css/main.css">' link는 현재 문서에 css 문서를 연결할때 쓰인다.
    - rel은 현재 문서와 외부 문서 관계를 지정, href는 지정 경로
  - '<style></style>'은 현재 문서에 css를 작성할때 사용한다.
  - '<script></script>'은 현재 문서에 js를 연결하거나 직접 작성할 수 있는 두가지 기능을 제공한다.

------------------
## TIP
- VS에서 (파일이름.html로 파일을 만들고 -!입력후- 엔터) 하면 기본구조를 갖춘 html 파일 생성 가능!!!!!!!
## 실습
```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <title>Github</title>
</head>
<body>
    <div class="header">
        <div class="container">
            <div class="container-left">
                <div class="logo">
                    <img src="https://heropcode.github.io/GitHub-Responsive/img/logo.svg" alt="Github Logo">
                </div>
                <div class="menu">
                    <div class="menu-item">황한식</div>
                    <div class="menu-item">H-up</div>
                    <div class="menu-item">공부</div>
                    <div class="menu-item">계획</div>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
```
![image](https://user-images.githubusercontent.com/67450413/116388946-595fbe00-a857-11eb-9e2d-0591d68cf0a1.png)


