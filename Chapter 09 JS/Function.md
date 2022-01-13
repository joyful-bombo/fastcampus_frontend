# 💡 함수
- 특정 동작(기능)을 수행하는 일부 코드의 **집합**(부분)
- function
---
```JS
// 함수 선언
function helloFunc() {
  // 실행 코드
  console.log(1234);
}

// 함수 호출
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
function sum(a, b) { // a와 b는 매개변수(Parameters)
  return a + b;
}

// 재사용 !
let a = sum(1, 2); // 1과 2는 인수(Arguments)
let b = sum(7, 12);
let c = sum(2, 4);

console.log(a, b, c); // 3, 19, 6
```
```JS
// 기명(이름이 있는) 함수
function hello() {
  console.log('Hello~');
}

// 익명(이름이 없는) 함수
let world = function () {
  console.log('World~');
  // Hoisting과 연관이 되어 있다.
}

// 함수 호출!
hello(); // Hello~
world(); // World~
```
```JS
const bombo = {
  name: 'Bombo',
  age: 27,
  // 메소드(Method)
  getName: function () {
    return this.name;
  }
};

const hisName = bombo.getName();
console.log(hisName); // Bombo
console.log(bombo.getName()); // Bombo
```
