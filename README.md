# web-study
basic things about web


## css(from 생활코딩)
* inline, block level
  * inline은 본문의 크기(요소의 크기 X)만큼의 공간만 사용하는 것, block은 줄 전체를 사용하는 것

* border, padding, margin
  * border : 그 요소의 테두리
  * padding : 본문과 테두리 사이의 간격 --> 식당에서 접시는 큰데 음식이 조금 나왔다! padding 값이 상당히 크군!!
  * margin : 두 개 이상의 요소가 있을 때, 그 요소들 사이의 간격 --> 접시와 접시 사이의 간격! 다른 접시 놔야되니까 margin을 줄여!!

* 마진 겹침 현상 --> margin : 30px로 지정해줄 시에, 벽과 요소들 사이 및 요소와 요소들 사이의 거리가 모두 30px이 되어야 한다. 마진 겹침이 되지 않는다면 요소와 요소들 사이는 그 두배인 60px이 되어버린다.

* width, height
  *  block element들을 다루는 중에 한 줄 전체를 사용하고 싶지 않은 경우에 이들을 통해 조정이 가능하다. --> height는 지정 시 본문이 요소를 이탈하는 경우 종종 생김. 따라서 잘 안씀.
  *  inline element들에게는 적용이 되지 않는다.


* position
  * default value : static --> 본래 요소의 위치를 바꿀 수 없는 상황
  * position type : relative, absolute 등등이 있다.
  * left, right, top, bottom을 이용해 위치를 결정한다. (left, right중에 left, top, bottom중에 top을 선택한다. 이들을 offset이라고 부른다.)
  * static : 현재의 위치이고, 위치를 바꿀 수 없게 한다.
  * relative : 부모의 element를 기준으로 상대적 위치가 정해진다.
  * absolute : static이 아닌 부모의 element를 기준으로 위치가 정해진다. --> offset이 지정되어 있지 않은 경우에는 현재 본인의 위치가 default 값으로 설정됨. 그리고 부모랑 연이 끊어진 듯하게 행동함.
  * fixed : 위치가 스크롤에 무관하게 고정되야 될 상황에 사용이 가능하다. (가장 위의 menu 같은 경우 fixed 사용하면 좋을 듯) absolute와 유사하게 기능함.


* flex
  * display : flex; 로 모든걸 시작한다.
  * container와 item이 있을 시에 잘 정리할 수 있다.
  * container
   1. flex-direction : 내부 요소들을 정렬한다. row계열의 경우(가로로 정렬)에는 세로 전체를, column 계열의 경우(세로롤 정렬)에는 가로 전체를 사용한다.

  * item
   1. flex-basis : 내부 요소의 기본 크기를 설정한다.
   2. flex-grow : 0이 아닌 숫자를 지정하면 그 비율만큼 가져간다.
   3. flex-shrink : 화면 크기 변화할 때 그 크기 줄어드는 속도를 나타낸다.(화면의 크기가 줄어도 모든 요소를 화면안에 담고 싶기 때문!)

holy-grail layout!!!!!..
