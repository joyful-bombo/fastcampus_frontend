# π‘ λ³μ
- λ°μ΄ν°λ₯Ό μ μ₯νκ³  μ°Έμ‘°(μ¬μ©)νλ **λ°μ΄ν°μ μ΄λ¦**
- **var, let, const**
- varμ κΆμ₯νμ§ μμ.
---
## π‘ let
```JS
// μ¬μ¬μ©μ΄ κ°λ₯!
// λ³μ μ μΈ
let a = 2;
let b = 5;

console.log(a + b); // 7
console.log(a - b); // -3
console.log(a * b); // 10
console.log(a / b); // 0.4

let a = 12; // λ³μ μ μΈ
console.log(a); // 12

a = 999; // μ¬ν λΉ
console.log(a); // 999

// κ°(λ°μ΄ν°)μ μ¬ν λΉ κ°λ₯!
```
---
## π‘ const
```JS
// κ°(λ°μ΄ν°)μ μ¬ν λΉ λΆκ°λ₯!
const a = 12; // μμ μ μΈ
console.log(a); // 12

a = 999;
console.log(a); // TypeError: Assignment to constant variable.
```
---
# π‘ μμ½μ΄(Reserved Word)
- **νΉλ³ν μλ―Έ**λ₯Ό κ°μ§κ³  μμ΄, λ³μλ ν¨μ μ΄λ¦ λ±μΌλ‘ μ¬μ©ν  μ μλ λ¨μ΄
---
```JS
let this = 'Hello!'; // Syntax Error
let if = 123; // Syntax Error
let break = true; // Syntax Error
```
