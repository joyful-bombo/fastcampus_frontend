## π‘ μ νμ μ°μ μμ
- κ°μ μμκ° μ¬λ¬ μ μΈμ λμμ΄ λ κ²½μ°, μ΄λ€ μ μΈμ CSS μμ±μ μ°μ  μ μ©ν μ§ κ²°μ νλ λ°©λ²
  - μ μκ° λμ μ μΈμ΄ μ°μ 
  - μ μκ° κ°μΌλ©΄, κ°μ₯ λ§μ§λ§μ ν΄μλ μ μΈμ΄ μ°μ 
    - μ μΈ μμμ λ°λΌ μ°μ νλ€.
- μλμ μμλ **λͺμλ**μ΄λ€.
  - CSS μ°μ μμμ μ μλ₯Ό κ³μ°νλ κ²
  - Important ν€μλλ₯Ό μ¬μ©νλ κ²μ **μ€μλ** λΌκ³  λΆλ₯Έλ€.
- ```HTML
  <div
    id="color_yellow"
    class="color_green"
    style="color: orange;"> <!-- 1000μ  -->
    Hello World!
  </div>
  ```
- ```CSS
  div {
    color: red !important; /* infinity */
    }
  #color_yellow {
    color: yellow; /* 100μ  */
  }
  .color_green {
    color: green; /* 10μ  */
  }
  div {
    color: blue; /* 1μ  */
  }
  * {
    color: darkblue; /* 0μ  */
  }
  body {
    color: violet; /* μμX, μ μκ³μ°X */ 
  }
  ```
  
- ## β Example
  - ```CSS
    .list li.item { color: red; } /* .list(10) + li(1) + .item(10) = 21 */
    .list li:hover { color: red; } /* .list(10) + li(1) + :hover(10) = 21 */
    .box::before { content: "Good "; color: red; } /* .box(10) + ::before(1) = 11 */
    #submit span { color: red; } /* #submit(100) + span(1) = 101 */
    header .menu li:nth-child(2) { color: red; } /* header(1) + .menu(10) + li(1) + :nth-child(2) (10) = 22 */
    h1 { color: red; } /* h1 (1) = 1 */
    :not(.box) { color: red; }  /* .box(10), :notμ μ μκ³μ° X = 10 */
    ```
