# ESLint

[ESLint](https://eslint.org/docs/user-guide/getting-started) is a tool for identifying and reporting on patterns found in ECMAScript/JavaScript code, with the goal of making code more consistent and avoiding bugs. In many ways, it is similar to JSLint and JSHint with a few exceptions:

* ESLint uses Espree for JavaScript parsing.
* ESLint uses an AST to evaluate patterns in code.
* ESLint is completely pluggable, every single rule is a plugin and you can add more at runtime.

## Configuration file .eslintrc

* The file can be one of them:
  * JSON file: `.eslint.json`
  * JS file: `.eslint.js`
  * YAML: `.eslint.yml`

## Install

Global install:

```bash
npm install -g eslint eslint-plugin-import
```

Local install:

```bash
npm install --save-dev eslint eslint-plugin-import
```

## Style guide

Use the `eslint:recommended` for configuration.

```json
{
  "extends": ["eslint:recommended"]
}
```

Or use this [file](.eslintrc.json).

## Prettier integration

Global install:

```bash
npm install -g prettier eslint-plugin-prettier
```

Local install:

```bash
npm install --save-dev eslint-plugin-prettierr
```

Update your configuration file with:

```json
{
  "extends": ["eslint:recommended", "prettier"],
  "plugins": ["prettier"]
}
```

Or use this [file](.eslintrc.json).

## Node integration

Global install:

```bash
npm install -g eslint eslint-plugin-node
```

Local install:

```bash
npm install --save-dev eslint eslint-plugin-node
```

Update your configuration file with:

```json
{
  "extends": ["eslint:recommended"],
  "plugins": ["node"]
}
```

Or use this [file](.eslintrc.json).

## Extensions for Visual Code

* [Eslint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
