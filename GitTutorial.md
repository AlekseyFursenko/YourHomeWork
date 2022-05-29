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

To see all of the possible options you have with *git commit*, check out **[Git's documentation](https://git-scm.com/docs/git-commit)**.

## Git status

* `Git status` - shows the current state of your Git working directory and staging area.

A useful feature of *git status* is that it will provide helpful information depending on your current situation. In general, you can count on it to tell you:

* Where HEAD is pointing, whether that is a branch or a commit (this is where you are "checked out" to)
* If you have any changed files in your current directory that have not yet been committed
* If changed files are staged or not
* If your current local branch is linked to a remote branch, then git status will tell you if your local branch is behind or ahead by any commits

During merge conflicts, git status will also tell you exactly which files are the source of the conflict.

### Common usages and options for `git status`

*git status* - Most often used in its default form, this shows a good base of information

*git status -s* - Give output in short format

*git status -v* - Shows more "verbose" detail including the textual changes of any uncommitted files

You can see all of the options with *git status* in **[git-scm's documentation](https://git-scm.com/docs/git-status)**.

## Git diff

* `git diff` - Show changes between commits, commit and working tree, etc

Show changes between the working tree and the index or a tree, changes between the index and a tree, changes between two trees, changes resulting from a merge, changes between two blob objects, or changes between two files on disk.

You can see all of the options with *git diff* in **[git-scm's documentation](https://git-scm.com/docs/git-diff)**.

## Git checkout

* `git checkout` - Switch branches or restore working tree files

Updates files in the working tree to match the version in the index or the specified tree. If no pathspec was given, *git checkout* will also update HEAD to set the specified branch as the current branch.

### Common usages and options for `git checkout`

*git checkout [branch]* - 
To prepare for working on *branch*, switch to it by updating the index and the files in the working tree, and by pointing HEAD at the branch. Local modifications to the files in the working tree are kept, so that they can be committed to the *branch*.

HEAD normally refers to a named branch (e.g. `master`). Meanwhile, each branch refers to a specific commit.

You can see all of the options with *git checkout* in **[git-scm's documentation](https://git-scm.com/docs/git-checkout)**

## Git log

* `git log` - Show commit logs

List commits that are reachable by following the parent links from the given commit(s), but exclude commits that are reachable from the one(s) given with a ^ in front of them. The output is given in reverse chronological order by default.

You can see all of the options with *git log* in **[git-scm's documentation](https://git-scm.com/docs/git-log)**

## Git branch

`git-branch` - List, create, or delete branches

### Common usages and options for `git branch`

If `--list` is given, or if there are no non-option arguments, existing branches are listed; the current branch will be highlighted in green and marked with an asterisk. Option `-r` causes the remote-tracking branches to be listed, and option `-a` shows both local and remote branches.

The command’s second form creates a new branch head named `branchname` which points to the current HEAD, or `start-point` if given. As a special case, for `start-point`, you may use `"A...B"` as a shortcut for the merge base of A and B if there is exactly one merge base. You can leave out at most one of A and B, in which case it defaults to `HEAD`.

Note that this will create the new branch, but it will not switch the working tree to it; use `git switch newbranch` to switch to the new branch.

With a -m or -M option, `oldbranch` will be renamed to `newbranch`.

With a -d or -D option, `branchname` will be deleted. You may specify more than one branch for deletion.

You can see all of the options with *git log* in **[git-scm's documentation](https://git-scm.com/docs/git-branch)**

