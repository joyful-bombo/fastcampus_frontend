# 💡 변수
- 데이터를 저장하고 참조(사용)하는 **데이터의 이름**
- **var, let, const**
- var은 권장하지 않음.
---
## 💡 let
```JS
// 재사용이 가능!
// 변수 선언
let a = 2;
let b = 5;

console.log(a + b); // 7
console.log(a - b); // -3
console.log(a * b); // 10
console.log(a / b); // 0.4

let a = 12; // 변수 선언
console.log(a); // 12

a = 999; // 재할당
console.log(a); // 999

// 값(데이터)의 재할당 가능!
```
---
## 💡 const
```JS
// 값(데이터)의 재할당 불가능!
const a = 12; // 상수 선언
console.log(a); // 12

a = 999;
console.log(a); // TypeError: Assignment to constant variable.
```
---
# 💡 예약어(Reserved Word)
- **특별한 의미**를 가지고 있어, 변수나 함수 이름 등으로 사용할 수 없는 단어
---
```JS
let this = 'Hello!'; // Syntax Error
let if = 123; // Syntax Error
let break = true; // Syntax Error
```
