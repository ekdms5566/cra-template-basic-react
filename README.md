# Getting Started with Create Basic React App 

리액트 사용 시 필요한 기본 파일만 설치 가능한 custom template  
[npm package](https://www.npmjs.com/package/cra-template-basic-react)
### powershell 명령어
```
$npx create-react-app file_name --template basic-react
```
  
#### 폴더 구조
```
my-app
 ┣ node_modules
 ┃ ┗ ...
 ┣ public
 ┃ ┗ index.html
 ┣ src
 ┃ ┣ App.js
 ┃ ┗ index.js
 ┣ README.md
 ┣ package-lock.json
 ┗ package.json
```

##### index.html
```html
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>React App</title>
</head>
<body>
  <div id="root"></div>
</body>
</html>
```
##### index.js
```js
import React from "react";
// import ReactDOM from 'react-dom'; // 구버전
import { createRoot } from "react-dom/client";
import App from "./App";

const container = document.getElementById("root");
const root = createRoot(container);
root.render(<App />);
```

##### App.js
```js
function App() {
  return (
    <div>
      hello world
    </div>
  );
}
export default App;
```

### Available Scripts
`npx create-react-app`와 동일하게 사용 가능합니다.  
사용가능한 스크립트 명령어는 다음과 같습니다.
```json
"scripts": {
  "start": "react-scripts start",
  "build": "react-scripts build",
  "test": "react-scripts test",
  "eject": "react-scripts eject"
},
```
각 기능에 대한 설명은 [여기](https://create-react-app.dev/docs/getting-started/#scripts)에서 확인할 수 있습니다.
