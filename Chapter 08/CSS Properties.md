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
  - width, height
    - 요소의 가로/세로 너비
    - Default Value
      - auto
        - 브라우저가 너비를 계산
      - 단위
        - px, em, vw 등 단위로 지정
    - max-width, max-height
      - 요소가 커질 수 있는 **최대** 가로/세로 너비
        - none
          - 최대 너비 제한 없음
        - auto
          - 브라우저가 너비를 계산
        - 단위
          - px, em, vw 등 단위로 지정
    - min-width, min-height
      - 요소가 작아질 수 있는 **최소** 가로/세로 너비
        - 0
          - 최소 너비 제한 없음
        - auto
          - 브라우저가 너비를 계산
        - 단위
          - px, em, vw등 단위로 지정
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
