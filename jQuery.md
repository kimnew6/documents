# 제이쿼리(jQuery)
제이쿼리는 자바스크립트 언어를 간편하게 사용할 수 있도록 단순화시킨 오픈 소스 기반의 자바스크립트 라이브러리입니다.    
   
제이쿼리를 이용하면 문서 객체 모델(DOM)과 이벤트에 관한 처리를 손쉽게 구현할 수 있습니다.   
또한, Ajax 응용 프로그램 및 플러그인도 제이쿼리를 활용하여 빠르게 개발할 수 있습니다.

## React를 사용하는 이유?
### 1. React는 jQuery보다 빠릅니다
**React**가 가지고있는 가장 큰 것 중 하나는 전통적인 DOM 대신 **Virtual DOM (Document Object Model)** 을 사용하는 것입니다. jQuery는 DOM과 직접 작동하지만 React는 React를 훨씬 더 빠르게 만드는 가상 DOM을 사용합니다.   
DOM의 내용을 업데이트해야 할 때마다 Real DOM은 트리의 맨 위에서 아래까지 업데이트. Virtual DOM은 일반 DOM과 같이 시작, 변경된 부분만 업데이트하는  DOM 부분이 되도록 만든다.   
### 2. React는 현대적입니다
jQuery가 예전처럼 필요하지 않으며, 오늘날 대부분의 다른 라이브러리와 프레임 워크가 jQuery와 동일한 작업을 수행 할 수 있다.
### 3. React는 더 큰 앱에 더 좋습니다
앱이 커지면 더 많은 DOM 조작이 발생하므로 상황이 느려지기 시작합니다.   
더 큰 앱에서 작업을 시작할 때 jQuery에서 발생할 수있는 또 다른 문제는 "스파게티 코드"(관리가 매우 어렵거나 불가능 해지는 일명 코드)를 생성 할 가능성이 있다는 것입니다.
### 4. React Native를 사용하는 모바일 앱
모바일 애플리케이션을 만들고 싶었다면 React Native가 적합합니다.  jQuery는 모바일 장치에서 애플리케이션이 더 잘 보이도록 도울 수 있지만 React Native를 사용하면 IOS 및 Android 용 실제 모바일 앱을 만들 수 있습니다.
