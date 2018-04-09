# ESLint

[ESLint](https://eslint.org/docs/user-guide/getting-started) is a tool for identifying and reporting on patterns found in ECMAScript/JavaScript code, with the goal of making code more consistent and avoiding bugs. In many ways, it is similar to JSLint and JSHint with a few exceptions:

* ESLint uses Espree for JavaScript parsing.
* ESLint uses an AST to evaluate patterns in code.
* ESLint is completely pluggable, every single rule is a plugin and you can add more at runtime.

## Usage

* Install eslint globally `npm install -g eslint eslint-plugin-import` or locally `npm install --save-dev eslint eslint-plugin-import`

* Use Airbnb style guide

  * Install globally `npm install -g eslint-config-airbnb eslint-config-airbnb-base` or locally `npm intall --save-dev eslint-config-airbnb eslint-config-airbnb-base`
  * Add [.eslintrc](.eslintrc.json) in your root project folder.

* Prettier integration `npm install -g prettier eslint-plugin-prettier` or `npm intall --save-dev eslint-plugin-prettier`

## Extensions for Visual Code

* [Eslint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
