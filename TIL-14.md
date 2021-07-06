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
