# OpenTutorials_WEB2-JavaScript
생활코딩 WEB2 - JavaScript Study [[link]](https://opentutorials.org/course/3085)

## 2. 수업의 목적 (Purpose)
  - JavaScript가 할 수 있는 기능: '사용자와 상호작용'
  - 웹브라우저는 한번 출력된 화면을 바꾸지 못함 -> JavaScript가 바꿀 수 있음
  - Chrome - 검사 - Elements (=tag)
  
  - `<input type="button" value="night" onclick=" ">`
      - 버튼을 만드는 태그
      - 글씨: 'night'
      - onclick: 클릭했을 때 " " 안의 내용을 실행, 내부는 JavaScript로 작성
      
## 3. HTML과 JavaScript의 만남: script 태그
  - `<script> ~ </script>`: html 문서 안에서 ~ 부분에 JS를 실행하기 위한 태그
  - 그냥 html로 표현하는 것과의 차이
      - JS는 동적 (1+1=2) vs html은 정적 (1+1=1+1)
      
## 4. HTML과 JavaScript의 만남: 이벤트(Event)
  - `<input type="button" value="hi" onclick="alert('hi')">`
      - onclick 이라는 속성 값 = 반드시 JS
      - onclick 속성을 기억했다가, 사용자가 클릭했을 때(이벤트) JS 코드를 실행
      
  - 웹브라우저에서 일어날 수 있는 이벤트(Event)
      - onclick: 클릭했을 때
      - onchange: 내용이 바뀌었을 때
      - onkeydown: 키를 눌렀을 때
      - 등등...
      - 이를 통해 사용자와 상호작용하는 웹페이지를 만들 수 있음.
      
## 5. HTML과 JavaScript의 만남: 콘솔(Console)
  - Chrome - 검사 - Console
  - 파일을 만들지 않고 JavaScript를 실행할 수 있음
  - 현재 보고 있는 웹페이지를 대상으로 실행함
      - Ex) 페이스북 페이지 댓글 추첨
      
## 6. 데이터 타입 (Data Types) - 문자열과 숫자 (String and Number)
  - Console 창에서 숫자 연산이 가능 
      - 산술 연산자: +, -, *, /
  - '문자' "문자"
      - "문자열".length : 문자열의 개수
      - "문자열".toUpperCase : 전부 대문자로 변환
      - "문자열".indexOf('문자열') : 찾고자 하는 문자열의 위치를 알려줌
      - "문자열".trim : 공백을 없애줌
  
  - 비교
    - `1+1` -> 2
    - `"1"+"1"` -> 11

## 7. 변수와 대입 연산자
  - `x=1; y=1; x+y;` -> 2
      - x, y라는 '변수'에 값을 대입
  - 변수의 효용
      - 수많은 데이터를 수정한다 했을 때, 한번에 수정 가능
      - `var name = 'egoing';`
      
## 8. 웹브라우저 제어 
  1. CSS의 본질적이고 중요한 문법
  2. JavaScript를 이용해서 제어하고자 하는 태그를 선택하는 방법
      

## 9. CSS 기초: style 속성
  - `<~ style=" (CSS) ">` 
      - `background-color: (color)` : 해당 글씨의 배경 색 변경
      - `color: (color)` : 해달 글씨의 색 변경
  - style 이라는 속성 안에 CSS 문법을 넣으면 디자인이 가능.
  
## 10. CSS 기초: style 태그  
  - `<div> </div>`: CSS, JS를 통해 정보를 제어하고 싶을 때 감싸주는 무기능의 태그
      - 화면 전체를 쓰기 때문에 줄바꿈 됨
  - `<span> </span>`: `<div>`와 같은 기능이지만 줄바꿈 안됨
      - `<span style="font-weight:bold;">`: 진한 글씨를 표현하는 방법
      
      
  - 바꾸고 싶은 문자열이 여러 개일 경우, 한번에 수정하는 방법
      - `<style> (CSS) </style>`: CSS로 표현된 코드를 나타냄
          - class를 나타내는 법
              - `.(class_name) { (CSS) }` : 모든 (class_name)의 속성을 (CSS)로 바꿈
  
