# 서버와 클라이언트

- 클라이언트: 서버에세 요청하는 대상
- 서버: 요천받은 서비스를 알맞게 응답해주는 대상

### 웹 (Web)

- 요청과 응답이 일어나는 장소

### 웹 브라우저(Web Browser)

- 사용자의 요청에 맞는 주소로 찾아가서 인터넷 컨텐츠(문서와 그림, 파일 등)를
  검색 및 열람 후 사용자에게 응답하기 위한 응용 프로그램의 총칭이다

### 프로토콜(Protocol): 통신 규약

- 클라이언트의 요청에 반드시 응답해야 한다는 약속.

- http:// (Hypertext Transfer Protocol)
  - 클라이언트와서버 간 텍스트로 통신하기 때문에 가로채어 보낟면 누구든 내용을 볼 수 있다
- https:// (Hypertext Transfer Protocol Secure Socket)
  - SSL 프로토콜을 이용해서 자원을 암호화한 뒤 통신하는 규약

### IP(Internet Protocol)

- 클라이언트가 찾아갈 서버의 고유한 값, 컴퓨터가 다른 컴퓨터와 구별될 수 있도록 중복이 없는 값으로 설정되며, 네트워크 상에서 사용된다.

### 도메인(Domain)

- IP 주소는 기억하고 이해하기 힘들기 때문에 이를 위해서 이름(별칭)을 붙일 수 있도록 한 것

### WWW (World Wide Web)

- 인터넷에 연결된 전 세계 컴퓨터들을 통해 사람들이 정보를 공유할 수 있는 정보 공간

### W3C

- WWW를 위한 표준을 재정하고 관리하는 중립적인 기관이다.

<hr/>

## 웹 표준(Web Standard)

1.  HTML (Hypertext Markup Language)

    - 웹 페이지에서 다른 페이지로 이동할 수 있도록 해주는 마크업 언어이다.
    - 태그를 이용하여 문서나 데이터의 구조를 기술하는 언어이다.

2.  CSS (Cascading Style Sheets)

    - 구체적으로 어떤 스타일로 요소가 표시되는 지를 정하는 규격이다.
    - HTML에 작성된 스타일을 따로 분리해서 일괄처리가 가능하도록 한다

3.  JS (JavaScript)

    - 화면 쪽에서 연산이 가능한 스크립트 언어이다
    - 사용자의 다양한 이벤트 처리, 비동기 통신등을 자유롭게 사용할 수 있다
    - HTML 안엑서 태그형태로 JS를 사용할 수도 있으며, 외부 파일로 제작후 포함시켜서 사용할 수도 있다 유효성 검사, 통신 등을 담당한다.

4.  XHTML (Extensible HTML)

    - 기존에 사용되던 HTMl 규격이 가진 문제점을 극복하고 보다 다양한 분야에 응용될 수 있도록 해주는 여러가지 확장된 기능을 포함 한다.
    - HTML과 XHTML은 사실상 큰 차이없이 사용한다

5.  XML (Extensible Markup Language)

    - 어떠한 데이터를 설명하기 위해서 임의로 지은 태그로 데이터를 감싼다
    - 태그로 데이터를 설명하며, 이것이 데이터의 표시(Markup)가 되고 추가적인 데이터가 생기면 태그 추가와 태그 내부 내용을 추가할 수 있다. 따라서 데이터를 전달하는 데에 목적이 있다


        ####

            <?xml version="1.0">
            <user>
                <user.id>bsh</user.id>
                <name>백시현</name>
            </user>

    <hr/>

## HTML의 요소

      <p> You are better </p>
      --- -------------- ---
      (1)       (2)      (3)

      (1) 여는 태그(Opening tag): 요소의 이름(p)과 열고 닫는 꺽쇠 괄호로 구성한다
      (2) 내용(Content): 요소의 내용이며, 단순한 텍스트를 의미한다
      (3) 닫는 태그(Closing tag): 요소의 이름 앞에 슬래시(/)가 있다

