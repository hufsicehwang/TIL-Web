🐲TIL-14🐲

# position
: 위치의 기준을 지정한다.
- 기준을 지정한 다음 top,bottom,left,right로 위치를 지정한다.

## position : relative
: 원래 __자기 자신__이 있었던 위치를 기준으로 잡는다.

## position : absolute
: 보모 요소 중 __가장 최근의 position__을 가지는 위치를 기준으로 잡느다.
- 자식 요소에서 absolute를 쓰기위해선 부모 요소에 relative를 부여해야 한다.

## position : fixed
: view port(회면 자체)를 기준으로 위치를 잡는다.
ex) 쇼핑몰의 광고 베너 등등..

## position : sticky
: 스크롤시 상단에 붙어서 움직임, JS를 쓰지 않고 쉽게 구현 가능하다.

# background
: 배경을 지정한다. 이미지, 색상에 주로 사용된다.
- `background-img: url();`: 이미지를 지정할 수 있다,
- `background-size: (width) (height)` : 이미지의 사이즈를 지정할 수 있다.
    - __`background-size: (width)` 만 사용하여 이미지를 찌그러트리지 않고 사용하자!!__
- `background-repeat:no-repeat`: 반복을 멈춘다.
    - background의 지정 크기에서 이미지 사이즈를 지정하면 남는 크기만큼 반복된다.  

# transition
: 바뀌기 전의 태그에 속성을 부여하며 바뀔 것(property)과 시간(duration)을 지정한다.
```css
.box{
  width: 100px;
  height: 100px
  background:tomato;
  transition : width 1s;   // 1초동안 width를 바꾼다
}
.box:hover{
  width: 200px;
}
```
- `transition : width 1s` = `transition-property :width; ,  transition-during:1s` 
- __가상 선택자와 짝으로 사용시 애니메이션 기능으로 사용 가능!!!!!__

# 이동 (transform)
```css
.box{
  width: 100px;
  height: 100px
  background:tomato;
  transition: 1s;  // 1초동안
  
.box:hover{
  transform: translate(30px,30px)    // 마우스 올리면 해당 위치로 이동함
}
```

# 크기 (transform)
```css
.box{
  width: 100px;
  height: 100px
  background:tomato;
  transition: 1s;  // 1초동안
  
.box:hover{
  transform: scale(2)    // 마우스 올리면 2배로 늘어남 
  }
```
     
