# 💡 조건문
- 조건의 결과(true, false)에 따라 다른 코드를 실행하는 구문
- **if, else**
```JS
let isShow = true;
let checked = false;

if (isShow) { // true
  console.log('Show!'); // Show!
}

if (checked) { // false
  console.log('Checked!');
}
```

```JS
let isShow = true;

if (isShow) { // true
  console.log('Show!');
} else { // false
  console.log('Hide?');
}

isShow = false;

if (isShow) { // false
  console.log('Show!');
} else { // true
  console.log('Hide?');
}
```
