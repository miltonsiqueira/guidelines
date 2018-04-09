# ESLint

[ESLint](https://eslint.org/docs/user-guide/getting-started) is a tool for identifying and reporting on patterns found in ECMAScript/JavaScript code, with the goal of making code more consistent and avoiding bugs. In many ways, it is similar to JSLint and JSHint with a few exceptions:

* ESLint uses Espree for JavaScript parsing.
* ESLint uses an AST to evaluate patterns in code.
* ESLint is completely pluggable, every single rule is a plugin and you can add more at runtime.

## Usage

* Install eslint globally `npm intall eslint -g` or locally `npm intall eslint --save-dev`

* Use Airbnb style guide
  * Install globally `npm install -g eslint-config-airbnb` or locally `npm intall eslint-config-airbnb --save-dev`
  * Add [.eslintrc](.eslintrc.json) in your root project folder.

## Extensions for Visual Code

* [Eslint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
