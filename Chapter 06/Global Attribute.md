## π‘ μ μ­ μμ±
- title
  - λ§μ°μ€λ₯Ό κ°μ Έλ€ λμμ λ Tip μ΄ μΆλ ₯ λ.
  - μμμ μ λ³΄λ μ€λͺμ μ§μ 
  ```html
  <a href = " " title = "μ€λͺ"></a>
  ```
- style
  - μμμ μ μ©ν  μ€νμΌ(css)μ μ§μ 
  ```html
  <a href = " " style = "μ€νμΌ"></a>
  ```
- class
  - μμλ₯Ό μ§μΉ­νλ **μ€λ³΅ κ°λ₯**ν μ΄λ¦
  ```html
  <a href = " " class = "μ΄λ¦"></a> 
  
  .μ΄λ¦ {
    color : red;
  }
  ```
- id
  - μμλ₯Ό μ§μΉ­νλ **κ³ μ **ν μ΄λ¦
  ```html
  <a href = "" id = "μ΄λ¦"></a>
  
  #μ΄λ¦ {
    color : blue;
  }
  ```
- data
  - μμμ **λ°μ΄ν°**λ₯Ό μ§μ 
  ```html
  <div data-fruit-name="apple">μ¬κ³Ό</div>
  <div data-fruit-name="banana">λ°λλ</div>
  
  <script defer src="./main.js"></script>
  ```
  ```JS
  const els = document.querySelectorAll('div')
  els.forEach(el => {
    console.log(el.dataset.fruitName)
    })
  ```
 