### HTML의 주석

      <!-- 주석 -->

1. 설명글을 작성할 때 사용한다.
2. 지금 당장 사용하지 않는 코드를 숨기고 싶을 때 사용한다.

### 속성(Attribute)
- 태그는 속성을 가질수 있다
####
      <p class="conversation"> You are much better </p>
   속성은 내용에 나타나고 싶지 않지만 추가적인 내용을 담고 싶을 때 사용한다
   특히 id와 class 속성은 스타일에 관련된 내용이나 기타 연산등의 내용을 위해
   해당 태그를 찾을 수 있는 구분점 역할을 한다

- 속성 사용 시 주의사항
   1. 태그 이름 다음에 오는 속성은 태그 이름과 속성 사이에 공백이 있어야 하고,
      여러 속성이 있을 경우에도 공백으로 구분한다.
      ####
            <p id="p1" class="p-group"> You are pretty </p>

   2. 속성 이름 다음에는 등호(=)를 작성한다.
   3. 속성 값은 따옴표 안에 작성한다.

<hr/>

### HTML 요소의 종류
-  블록 요소
   - p, h, ul, ol, div, form, ... 등
   - 웹 페이지 상에 블록(영역)을 만드는 요소
   - 코드 상에 한 줄로 이어써도 화면 상에서는 앞 뒤 요소 사이에 새로운 줄을 만들어서
      줄을 만든 뒤 나타난다.
      ####
            <p>apple</p><p>banana</p>
   - 영역이 정확히 구분되어 있기 때문에, width와 height 속성을 수정할 수 있다.
   - margin-top, margin-bottom 속성도 잘 적용된다(바깥 여백 상하).
   - padding-top, padding-bottom 속성도 잘 적용된다(안쪽 여백 상하).

-  인라인 요소
   - span, a, img, strong, em, ... 등
   - 새로운 줄을 만들지 않고 작성한 단락 내에 나타난다.
   - 안에 있는 내용만큼만 영역을 차지하고 기본적으로 가지고 있는 영역은 없다.
   ####
         <em>apple</em><span>banana</span>
   - 영역이 불분명하기 때문에 width와 height를 임의로 부여할 수 없다.
   - margin-top, margin-bottom 속성은 부여할 수 없다(바깥 여백 상하).
   - padding-top, padding-bottom 속성은 부여할 수는 있지만 전체적인 구조를 잡기는 힘들다.(안쪽 여백 상하).

-  인라인 블록 요소
   - button, input, select, ... 등
   - inline 요소와 동일한 영역(내용만큼)을 가지지만 본인만의 영역을 정확히 가지고 있다.
   - width와 height를 설정할 수 있고,
      margin-top, margin-bottom, padding-top, padding-bottom 모두 잘 적용된다.

### form 태그
   웹 페이지 내에서 사용자로부터 입력을 받을 때 사용하는 태그
   사용자가 입력한 데이터를 처리하기 위해서 다른 곳으로 전송할 때 form 태그를 사용한다.
####
      <form action="" method="" name="">
         입력 태그
         입력 태그
         입력 태그
         ...
      </form>

- action: 데이터를 전송할 페이지의 경로
- method: 데이터를 전송하는 방식
- name: form 태그의 이름을 설정


### input 태그
- type : 입력 종류를 설정
- name : value의 key값
- value : 사용자가 입력한 값(입력 전에 미리 값을 넣어줄 수 있다).
- placeholder : 값은 아니지만 미리 출력해줄 문구를 작성할 수 있다.
- readonly : 수정할 수 없도록 하는 설정
- required : 필수 항목
- maxlength : 글자 수 제한

### input 태그의 type
      <input type="">

      *text
      *password
      *radio
      *checkbox
      *button, submit, reset
      *date
      *file
      color
      email
      url
      tel
      number, min, max, step
      range
      search
