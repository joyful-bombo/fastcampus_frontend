## 💡 선택자 우선순위
- 같은 요소가 여러 선언의 대상이 된 경우, 어떤 선언의 CSS 속성을 우선 적용할지 결정하는 방법
  - 점수가 높은 선언이 우선
  - 점수가 같으면, 가장 마지막에 해석된 선언이 우선
    - 선언 순서에 따라 우선한다.
- 아래의 예시는 **명시도**이다.
  - CSS 우선순위의 점수를 계산하는 것
  - Important 키워드를 사용하는 것을 **중요도** 라고 부른다.
- ```HTML
  <div
    id="color_yellow"
    class="color_green"
    style="color: orange;"> <!-- 1000점 -->
    Hello World!
  </div>
  ```
- ```CSS
  div {
    color: red !important; /* infinity */
    }
  #color_yellow {
    color: yellow; /* 100점 */
  }
  .color_green {
    color: green; /* 10점 */
  }
  div {
    color: blue; /* 1점 */
  }
  * {
    color: darkblue; /* 0점 */
  }
  body {
    color: violet; /* 상속X, 점수계산X */ 
  }
  ```
  
- ## ❗ Example
  - ```CSS
    .list li.item { color: red; } /* .list(10) + li(1) + .item(10) = 21 */
    .list li:hover { color: red; } /* .list(10) + li(1) + :hover(10) = 21 */
    .box::before { content: "Good "; color: red; } /* .box(10) + ::before(1) = 11 */
    #submit span { color: red; } /* #submit(100) + span(1) = 101 */
    header .menu li:nth-child(2) { color: red; } /* header(1) + .menu(10) + li(1) + :nth-child(2) (10) = 22 */
    h1 { color: red; } /* h1 (1) = 1 */
    :not(.box) { color: red; }  /* .box(10), :not은 점수계산 X = 10 */
    ```
