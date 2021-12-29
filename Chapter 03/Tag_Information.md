## 💡 Title
- HTML 문서의 제목(title)을 정의

## 💡 link
-  **rel** : 가져올 문서와 관계 (relative)
-  **href** : 가져올 문서의 경로 (hypertext reference)
- 외부 문서를 가져와 연결할 때 사용(대부분 css 파일)
- ex)
  ```
  <link rel="icon" href="/favicon.ico" type="image/x-icon">
  <link rel="stylesheet" href="./main.css">
  ```

cf)💡 icon
- **favicon** : Favorite Icon
- Title 옆에 있는 아이콘

## 💡 style
- 스타일(CSS)를 HTML 문서 안에서 작성하는 경우에 사용.

## 💡 script
- **src** : 자바스크립트(JS) 파일 가져오는 경우
``` 
<script src="./main.js"></script>
```
- 자바스크립트(JS)를 HTML 문서 안에서 작성하는 경우
```
<script>
  console.log('Hello World!')
</script>
```
## 💡 meta
- name : 정보의 종류
- content : 정보의 값
- HTML 문서의 제작자, 내용, 키워드 같은 여러 정보를 검색엔진이나 브라우저에게 제공
