# 💡 Data Type(자료형)
---
## 💡 String(문자 데이터)
```JS
//따옴표를 사용한다.
let myName = "Bombo";
let email = "bomboTest@naver.com";
let hello = `Hello ${myName}!?` // `...${Variable}` : 보간법

console.log(myName);
console.log(email);
console.hog(hello);
```
---
## 💡 Number(숫자 데이터)
```JS
// 정수 및 부동소수점 숫자를 나타냅니다.
let number = 123;
let opacity = 1.57;

console.log(number);
console.log(opacity);
```
---
## 💡 Boolean(불린 데이터)
```JS
// true, false 두 가지 값 밖에 없는 논리 데이터입니다.
let checked = true;
let isShow = false;

console.log(checked);
console.log(isShow);
```
---
## 💡 Undefined
```JS
// 값이 할당되지 않은 상태를 나타냅니다.
let undef;
let obj = { abc: 123 };

console.log(undef); // undefined
console.log(obj.abc); // 123
console.log(obj.xyz); // undefined
```
---
## 💡 Null
```JS
// 어떤 값이 의도적으로 비어있음을 의미합니다.
let empty = null; // 명시적 null
console.log(empty); // null
```
---
## 💡 Object(객체 데이터)
```JS
// 여러 데이터를 Key:Value 형태로 저장합니다. { Key: Value}
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
## 💡 Array(배열 데이터)
```JS
// 여러 데이터를 순차적으로 저장합니다. [ ]
let fruits = ['Apple', 'Banana', 'Cherry'];

console.log(fruits[0]);
console.log(fruits[1]);
console.log(fruits[2]);
```
