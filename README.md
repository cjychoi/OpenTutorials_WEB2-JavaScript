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
      
 
      
