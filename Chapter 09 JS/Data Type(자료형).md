# π‘ Data Type(μλ£ν)
---
## π‘ String(λ¬Έμ λ°μ΄ν°)
```JS
//λ°μ΄νλ₯Ό μ¬μ©νλ€.
let myName = "Bombo";
let email = "bomboTest@naver.com";
let hello = `Hello ${myName}!?` // `...${Variable}` : λ³΄κ°λ²

console.log(myName);
console.log(email);
console.hog(hello);
```
---
## π‘ Number(μ«μ λ°μ΄ν°)
```JS
// μ μ λ° λΆλμμμ  μ«μλ₯Ό λνλλλ€.
let number = 123;
let opacity = 1.57;

console.log(number);
console.log(opacity);
```
---
## π‘ Boolean(λΆλ¦° λ°μ΄ν°)
```JS
// true, false λ κ°μ§ κ° λ°μ μλ λΌλ¦¬ λ°μ΄ν°μλλ€.
let checked = true;
let isShow = false;

console.log(checked);
console.log(isShow);
```
---
## π‘ Undefined
```JS
// κ°μ΄ ν λΉλμ§ μμ μνλ₯Ό λνλλλ€.
let undef;
let obj = { abc: 123 };

console.log(undef); // undefined
console.log(obj.abc); // 123
console.log(obj.xyz); // undefined
```
---
## π‘ Null
```JS
// μ΄λ€ κ°μ΄ μλμ μΌλ‘ λΉμ΄μμμ μλ―Έν©λλ€.
let empty = null; // λͺμμ  null
console.log(empty); // null
```
---
## π‘ Object(κ°μ²΄ λ°μ΄ν°)
```JS
// μ¬λ¬ λ°μ΄ν°λ₯Ό Key:Value ννλ‘ μ μ₯ν©λλ€. { Key: Value}
let user = {
  name: 'Bombo',
  age: 27,
  isValid: true
};

console.log(user.name); 
console.log(user.age); 
console.log(user.isValid);
```
---
## π‘ Array(λ°°μ΄ λ°μ΄ν°)
```JS
// μ¬λ¬ λ°μ΄ν°λ₯Ό μμ°¨μ μΌλ‘ μ μ₯ν©λλ€. [ ]
let fruits = ['Apple', 'Banana', 'Cherry'];

console.log(fruits[0]);
console.log(fruits[1]);
console.log(fruits[2]);
```
