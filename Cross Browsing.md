## 프론트엔드는 크로스브라우징에 신경을 써야 할 텐데 대처는 어떻게 하시나요?
### 크로스 브라우징
- 웹 페이지의 상호 호환성을 말한다.
- 크로스 브라우징은 동일성을 의미하지 않는다! 모든 웹 브라우저에서 100% 똑같이 보이도록 만드는 것이 아니다.
- 표준 웹기술을 채용하여 다른 기종 혹은 플랫폼에 따라 달리 구현되는 기술을 비슷하게 만듦과 동시에 어느 한쪽에 최적화되어 치우치지 않도록 공통 요소를 사용하여 웹페이지를 제작하는 기법
- 사용자가 웹 사이트에 방문했을 때 정보로서 소외감을 느끼지 않도록 하는 방법론적 가이드
- 즉, 동등한 수준의 정보, 기능 접근에 초점을 맞춘다.
### 크로스 브라우징 작업
1. 도움이 되는 사이트를 이용하여 브라우저에 맞게 작업한다. - 캔아이유즈 https://caniuse.com
2. 초기화 작업 (CSS 초기화 작업) - 브라우저마다 차이가 나는 기본 스타일 값들을 초기화 시킨다.
3. 핵(Hack) - 스타일을 줄 때 특수문자를 넣어서 다른브라우저들에서는 인식이 안되지만 IE 특정 버전에서는 인식되도록 하는 방법이다. 이 방법은 추천하지 않는다.
4. IE용 주석을 이용한 방법 (Conditional comments) - HTML 문서 내에서 주석을 이용하여 구별한다.
5. 메타 태그를 이용한 IE모드
- <head> 요소 안에 넣어두며 IE가 문서를 읽고 랜더링 할 때 원하는 모드로 랜더링을 하게 해준다.
만약 content에 값이 "IE=edge"라면 해당브라우저가 할 수 있는 가장 최신의 모드로 랜더링한다.


## 만든 페이지가 IE11에서도 작동했는지, 작동하게 하려면 어떤 방식을 써야하는지?
  #### 먼저 IE TEST 사이트를 이용하여 호환성 체크
  #### 리액트 IE11 크로스 브라우징 문제 해결
   react-app-polyfill을 설치<br>
  package.json 파일에서 development 항목에 ie11 추가하기 <br>
  index.js 파일에서 react-app-polyfill/ie11과 /stable을 import<br>
  마지막으로 node_modules/.cache 폴더를 삭제하고(존재한다면) 다시 npm start로 실행