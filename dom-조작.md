# DOM 조작

## DOM이란

- 브라우저가 HTML 문서를 이해하고 조작할 수 있도록 **트리 구조의 객체로 변환**한 모델이다.
- 자바스크립트를 이용해 **웹 페이지의 요소를 동적으로 추가, 삭제, 수정**하는 API 역할을 하며, HTML구조와 상호작용하는 필수적인 인터페이스이다.

## 주요 특징

- HTML 태그를 계층적인 **트리 노드 형태로 구조화**한다.
- 자바스크립트를 사용해 웹 문서의 **내용이나 스타일을 실시간으로 변경**할 수 있다.
- 마우스 클릭, 키보드 입력 등 **사용자 인터랙션**에 반응한다.

## 주요 DOM 선택자 및 사용법

- document.getElementByld()
  - **ID로 요소를 선택**하며 **하나**의 요소만 반환한다.
- document.getElementsByClassName()
  - **클래스 이름으로 여러 요소**를 선택한다.
- document.querySelector() / querySelectorAll()
  - **CSS 선택자 형식**으로 요소를 선택할 수 있다.

## 자주 발생하는 오류와 해결 방법

- Uncaught TypeError: Cannot read properties of null
  - 원인 : 선택한 **요소가 존재하지 않을 때** 발생
  - 해결 방법 : 요소가 존재한 이후에 자바스크립트가 실행되도록 처리한다.
- 스타일 적용 안됨
  - 원인 : 선택자 오류, **inline 스타일 우선순위** 문제
  - 해결 방법 : 올바른 선택자 사용 및 우선순위 확인
- querySelectorAll로 선택한 요소가 **반복되지 않음**()
  - 해결 방법 : NodeList에 forEach 또는 반복문 사용

<hr>

## 요소 생성 / 수정

## 요소 생성

- createElement : 요소를 만드는 메서드
- createTextNode : 거북이를 만드는 방법

## 요소 속성

- 속성 설정 : setAttribute('속성명','속성값');
- 속성값 찾기 : getAttribute('속성명);
- innerHTML : HTML 요소 내부에 있는 HTML 코드를 **있는 그대로 문자열 형태로 접근**할 수 있도록 해준다.
- innerText : **HTML 코드는 무시**하고 화면에 보이는 텍스트를 **있는 그대로 접근**할 수 있도록 해준다.
- textContent : innerText처럼 **HTML 코드를 무시**하고 텍스트만 접근할 수 있도록 해준다. 하지만 속성 값에 **숨겨진 요소의 텍스트까지 포함**된다는 차이점이 있다.

## 요소 삽입

- prependChild(삽입할 요소) : **첫번째** 위치에 삽입
- appendChild : **마지막** 위치에 삽입

## 요소 삭제

- RemoveChild(삭제할 요소)
