## 💡 내장방식
- html의 head에 작성
- `<style></style>`의 내용(Contents)으로 스타일을 작성하는 방식
- ```html
  <style>
    div {
      color: red;
      margin: 20px;
    }
  </style>
  ```

## 💡 인라인 방식
- 요소의 **style 속성**에 직접 스타일을 작성하는 방식(선택자 없음)
- ```html
  <div style="color: red; margin: 20px;"></div>
  ```

## 💡 링크 방식
- **병렬** 연결
- `<link />`로 외부 CSS 문서를 가져와서 연결하는 방식
- ```html
  <link rel="stylesheet" href="./main.css">
  ```

## 💡 @import 방식
- **직렬** 연결
- CSS의 @import 규칙으로 CSS 문서 안에서 또 다른 CSS 문서를 가져와 연결하는 방식
- ```html
  <link rel ="stylesheet" href="./css/main.css">
  ```
  ```css
  @import url("./box.css");
  
  div {
    color: red;
    margin: 20px;
  }
  ```
  ```css
  .box {
    background-color: red;
    padding: 20px;
  }
  ```
