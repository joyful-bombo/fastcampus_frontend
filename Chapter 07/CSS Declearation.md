## ๐ก ๋ด์ฅ๋ฐฉ์
- html์ head์ ์์ฑ
- `<style></style>`์ ๋ด์ฉ(Contents)์ผ๋ก ์คํ์ผ์ ์์ฑํ๋ ๋ฐฉ์
- ```html
  <style>
    div {
      color: red;
      margin: 20px;
    }
  </style>
  ```

## ๐ก ์ธ๋ผ์ธ ๋ฐฉ์
- ์์์ **style ์์ฑ**์ ์ง์  ์คํ์ผ์ ์์ฑํ๋ ๋ฐฉ์(์ ํ์ ์์)
- ```html
  <div style="color: red; margin: 20px;"></div>
  ```

## ๐ก ๋งํฌ ๋ฐฉ์
- **๋ณ๋ ฌ** ์ฐ๊ฒฐ
- `<link />`๋ก ์ธ๋ถ CSS ๋ฌธ์๋ฅผ ๊ฐ์ ธ์์ ์ฐ๊ฒฐํ๋ ๋ฐฉ์
- ```html
  <link rel="stylesheet" href="./main.css">
  ```

## ๐ก @import ๋ฐฉ์
- **์ง๋ ฌ** ์ฐ๊ฒฐ
- CSS์ @import ๊ท์น์ผ๋ก CSS ๋ฌธ์ ์์์ ๋ ๋ค๋ฅธ CSS ๋ฌธ์๋ฅผ ๊ฐ์ ธ์ ์ฐ๊ฒฐํ๋ ๋ฐฉ์
- ```html
  <link rel ="stylesheet" href="./css/main.css">
  ```
  ```css
  /* main.css */
  @import url("./box.css");
  
  div {
    color: red;
    margin: 20px;
  }
  ```
  ```css
  /* box.css */
  .box {
    background-color: red;
    padding: 20px;
  }
  ```
