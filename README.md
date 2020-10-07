# markup-study


### Day 1
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
