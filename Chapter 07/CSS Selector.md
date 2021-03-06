# π‘ CSS μ νμ

## π‘ κΈ°λ³Έ
  - μ μ²΄ μ νμ(Universal Selector)
    - **λͺ¨λ ** μμλ₯Ό μ ν
    - ```CSS
      *{
        color: red;
      }
      ```
  - νκ·Έ μ νμ(Type Selector)
    - **νκ·Έ μ΄λ¦** μμ μ ν
    - ```CSS
      li{
        color: red;
      }
      ```
  - ν΄λμ€ μ νμ(Class Selector)
    - HTML **class μμ±μ κ°**μΈ μμλ₯Ό μ ν
    - ```CSS
      .orange{
        color: red;
      }
      ```
  - μμ΄λ μ νμ(ID Selector)
    - ```CSS
      #orange{
      color: red;
      }
      ```
## π‘ λ³΅ν©
  - μΌμΉ μ νμ(Basic Combinator)
    - A.B
    - μ νμ Aμ Bλ₯Ό **λμμ λ§μ‘±**νλ μμ μ ν
    - ```CSS
      span.orange {
        color : red;
      }
      ```
  - μμ μ νμ(Child Combinator)
    - A > .B
    - μ νμ Aμ **μμ** μμ B μ ν
    - ```CSS
      ul > .orange {
        color: red;
      }
      ```
  - νμ μ νμ(Descendant Combinator)
    - A .B
    - μ νμ Aμ **νμ** μμ B μ ν **λμ΄μ°κΈ°**κ° μ νμμ κΈ°νΈ
    - ```CSS
      div .orange {
        color: red;
      }
      ```
  - μΈμ  νμ  μ νμ(Adjacent Sibling Combinator)
    - A + B
    - μ νμ Aμ λ€μ νμ  μμ B **νλ**λ₯Ό μ ν
    - ```CSS
      .orange + li {
        color: red;
      }
  - μΌλ° νμ  μ νμ(General Sibling Combinator)
    - A ~ B
    - μ νμ Aμ λ€μ νμ  μμ B **λͺ¨λ**λ₯Ό μ ν
    - ```CSS
      .orange ~ li {
        color: red;
      }
      ```
## π‘ κ°μ ν΄λμ€
  - κ°μ ν΄λμ€ μ νμ(Pseudo-Classes)
  - HOVER
    - A:hover
    - μ νμ Aμ μμμ **λ§μ°μ€ μ»€μκ° μ¬λΌκ° μλ λμ** μ ν
    - ```CSS
      a:hover {
        color: red;
      }
      ```
  - ACTIVE
    - A:active
    - μ νμ A μμμ **λ§μ°μ€λ₯Ό ν΄λ¦­νκ³  μλ λμ** μ ν
    - ```CSS
      a:active {
        color: red;
      }
      ```
  - FOCUS
    - A:focus
    - μ νμ A μμκ° **ν¬μ»€μ€λλ©΄** μ ν
      - ν¬μ»€μ€ κ°λ₯ μμ
        - HTML λνν μ»¨νμΈ 
        - INPUT, A, BUTTON, LABEL, SELECT, tabindexλ±λ±
      - ```CSS
        input:focus {
          background-color: orange;
        }
        ```
  - FIRST CHILD
    - A:first-child
    - μ νμ Aκ° νμ  μμ μ€ μ²«μ§ΈλΌλ©΄ μ ν
    - ```CSS
      .fruits span:first-child {
        color: red;
      }
      ```
  - LAST CHILD
    - A:last-child
    - μ νμ Aκ° νμ  μμ μ€ λ§λ΄λΌλ©΄ μ ν
    - ```CSS
      .fruits h3:last-child {
        color: red;
      }
      ```
  - NTH CHILD
    - A:nth-child(n)
    - μ νμ Aκ° νμ  μμ μ€ (n)μ§ΈλΌλ©΄ μ ν
    - ```CSS
      .fruits *:nth-child(2) {
        color: red;
      }
      
      .fruits *:nth-child(2n) {
        color: red;
      }
      ```
    - nμ 0λΆν° μμ(Zero-Based Numbering)
  - NOT
    - A:not(B)
    - μ νμ Aκ° μλ BμΈ λͺ¨λ  μμ μ ν
    - ```CSS
      .fruits *:not(span) {
        color: red;
      }
      ```
## π‘ κ°μ μμ
  - BEFORE
    - A::before
    - μ νμ A μμμ **λ΄λΆ μ**μ λ΄μ©(Content)μ μ½μ.
    - **contentλ₯Ό μμ°λλΌλ κΌ­ μ¨μ€μΌνλ€.**
    - ```CSS
      .box::before {
        content: "μ!";
      }
      ```
  - AFTER
    - A::after
    - μ νμ Aμ μμμ **λ΄λΆ λ€**μ λ΄μ©(Content)μ μ½μ.
    - **contentλ₯Ό μμ°λλΌλ κΌ­ μ¨μ€μΌνλ€.**
    - ```CSS
      .box::after {
        content: "λ€!";
      }
      ```
      
## π‘ μμ± μ νμ(Attribute)
  - [ABC]
    - μμ± ABCλ₯Ό ν¬ν¨ν μμ μ ν
    - ```CSS
      [disabled] {
        color: red;
      }
      ```
  - [Type]
    - μμ± ABCλ₯Ό ν¬ν¨ν μμ μ ν
  - [ATTR=VALUE]
    - [ABC="XYZ"]
    - μμ± ABCλ₯Ό ν¬ν¨νκ³  κ°μ΄ XYZμΈ μμ μ ν.
    - ```CSS
      [type="password"] {
        color: red;
      }
      ```
