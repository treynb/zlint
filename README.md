## 简介

React Typescript Eslint 配置

## 安装

```
npm i @treynb/eslint-config-zlint -D
```

## 依赖

```
"peerDependencies": {
  "eslint": "^7.4.0"
}
```

## 使用

在项目中添加 .eslintrc.js

```
module.exports = {
  extends: [
    '@treynb/zlint'
  ],
  rules: {

  },
};
```

默认集成了 prettier，添加 .prettierrc

```
{
  "printWidth": 100,
  "tabWidth": 2,
  "useTabs": false,
  "semi": true,
  "singleQuote": true,
  "quoteProps": "as-needed",
  "jsxSingleQuote": false,
  "trailingComma": "all",
  "bracketSpacing": true,
  "jsxBracketSameLine": false,
  "arrowParens": "always",
  "parser": "babel-ts",
  "endOfLine": "lf",
  "requirePragma": false,
  "insertPragma": false,
  "proseWrap": "preserve"
}
```

添加 scripts

```
"scripts": {
  "lint": "eslint src --ext .tsx,.ts"
}
```

进行代码检查

```
npm run lint
```
