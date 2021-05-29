🦄TIL-9🦄
# [멀티미디어]
# IMG의 srcset과 sizes 속성
- 반응형 웹 사이트를 만들기 위한 속성들 이다.
- 이미지를 깨긋하게 사용하기 위해서 이미지를 늘리지 않고 줄여서 사용하기 위해 사용된다.
```html
<img
  srcset="images/heropy_small.png 400w,
          images/heropy_medium.png 700w,
          images/heropy_large.png 1000w"   /*이미지 후보들 */
  sizes="(max-width: 500px) 444px,
         (max-width: 800px) 777px,   /*최적화 출력*/
         1222px"
  src="images/heropy.png"
  alt="HEROPY" />
```
- srcset = source set으로 후보 이미지들과 그 범위를 지정해 준다.
  - 단위는 `w`임에 주의하자!
- css 코드로도 구현 가능하지만 코드가 너무 길어 지기 때문에 HTML의 srcset과 sizes 속성을 이용한다!

# audio 태그
- 오디오 콘텐츠를 삽임 가능한 태그이다.

|속성|의미|값|
|------|---|---| 
|autoplay|준비되면 바로 재생|Boolean|	
|controls|제어 메뉴를 표시|Boolean|	
|loop|재생이 끝나면 다시 처음부터 재생|Boolean|	
|preload|	페이지가 로드될 때 파일을 로드할지의 지정(힌트 제공)|	none: 로드하지 않음,<br/>metadata: 메타데이터만 로드,<br/>auto: 전체 파일 로드
|src|	콘텐 URL|	URL	|
|muted|음소거 여부|Boolean|

# video 태그
- 비디오 콘텐츠를 삽임 가능한 태그이다.

|속성|의미|값|
|------|---|---| 
|autoplay|준비되면 바로 재생|Boolean|	
|controls|제어 메뉴를 표시|Boolean|	
|loop|재생이 끝나면 다시 처음부터 재생|Boolean|	
|preload|	페이지가 로드될 때 파일을 로드할지의 지정(힌트 제공)|	none: 로드하지 않음,<br/>metadata: 메타데이터만 로드,<br/>auto: 전체 파일 로드
|src|	콘텐 URL|	URL	|
|muted|음소거 여부|Boolean|
|poster|	동영상 썸네일 이미지 URL|	URL|
|width	|동영상 가로 너비|
|height|	동영상 세로 너비|

# figure, figcaption 태그
- 이미지의 설명 텍스트를 지정한다.
```html
<figure>
  <img src="milk.jpg" alt="A milk">
  <figcaption>This is text for picture </figcaption>
</figure>
```
`figure` = 전체 영역 지정
`figcaption` = 텍스트 지정

# [내장 콘텐츠]
# iframe
- 다른 페이지를 현재 페이지에 삽입하는 기능을 한다. (중첩된 브라우저를 표시한다.)
- `유튜브 영상 우클릭- 소스코드 복사` 후 에디터에 붙여 넣기 하면 바로 iframe 생성됨!

|속성|의미|값|
|----|----|------|
|name|	프레임의 이름|
|src|	포함할 문서의 URL	|URL	
|width	|프레임의 가로 너비		
|height	|프레임의 세로 너비		
|allowfullscreen	|전체 화면 모드 사용 여부|	불린(Boolean)	
|frameborder	|프레임 테두리 사용 여부	|0, 1	
|sandbox|	보안을 위한 읽기 전용으로 삽입	|불린(Boolean) or<br/>allow-form: 양식 제출 가능,<br/>allow-scripts: 스크립트 실행 가능 ,<br/> allow-same-origin: 같은 출처(도메인)의 리소스 사용 가능|

# [스크립트]
# script 태그
- link는 css를 불러오고 style은 css를 포함하는 태그 였다면, script는 JS를 위한 태그이다.
- JS를 내부에 포함 시키거나, 불러 올 수 있다. (2가지 기능!)
- script 태그는 바디 태그 맨 마지막에 넣는다. == <script src="" __defer="true"__>

    
