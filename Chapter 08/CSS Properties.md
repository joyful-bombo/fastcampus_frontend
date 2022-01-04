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
  - 단위
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
## 💡 글꼴, 문자

## 💡 배경

## 💡 배치

## 💡 플렉스(정렬)-수평 정렬

## 💡 전환

## 💡 변환

## 💡 띄움

## 💡 애니메이션

## 💡 그리드

## 💡 다단

## 💡 필터
