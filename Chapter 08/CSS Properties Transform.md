## 💡 변환
---
- ❗ transform
  - 요소의 **변환 효과**
  - ```CSS
    transform: 변환함수1 변환함수2 변환함수3 ...;
    transform: 원근법 이동 크기 회전 기울임;
    ```
  - ## ❗ 2D 변환 함수
  - **단위 px**
    - translate(x, y)
      - 이동(x축, y축)
    - translateX(x)
      - 이동(x축)
    - translateY(y)
      - 이동(y축)
  - **없음(배수)**
    - scale(x, y)
      - 크기(x축, y축)
  - **단위 deg**
    - rotate(degree)
      - 회전(각도)
    - skewX(x)
      - 기울임(x축)
      - 마름모 모양
    - skewY(y)
      - 기울임(y축)
      - 마름모 모양
  - matrix
    - matrix(n, n, n, n, n, n)
      - 2차원 변환 효과
  - ## ❗ 3D 변환 함수
  - perspective(n)
    - 하위 요소를 관찰하는 **원근 거리**를 지정
    - 원근법(거리)
    - **제일 앞에 작성해야 한다**
    - 기준점
      - transform-origin
    - 단위 px
  - rotateX(x)
    - 회전(x축기준)
    - 단위 deg
  - rotateY(y)
    - 회전(y축기준)
    - 단위 deg
  - backface-visibility
    - 3D 변환으로 회전된 요소의 **뒷면 숨김 여부**
    - visible
      - 뒷면 보임
    - hidden
      - 뒷면 숨김
## 💡 perspective
  - 관찰 대상의 부모에게 **원근 거리 지정**
  - transform의 perspective 함수와 다름
  - 기준점
    - perspective-origin