## 11. CSS 기초: 선택자
  - 웹페이지의 여러 요소들을 효율적으로 수정하는 법
      - `<style> (CSS) </style>`
          - id 값을 부여하는 법
              - `#(id) { (CSS) }` : (id) 대상의 속성을 (CSS)로 바꿈
          - id vs. class
              - id: 고유 식별자, 오직 하나의 대상만을 가리킴
              - class: 그룹핑, id보다 포괄적인 개념
              - 같은 class 이더라도 id 선택자로 예외처리 가능. (id가 우선순위 더 높음)
          - `span { (CSS) }`
              - 모든 span 태그의 속성이 변함
      - 우선순위
          - id > class > span
  - 선택자가 중요한 이유
      - 원하는 속성을 원하는 대상에 정확하게 타겟팅해서 적용해야 하기 때문.
      
 ## 12. 제어할 태그 선택하기
  - EX08 동작 원리
      - 'night' 버튼을 눌렀을 때 `<body>` 태그에 `<style>` 속성이 생기면서 CSS의 내용에 따라 디자인이 변함.
  - EX12
      - 'onclick' 시 실행될 JavaScript 명령 (동적 상호작용)
          - `<body>` 태그를 선택하도록 해야 함
          ```
          document.querySelector('body')
          ```
          - `<body>` 태그에 `<style>` 속성을 넣어야 함
          ```
                      ~~~.style.~~~
          (querySelector).style.(backgroundColor)
          ```          
          
## 13. 프로그램, 프로그래밍, 프로그래머  
  - Program
      - 어떤 일을 수행하는 '순서'
      - 의도에 따라 순서대로 여러 기능을 작동 시키는 과정
      - 반복되는 과정을 간소화 하기 위한 방법
          - 시간의 순서에 따라 실행되어야 할 기능을 문법에 맞게 글을 적는 방식
          - '프로그래밍 언어'
          
  - HTML과 JavaScript의 차이
      - HTML: 컴퓨터 언어
          - 시간의 순서에 따라 실행되는 기능 X
      - JavaScript: 컴퓨터 언어, 컴퓨터 프로그래밍 언어      
          - 사용자와 상호작용 하기 위해 만들어짐
          - 시간의 순서에 따라 웹브라우저의 여러 기능이 실행되어야 함
  
## 15. 비교연산자(Comparison Operator)와 Boolean 변수
  ```
  <script>
    document.write(~~~)   // 웹페이지에 (~~~) 출력
  </script>
  ```
  - 비교 이항 연산자 `===`
      - 양쪽 값이 같으면 true 
      - 양쪽 값이 다르면 false 출력
  - boolean 데이터 타입
      - true 또는 false의 값을 가지는 변수
  - `&lt;` = `<`의 HTMl 표현

## 16. 조건문 (Conditional Statements)
  - `if(true)` 일 경우
      - 바로 다음 {} 수행
      - else{} 무시
  - `if(false)`일 경우
      - 바로 다음 {} 무시
      - else{} 수행
      
## 17. 조건문의 활용      
  - EX17
      - night와 day 버튼을 하나로 융합하기
      - 초기 상태: night
          1. 'NIGHT' 버튼을 누를 경우
              - if(true){}로 진입
              - 배경색: 검정, 글씨색: 흰색 으로 변경
              - value 값을 'DAY'로 변경
          2. 'DAY' 버튼을 누를 경우
              - else{}로 진입
              - 배경색: 흰색, 글씨색: 검정 으로 변경
              - value 값을 'NIGHT'로 변경

## 18. 리팩토링, 중복의 제거
  - 리팩토링(Refactoring)
      - 비효율적이고 반복되는 코드를 제거하는 과정
  
  - `this`
      - 현재 코드가 가리키고 있는 태그를 가리키는 키워드
      - EX 18
      ```
      onclick="
        if(this.value === 'NIGHT')
           this.value = "DAY';
      "
      ```
  - 중복된 코드를 제거하기 (변수 활용)
     ```
     var target = document.querySelector('body');
     target.style.backgroundColor = 'black';
     target.style.color = 'white';
     ...
     ```
     
  
