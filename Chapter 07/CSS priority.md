## 💡 선택자 우선순위
- 같은 요소가 여러 선언의 대상이 된 경우, 어떤 선언의 CSS 속성을 우선 적용할지 결정하는 방법
  - 점수가 높은 선언이 우선
  - 점수가 같으면, 가장 마지막에 해석된 선언이 우선
  
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
    color: violet;
  }
  ```
