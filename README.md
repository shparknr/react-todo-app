# 할 일 앱 만들기

## 리액트 프로젝트 세팅
- npm으로 설치 한 경우 yarn add 대신에 npm i(nstall)
- `yarn create react-app ./`         (`npx create-react-app ./`)
- `yarn add normalize.css`           (`npm i normalize.css`)
- `yarn add sass`                    (`npm i sass`)
- `yarn add classnames react-icons`  (`npm i classnames react-icons`)

## ESLint, prettier 설정
- ./ (제일 상위폴더)
- ./.prettierrc.json (.prettierrc.json 폴더생성)

```json
{
  "singleQuote": false,
  "semi": true,
  "useTabs": false,
  "tabWidth": 2,
  "trailingComma": "all",
  "printWidth": 80,
  "arrowParens": "avoid",
  "endOfLine": "auto"
}
```

- `yarn add eslint --dev`         (`npm i eslint --dev`)
- `yarn eslint --init`            (`npx eslint --init`)
- `yarn add eslint-config-prettier --save-dev`
 (`npm install eslint-config-prettier --save-dev`)
-
- json (.eslintrc.js)
```json (.eslintrc.js)
"extends": [
        "eslint:recommended",
        "plugin:react/recommended",
        "prettier"
    ],



    rules: {
  "react/react-in-jsx-scope": "off",
  "react/prop-types": "off",
  "no-unused-vars": "off",
},
```

- css (index.css)
```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  outline-style: none;
}
ul,
li {
  list-style: none;
}
a {
  color: #000000;
  text-decoration: none;
}
img {
  vertical-align: middle;
  border: 0;
}
html {
  font-size: 16px;
}
body {
  font-family: "Pretendard-Regular", sans-serif;
  font-size: 1rem;
  line-height: 1.25;
  letter-spacing: -0.23px;
  word-break: keep-all;
  color: #000000;
}
```

- `yarn add @babel/plugin-proposal-private-property-in-object --dev`
  (`npm install @babel/plugin-proposal-private-property-in-object --dev`)