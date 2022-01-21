## 💡 스타일 상속
- ```css
  .animal {
    color: red;
  }
  
  <div class="ecosystem">생태계
    <div class="animal">동물
      <div class="tiger">호랑이</div>
      <div class="lion">사자</div>
      <div class="elephant">코끼리</div>
    </div>
    <div class="plant">식물</div>
  </div>
  ```
- 부모의 스타일이 하위 요소까지 상속되는 것을 의미한다.
- 상속되는 CSS 속성들
  - **모두 글자/문자 관련 속성들!** 단, 모든 글자/문자 속성은 아님
  - font-style : 글자 기울기
  - font-weight : 글자 두께
  - font-size : 글자 크기
  - line-height : 줄 높이
  - font-family : 폰트(서체)
  - color : 글자 색상
  - text-align : 정렬 
  - 등등

## 💡 강제 상속
  - ```
    .tiger {
      color: inherit; /* 상속 */
    }
    ```
