## 💡 전환
---
- ## ❗ transition
  - 요소의 **전환(시작과 끝) 효과**를 지정하는 **단축 속성**
  - ```CSS
    transition: 속성명 지속시간 타이밍함수 대기시간;
    /* transition-property, transition-duration, transition-timing-function, transition-delay */
    /* transition-duration(지속시간) : 필수 속성 */
    ```
- ❗transition-property
  - 전환 효과를 사용할 **속성 이름**을 지정
  - all
    - 모든 속성에 적용
  - 속성이름
    - 전환 효과를 사용할 속성 이름 명시
- ❗transition-duration
  - **전환 효과**의 **지속시간**을 지정
  - 0s
    - 전환 효과 없음
  - 시간
    - 지속시간(s)을 지정
    - 0.5s == .5s
- ❗transition-timing-function
  - 전환 효과의 **타이밍(Easing)** 함수를 지정
  - ease
    - 느리게 -> 빠르게 -> 느리게 == cubic-bezier(0.25, 0.1, 0.25, 1)
  - linear
    - 일정하게 == cubic-bezier(0, 0, 1, 1)
  - ease-in
    - 느리게 -> 빠르게 == cubic-bezier(0.42, 0, 1, 1)
  - ease-out
    - 빠르게 -> 느리게 == cubic-bezier(0, 0, 0.58, 1)
  - ease-in-out
    - 느리게 -> 빠르게 -> 느리게 == cubic-bezier(0.42, 0, 0.58, 1)
  - cubic-bezier(n,n,n,n)
    - 자신만의 값을 정의(0~1)
    - 복잡해서 잘 사용하지 않음
  - steps(n)
    - n번 분할된 애니메이션
  - cf) easing functions, easing functions mdn, tweenmax easing
- ❗transition-delay
  - 전환 효과가 몇 초 뒤에 시작할지 대기시간을 지정
  - 0s
    - 대기시간 없음
  - 시간
    - 지속시간(s)을 지정
