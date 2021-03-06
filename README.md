# markup-study


## Day 1
https://minjung-jeon.github.io/markup-study/day1/index.html

1. background-image 를 사용한 이미지 사용
   - background-repeat: no-repeat;
   - background-size: cover; : 이미지의 가로,세로 크기 지정
     - cover: 요소를 다 채울 수 있게 이미지 확대, 축소(가로, 세로 비율 유지)
     - contain: 요소를 벗어나지 않는 최대 크기로 이미지 확대, 축소(가로, 세로 비율 유지)
   - background-position: 50% 50%; : 배경이미지 위치 지정

2. calc, padding-top 을 사용한 높이값 계산
   - calc 함수를 사용하여 높이값 계산
    - 비지원 브라우저 존재(IE 9 부터 지원)
    - `+, -` 연산자는 공백이 있어야한다.
   - padding-top
     - padding의 값은 width를 기반으로 생성
     - 내부의 요소들은 absolute를 사용하여 위치 지정

----

- 참고 Site 목록
1. [CSS 레이아웃을 배웁시다](https://ko.learnlayout.com/display.html)



## Day 2
https://minjung-jeon.github.io/markup-study/day2/index.html

1. `box-sizing` : 박스의 크기를 어떤 기준으로 계산할지 정하는 속성
   -  border-box : 해당 엘리먼트의 padding과 border를 포함하여 요소의 크기를 정한다.(선안한 값 width 그대로 보여진다.)
2. border-radius 와 overflow:hidden
   - 상위 엘리먼트에서 border-radius 속성 지정 후 하위 엘리먼트에서 background-color를 지정할 경우 radius가 정상적으로 나타나지 않는다.
   - 이때 상위 엘리먼트에서 `overflow: hidden` 속성을 추가하면 radius가 정상적으로 적용
   
   ```html
   <div id="wrapper">
      <div id="box"></div>
   </div>
   ```
   ```css
   #wrapper {
      width: 300px; height: 300px;
      border-radius: 100px;
      overflow: hidden;
   }

   #box {
      width: 300px; height: 300px;
      background-color: #cde;
   }
   ```

3. inline-block 이 html의 공백을 고려하여 여백이 생긴다.
      - inline-block 레벨 요소 뒤에 공백이 있는 경우, 정의하지 않은 공간이 자동으로 지정된다.
      - 회피 하는 방법은 부모 요소에 `font-size:0` 을 지정 하여 공백의 사이즈를 없앤다.

- 참고 Site 목록
1. [Fighting the Space Between Inline Block Elements](https://css-tricks.com/fighting-the-space-between-inline-block-elements/)


## Day3

https://minjung-jeon.github.io/markup-study/day3/index.html

1. float 속성 적용시 부모(상위요소)에 `overflow: hidden;` 속성을 지정하여 float clear 시킨다.

2. 공부해야할 것 : flex, float clear 시키는 방법들

----

- 참고 Site 목록
1. [CSS 레이아웃을 배웁시다](https://ko.learnlayout.com/inline-block.html)
2. [float 레이아웃 문제 해결](https://webdir.tistory.com/272)
