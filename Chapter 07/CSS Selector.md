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
    - 선택자 A와 B를 **동시에 만족**하는 요소 선택
    - ```
      span.orange {
        color : red;
      }
      ```
  - 자식 선택자(Child Combinator)
    - 선택자 A의 **자식** 요소 B 선택
    - ```
      ul > .orange {
        color: red;
      }
      ```
  - 하위 선택자(Descendant Combinator)
    - 선택자 A의 **하위** 요소 B 선택 **'띄어쓰기'**가 선택자의 기호
    - ```
      div .orange {
        color: red;
      }
      ```
  - 인접 형제 선택자(Adjacent Sibling Combinator)
    - 선택자 A의 다음 형제 요소 B **하나**를 선택
    - ```
      .orange + li {
        color: red;
      }
  - 일반 형제 선택자(General Sibling Combinator)
    - 선택자 A의 다음 형제 요소 B **모두**를 선택
    - ```
      .orange ~ li {
        color: red;
      }
      ```
## 💡 가상 클래스

## 💡 가상 요소

## 💡 속성
