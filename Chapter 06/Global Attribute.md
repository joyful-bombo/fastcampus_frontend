## 💡 전역 속성
- title
  - 마우스를 가져다 되었을 때 Tip 이 출력 됌.
  - 요소의 정보나 설명을 지정
  ```html
  <a href = " " title = "설명"></a>
  ```
- style
  - 요소에 적용할 스타일(css)을 지정
  ```html
  <a href = " " style = "스타일"></a>
  ```
- class
  - 요소를 지칭하는 **중복 가능**한 이름
  ```html
  <a href = " " class = "이름"></a> 
  
  .이름 {
    color : red;
  }
  ```
- id
  - 요소를 지칭하는 **고유**한 이름
  ```html
  <a href = "" id = "이름"></a>
  
  #이름 {
    color : blue;
  }
  ```
- data
  - 요소에 **데이터**를 지정
  ```html
  <div data-fruit-name="apple">사과</div>
  <div data-fruit-name="banana">바나나</div>
  
  <script defer src="./main.js"></script>
  ```
  ```JS
  const els = document.querySelectorAll('div')
  els.forEach(el => {
    console.log(el.dataset.fruitName)
    })
  ```
 
