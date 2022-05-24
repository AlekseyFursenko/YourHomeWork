# This is my Git Tutorial

![This is an image from git repository](git.jpeg)

![This is an image from URL](https://myoctocat.com/assets/images/base-octocat.svg)

## Git init

* `git init` - turns any directory into a Git repository.

### Common usages and options for 'git init'

* *git init* - Transform the current directory into a Git repository

* *git init  <directory>* - Transform a directory in the current path into a Git repository

* *git init --bare* - Create a new bare repository (a repository to be used as a remote repository only, that won't contain active development)

You can see all of the options with git init in **[git-scm's documentation](https://git-scm.com/docs/git-init)**

## Git add

* `git add` [filename] - command adds new or changed files in your working directory to the Git staging area.

*git add* is an important command - without it, no *git commit* would ever do anything. Sometimes, *git add* can have a reputation for being an unnecessary step in development. But in reality, *git add* is an important and powerful tool. *git add* allows you to shape history without changing how you work.

### Common usages and options for git add

* *git add <path>* - Stage a specific directory or file

* *git add .* - Stage all files (that are not listed in the .gitignore) in the entire repository

* *git add -p* - Interactively stage hunks of changes

*git add* and *git commit* go together hand in hand. They don't work when they aren't used together. And, they both work best when used thinking of their joint functionality.

You can see all of the many options with *git add* in **[git-scm's documentation](https://git-scm.com/docs/git-add)**

