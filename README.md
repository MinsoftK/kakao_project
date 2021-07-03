# Kakao_Clone_Coding  

* Made by Minsoftk  
기간 : 2021.06.13 ~ 현재진행중  

환경 : Chrome 브라우저  

주제 : 웹 사이트 UI 개발

<br/>
<br/>

# 프로젝트 상세 내용
## 주제
* 우리가 자주 사용하는 kakao톡의 UI를 따라 만들어보기.  

## 목적
* 세련된 웹 페이지 제작을 위해서 CSS의 고급 기술을 익히기

## 구현 목표
* Media Query와 Animation을 적용해 세련된 웹 페이지 구현

## 기술스택
* [HTML, CSS, JS](https://github.com/MinsoftK/TIL/tree/master/HTML-CSS-JS)에 대한 간략한 정리내용.
* [Block Element Modifier](https://velog.io/@ylem76/BEM) 방식을 사용.
* Icon : [Heroicons](https://heroicons.dev/), [font Awesome](https://fontawesome.com/)
* 개발 : VSC(Visual Studio Code), GitHub, HTML, CSS


## Trouble
### 1
Friends.html 에서 status-bar와 nav-bar를 fixed 해놓은 상태에서 friends-display-link를 body안에 삽입했을때 계속 nav-bar 와 겹쳐져서 보이지 않는 이슈를 겪었다. body 프레임 안에서 nav-bar가 위치하지 않는걸로 인식돼 계속 겹쳐져서 보이지 않는것 같다. 따라서 absolute를 통해 부모 relative에 위치하게 만든 다음 위치를 수정시켰다.  
<br/>

[CSS 스크롤 관련 엘리먼트 움직이지 않는 이슈](https://www.notion.so/minsoftk/39b928dcefd84677992333ed08379a42#dddc90c8e1144638a3811e0d099c1dd6)  
위 블로그를 참고해 position : sticky 속성을 활용했다. 결국 두방법 모두 부모의 relative가 중요했다.

-> 1. 해결 : 아예 body의 속성을 없애버리고 component css로 각각 넣어서 해결했다.



