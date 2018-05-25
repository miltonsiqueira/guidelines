# Git

## Diff with .docx files

* [Install Pandoc](http://pandoc.org/installing.html)
* Create or edit file `.gitconfig`
  * Linux / Mac: `~/.gitconfig`.
  * Windows: `%HOMEDRIVE%%HOMEPATH%\.gitconfig`.

```ini
[diff "pandoc"]
  textconv=pandoc --to=markdown
  prompt = false
[alias]
  wdiff = diff --word-diff=color --unified=1
```

* Create or edit the `.gitattribute` in the root of your git project:

```ini
*.docx diff=pandoc
```

* Run diff command:

```shell
git wdiff [your_file.docx]
```

## Extensions for Microsoft Visual Code

* [Git History](https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory)

* [Git Lens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)

* [gitignore](https://marketplace.visualstudio.com/items?itemName=codezombiech.gitignore)
