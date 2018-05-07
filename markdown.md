# Markdown

## Extensions for Microsoft Visual Code

* Install [Prettier extension](prettier.md).
* [markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint).
  * Remove the rule [MD030](https://github.com/DavidAnson/markdownlint/blob/v0.8.1/doc/Rules.md#md030),
    because `Prettier` always put [double spaces in ordered list](https://github.com/prettier/prettier/issues/4114).
    Update file `.markdownlint.json` in your project root folder:

```json
{
  "MD030": false
}
```
