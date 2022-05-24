# This is my Git Tutorial

![This is an image from git repository](git.jpeg)

![This is an image from URL](https://myoctocat.com/assets/images/base-octocat.svg)

## Git init

* `git init` - turns any directory into a Git repository.

### Common usages and options for `git init`

* *git init* - Transform the current directory into a Git repository

* *git init  <directory>* - Transform a directory in the current path into a Git repository

* *git init --bare* - Create a new bare repository (a repository to be used as a remote repository only, that won't contain active development)

You can see all of the options with git init in **[git-scm's documentation](https://git-scm.com/docs/git-init)**

## Git add

* `git add` [filename] - command adds new or changed files in your working directory to the Git staging area.

*git add* is an important command - without it, no *git commit* would ever do anything. Sometimes, *git add* can have a reputation for being an unnecessary step in development. But in reality, *git add* is an important and powerful tool. *git add* allows you to shape history without changing how you work.

### Common usages and options for `git add`

* *git add <path>* - Stage a specific directory or file

* *git add .* - Stage all files (that are not listed in the .gitignore) in the entire repository

* *git add -p* - Interactively stage hunks of changes, to walk through the changes and separate them out, even if they're in the same file.

*git add* and *git commit* go together hand in hand. They don't work when they aren't used together. And, they both work best when used thinking of their joint functionality.

You can see all of the many options with *git add* in **[git-scm's documentation](https://git-scm.com/docs/git-add)**

## Git commit

* `git commit -m "update the file"` - creates a commit, which is like a snapshot of your repository. These commits are snapshots of your entire repository at specific times. You should make new commits often, based around logical units of change. Over time, commits should tell a story of the history of your repository and how it came to be the way that it currently is. Commits include lots of metadata in addition to the contents and message, like the author, timestamp, and more.

Commits have two phases to help you craft commits properly. Once you're ready to craft your commits, you'll use *git add <FILENAME>* to specify the files that you'd like to "stage" for commit. Without adding any files, the command git commit won't work. Git only looks to the staging area to find out what to commit.

### Common usages and options for `Git commit`

*git commit -m "descriptive commit message"* - This starts the commit process, and allows you to include the commit message at the same time.

*git commit -am "descriptive commit message"* - In addition to including the commit message, this option allows you to skip the staging phase. The addition of `-a` will automatically stage any files that are already being tracked by Git (changes to files that you've committed before).

*git commit --amend* - Replaces the most recent commit with a new commit.