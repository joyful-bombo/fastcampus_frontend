## 💡 배치
  - ❗ position
    - 요소의 위치 지정 **기준**
    - static
      - 기준 없음
    - relative
      - 요소 **자신**을 기준
    - absolute
      - 위치 상 **부모 요소**를 기준
      - **display 속성이 block으로 변경 됨**
    - fixed
      - **뷰포트**(브라우저)를 기준
      - **display 속성이 block으로 변경 됨**
    - sticky
      - **스크롤 영역** 기준
    - cf) position과 같이 사용하는 CSS 속성
      - **모두 음수를 사용 할 수 있다.**
      - top, bottom, left, right
        - auto
        - 단위
      - z-index
        - 요소의 쌓임 정도를 지정
        - auto
          - 부모 요소와 동일한 쌓임 정도
        - 숫자
          - 숫자가 높을 수록 위에 쌓임
  - ❗ 요소 쌓임 순서(Stack order)
    - **어떤 요소가 사용자와 더 가깝게 있는지(위에 쌓이는지) 결정**
      - 요소에 position 속성의 값이 있는 경우 위에 쌓임.(기본값 static 제외)
      - 1번 조건이 같은 경우, z-index 속성의 숫자 값이 높을 수록 위에 쌓임.
      - 1번 2번 조건까지 같은 경우, HTML의 다음 구조일 수록 위에 쌓임.
