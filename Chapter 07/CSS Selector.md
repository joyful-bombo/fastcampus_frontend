# 💡 CSS 선택자

## 💡 기본
  - 전체 선택자(Universal Selector)
    - **모든** 요소를 선택
    - ```
      *{
        color: red;
      }
      ```
  - 태그 선택자(Type Selector)
    - **태그 이름** 요소 선택
    - ```
      li{
        color: red;
      }
      ```
  - 클래스 선택자(Class Selector)
    - HTML **class 속성의 값**인 요소를 선택
    - ```
      .orange{
        color: red;
      }
      ```
  - 아이디 선택자(ID Selector)
    - ```
      #orange{
      color: red;
      }
      ```
## 💡 복합
  - 일치 선택자(Basic Combinator)
    - A.B
    - 선택자 A와 B를 **동시에 만족**하는 요소 선택
    - ```
      span.orange {
        color : red;
      }
      ```
  - 자식 선택자(Child Combinator)
    - A > .B
    - 선택자 A의 **자식** 요소 B 선택
    - ```
      ul > .orange {
        color: red;
      }
      ```
  - 하위 선택자(Descendant Combinator)
    - A .B
    - 선택자 A의 **하위** 요소 B 선택 **띄어쓰기**가 선택자의 기호
    - ```
      div .orange {
        color: red;
      }
      ```
  - 인접 형제 선택자(Adjacent Sibling Combinator)
    - A + B
    - 선택자 A의 다음 형제 요소 B **하나**를 선택
    - ```
      .orange + li {
        color: red;
      }
  - 일반 형제 선택자(General Sibling Combinator)
    - A ~ B
    - 선택자 A의 다음 형제 요소 B **모두**를 선택
    - ```
      .orange ~ li {
        color: red;
      }
      ```
## 💡 가상 클래스
  - 가상 클래스 선택자(Pseudo-Classes)
  - HOVER
    - A:hover
    - 선택자 A의 요소에 **마우스 커서가 올라가 있는 동안** 선택
    - ```
      a:hover {
        color: red;
      }
      ```
  - ACTIVE
    - A:active
    - 선택자 A 요소에 **마우스를 클릭하고 있는 동안** 선택
    - ```
      a:active {
        color: red;
      }
      ```
  - FOCUS
    - A:focus
    - 선택자 A 요소가 **포커스되면** 선택
      - 포커스 가능 요소
        - HTML 대화형 컨텐츠
        - INPUT, A, BUTTON, LABEL, SELECT, tabindex등등
      - ```
        input:focus {
          background-color: orange;
        }
        ```
  - FIRST CHILD
    - A:first-child
    - 선택자 A가 형제 요소 중 첫째라면 선택
    - ```
      .fruits span:first-child {
        color: red;
      }
      ```
  - LAST CHILD
    - A:last-child
    - 선택자 A가 형제 요소 중 막내라면 선택
    - ```
      .fruits h3:last-child {
        color: red;
      }
      ```
  - NTH CHILD
    - A:nth-child(n)
    - 선택자 A가 형제 요소 중 (n)째라면 선택
    - ```
      .fruits *:nth-child(2) {
        color: red;
      }
      
      .fruits *:nth-child(2n) {
        color: red;
      }
      ```
    - n은 0부터 시작(Zero-Based Numbering)
  - NOT
    - A:not(B)
    - 선택자 A가 아닌 B인 모든 요소 선택
    - ```
      .fruits *:not(span) {
        color: red;
      }
      ```
## 💡 가상 요소
  - BEFORE
    - A::before
    - 선택자 A 요소의 **내부 앞**에 내용(Content)을 삽입.
    - **content를 안쓰더라도 꼭 써줘야한다.**
    - ```
      .box::before {
        content: "앞!";
      }
      ```
  - AFTER
    - A::after
    - 선택자 A의 요소의 **내부 뒤**에 내용(Content)을 삽입.
    - **content를 안쓰더라도 꼭 써줘야한다.**
    - ```
      .box::after {
        content: "뒤!";
      }
      ```
      
## 💡 속성 선택자(Attribute)
  - [ABC]
    - 속성 ABC를 포함한 요소 선택
    - ```
      [disabled] {
        color: red;
      }
      ```
  - [Type]
    - 속성 ABC를 포함한 요소 선택
  - [ATTR=VALUE]
    - [ABC="XYZ"]
    - 속성 ABC를 포함하고 값이 XYZ인 요소 선택.
    - ```
      [type="password"] {
        color: red;
      }
      ```
