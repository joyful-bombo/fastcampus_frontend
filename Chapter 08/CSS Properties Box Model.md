## 💡 CSS 속성 개요
  - 박스 모델
  - 글꼴, 문자
  - 배경
  - 배치
  - 플렉스(정렬)
  - 전환
  - 변환
  - 띄움
  - 애니메이션
  - 그리드
  - 다단
  - 필터

## 💡 CSS 표현 단위
  - ## ❗ 단위
    - px
      - 픽셀
      - 화면에 출력하는 한개의 점
    - %
      - 상대적 백분율
    - em
      - 요소의 글꼴 크키
      - 어떤 글꼴의 크기가 10px이라면 1em == 10px
    - rem
      - 루트 요소(html)의 글꼴 크기
      - 최상위 요소(root)
    - vw
      - 뷰포트 가로 너비의 백분율
    - vh
      - 뷰포트 세로 너비의 백분율
  - **❗html 기본 폰트 사이즈**
    - 16px
## 💡 박스 모델
  - ```HTML
    <div></div>
    <span></span>
    ```
    
    ```CSS
    div { /* 블록요소 */
      width: 100px; /* 가로너비, 없으면 parent */
      height: 100px; /* 세로너비, 없으면 0 */
      background-color: orange;
    }
    
    span { /* 인라인요소 */
      background-color: orange;
      /* 가로너비와 세로너비가 콘텐츠 요소에 맞게 줄어듬 */
    }
    ```
  - ## ❗ width, height
    - 요소의 가로/세로 너비
    - Default Value
      - auto
        - 브라우저가 너비를 계산
      - 단위
        - px, em, vw 등 단위로 지정
    - **max-width, max-height**
      - 요소가 커질 수 있는 **최대** 가로/세로 너비
        - none
          - 최대 너비 제한 없음
        - auto
          - 브라우저가 너비를 계산
        - 단위
          - px, em, vw 등 단위로 지정
    - **min-width, min-height**
      - 요소가 작아질 수 있는 **최소** 가로/세로 너비
        - 0
          - 최소 너비 제한 없음
        - auto
          - 브라우저가 너비를 계산
        - 단위
          - px, em, vw등 단위로 지정
  - ## ❗ margin
    - 요소의 **외부** 여백(공간)을 지정하는 **단축 속성**
    - **음수를 사용할 수 있다.**
    - 0
      - 외부 여백 없음
    - auto
      - 브라우저가 여백을 계산
      - 가로(세로) 너비가 있는 요소의 **가운데 정렬**에 활용!
    - 단위
      - px, ex, vw 등 단위로 지정
    - %
      - 부모 요소의 **가로 너비**에 대한 비율로 지정
      - 잘 사용하지 않음
    - ```CSS
      margin: 20px; /* Top, Bottom, Left, Right 20px */
      margin: 10px 20px; /* Top, Bottom 10px & Left, Right 20px */ 
      margin: 10px 20px 30px; /* Top 10px & Left, Right 20px & Bottom 30px */
      margin: 10px 20px 30px 40px; /* Top 10px & Right 20px & Bottom 30px & Left 40px */
      ```
    - margin-방향
      - 요소의 외부 여백(공간)을 지정하는 기타 **개별 속성**들
        - margin-top
        - margin-bottom
        - margin-left
        - margin-right
  - ## ❗ Padding
    - 요소의 **내부 여백(공간)**을 지정하는 단축 속성
    - **요소의 크기가 커진다.**
      - 0
        - 내부 여백 없음
      - 단위
        - px, em, vw 등 단위로 지정
      - %
        - 부모 요소의 **가로 너비**에 대한 비율로 지정
    - ```CSS
      padding: 20px; /* Top, Bottom, Left, Right 20px */
      padding: 10px 20px; /* Top, Bottom 10px & Left, Right 20px */ 
      padding: 10px 20px 30px; /* Top 10px & Left, Right 20px & Bottom 30px */
      padding: 10px 20px 30px 40px; /* Top 10px & Right 20px & Bottom 30px & Left 40px */
      ```
    - padding-방향
      - 요소의 외부 여백(공간)을 지정하는 기타 **개별 속성**들
        - padding-top
        - padding-bottom
        - padding-left
        - padding-right
  - ## ❗ border
    - 요소의 **테두리 선**을 지정하는 **단축 속성**
    - border: 선-두께 선-종류 선-색상;
    - ```CSS
      border: border-width, border-style, border-color;
      ```
    - default Value
      - medium, none, black
    - **border-width**
      - medium(중간두께)
      - thin(얇은 두께)
      - thick(두꺼운 두께)
      - 단위
        - px, em, % 등 단위로 지정
      - 단축 속성 적용 가능
      - ```CSS
        border-width: 10px;
        border-width: 10px 10px;
        border-width: 10px 20px 30px;
        border-width: 10px 20px 30px 40px;
        ```
    - **border-style**
      - none : 선 없음
      - solid : 실선
      - dotted : 점선
      - dashed : 파선
      - double : 두 줄 선
      - groove : 홈이 파여있는 모양
      - ridge : 솟은 모양
      - inset : 요소 전체가 들어간 모양
      - outset : 요소 전체가 나온 모양
      - ```CSS
        border-style: 10px;
        border-style: 10px 10px;
        border-style: 10px 20px 30px;
        border-style: 10px 20px 30px 40px;
        ```
    - **border-color**
      - black
      - 색상
      - transparent(투명도)
      - ```CSS
        border-color: 10px;
        border-color: 10px 10px;
        border-color: 10px 20px 30px;
        border-color: 10px 20px 30px 40px;
        ```
