# π‘ ν¨μ
- νΉμ  λμ(κΈ°λ₯)μ μννλ μΌλΆ μ½λμ **μ§ν©**(λΆλΆ)
- **function**
---
```JS
// ν¨μ μ μΈ
function helloFunc() {
  // μ€ν μ½λ
  console.log(1234);
}

// ν¨μ νΈμΆ
helloFunc(); // 1234
```
```JS
function returnFunc() {
  return 123;
}

let a = returnFunc();

console.log(a); // 123
```
```JS
function sum(a, b) { // aμ bλ λ§€κ°λ³μ(Parameters)
  return a + b;
}

// μ¬μ¬μ© !
let a = sum(1, 2); // 1κ³Ό 2λ μΈμ(Arguments)
let b = sum(7, 12);
let c = sum(2, 4);

console.log(a, b, c); // 3, 19, 6
```

```JS
// κΈ°λͺ(μ΄λ¦μ΄ μλ) ν¨μ
function hello() {
  console.log('Hello~');
}

// μ΅λͺ(μ΄λ¦μ΄ μλ) ν¨μ
let world = function () {
  console.log('World~');
  // Hoistingκ³Ό μ°κ΄μ΄ λμ΄ μλ€.
}

// ν¨μ νΈμΆ!
hello(); // Hello~
world(); // World~
```
```JS
const bombo = {
  name: 'Bombo',
  age: 27,
  // λ©μλ(Method)
  getName: function () {
    return this.name;
  }
};

const hisName = bombo.getName();
console.log(hisName); // Bombo
console.log(bombo.getName()); // Bombo
```
