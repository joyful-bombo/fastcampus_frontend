# π‘ DOM API
(Document Object Model, Application Programming Interface)
---
## π‘ Document
- **HTML**

## π‘ Object
- **div, span, input**
---
```JS
// HTML μμ(Element) 1κ° κ²μ/μ°ΎκΈ°, μ μΌ λ¨Όμ  μ°Ύμμ§λ μμ
const boxEl = document.querySelector('.box');

// HTML μμμ μ μ©ν  μ μλ λ©μλ!
boxEl.addEventListener();

// μΈμ(Arguments)λ₯Ό μΆκ° κ°λ₯!
boxEl.addEventListener(1, 2);

// 1 - μ΄λ²€νΈ(Event, μν©)
boxEl.addEventListener('click', 2);

// 2 - νΈλ€λ¬(Handler, μ€νν  ν¨μ)
boxEl.addEventListener('click', function () {
  console.log('Click~!');
});

// μμμ ν΄λμ€ μ λ³΄ κ°μ²΄ νμ©!
boxEl.classList.add('active');
let isContains = boxEl.classList.contains('active');
console.log(isContains); // true

boxEl.classlist.remove('active');
isContains = boxEl.classList.contains('active');
console.log(isContains); // false
```
---
```JS
// HTML μμ(Element) λͺ¨λ κ²μ/μ°ΎκΈ°
const boxEls = documnet.querySelectorAll('.box');
console.log(boxEls);

// μ°Ύμ μμλ€ λ°λ³΅ν΄μ ν¨μ μ€ν!
// μ΅λͺ ν¨μλ₯Ό μΈμλ‘ μΆκ°!
boxEls.forEach(function () {});

// μ²« λ²μ§Έ λ§€κ°λ³μ(boxEl): λ°λ³΅ μ€μΈ μμ
// λ λ²μ§Έ λ§€κ°λ³μ(index): λ°λ³΅ μ€μΈ λ²νΈ
boxEls.forEach(function (boxEl, index) {} );

// μΆλ ₯!
boxEls.forEach(function(boxEl, index) {
  boxEl.classList.add(`order-${index + 1}`);
  console.log(index, boxEl);
});
```
---
```JS
const boxEl = document.querySelector('.box');

// Getter, κ°μ μ»λ μ©λ
console.log(boxEl.textContent); // Box!!

// Setter, κ°μ μ§μ νλ μ©λ
boxEl.textContent = 'Bombo!?';
console.log(boxEl.textContent); // Bombo!?
```