- ## ❗ 색상표현
  - 색상 이름
    - 브라우저에서 제공하는 색상 이름
    - red, tomato, royalblue
  - Hex 색상코드
    - 16진수 색상(Hexadecimal Colors)
    - #000, #FFFFFF
  - RGB
    - 빛의 삼원색
    - rgb(255, 255, 255)
  - RGBA
    - 빛의 삼원색 + 투명도 
    - rgba(0, 0, 0, 0.5)
  - HSL
    - 색상, 채도, 명도
    - hsl(120, 100%, 50%)
  - HSLA
    - 색상, 채도, 명도 + 투명도
    - hsla(120, 100%, 50%, 0.3)
  - border-방향
  - border-방향-속성
  - ```CSS
    border-top: 두께 종류 색상;
    border-top-width: 두께;
    border-top-style: 종류;
    border-top-color: 색상;
    ```
- ## ❗ border-radius
  - 요소의 모서리를 둥글게 깎음
  - 0
    - 둥글게 없음
  - 단위
    - px, em, vw등 단위로 지정
- ## ❗ box-sizing
  - content-box
    - 요소의 내용(content)으로 크기 계산
    - 수동 계산
  - border-box
    - 요소의 내용 + padding + border로 크기 계산
- ## ❗ overflow
  - 요소의 크기 이상으로 **내용이 넘쳤을 때, 보여짐을 제어하는 단축 속성**
  - visible
    - 넘친 내용을 그대로 보여줌
  - hidden
    - 넘친 내용을 잘라냄
  - scroll
    - 넘친 내용을 잘라냄, 스크롤바 생성
  - auto
    - 넘친 내용이 있는 경우에만 잘라내고 스크롤바 생성
  - **개별 속성**
    - overflow-x
    - overflow-y
- ## ❗ display
  - 요소의 화면 **출력(보여짐) 특성**
---
  - block
    - 상자(레이아웃) 요소
  - inline
    - 글자 요소
  - inline-block
    - 글자 + 상자 요소
  - **각 요소에 이미 지정되어 있는 값**
---
  - flex
    - 플렉스 박스 (1차원 레이아웃)
  - grid
    - 그리드 (2차원 레이아웃)
  - none
    - 보여짐 특성 없음, 화면에서 사라짐
  - 기타
    - table, table-row, table-cell 등등
  - **따로 지정해서 사용하는 값**
  
  - ## ❗ Opacity
    - 요소 투명도
    - 1
      - 불투명
    - 0 ~ 1
      - 0부터 1 사이의 소수점 숫자
