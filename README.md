<h1 align="center">Git/GitHub_cheat_sheet</h1>

<p align="center">
  <a href="#about">About</a> &#xa0; | &#xa0; 
  <a href="#basics">Basics</a> &#xa0; | &#xa0;
  <a href="#undo-things">Undo things</a> &#xa0; | &#xa0;
  <a href="#branches">Branches</a> &#xa0; | &#xa0;
</p>

<br>

## About

**`Git`** is a distributed version control system that allows developers to track changes to their codebase, manage different versions, and collaborate with others efficiently. It enables users to work offline, create branches for experimentation, and merge changes seamlessly.

**`GitHub`** is a web-based platform built on top of git, providing additional features such as hosting git repositories, facilitating collaboration among developers, managing issues and pull requests, and enabling project management through features like wikis and project boards. It serves as a central hub for developers to store, share, and collaborate on code.

## Basics

- Install git from [here](https://git-scm.com/downloads).
- Create a GitHub account [here](https://github.com/).
- Configure git: set up your name and email using the following commands:

```shell
git config --global user.name my_name
git config --global user.email my.email@example.com
```

- Create a repository:

```shell
git init
```

- Add files to the repository (staging area):

```shell
# add all files in the current directory and its subdirectories
git add .
# add only the files in the current directory and not its subdirectories
git add *
# add specific files
git add filename
```

- Commit your changes (save changes to the repository):

```shell
git commit -m "Commit message"
```

- Push changes to GitHub:

```shell
# push to the current branch
git push
```

## Undo things

- Discard changes in a file (restore it to the state of the last commit):

```shell
# new and preferred way
git restore filename
# older way
git checkout -- filename
```

- Revert a given commit (create a new commit that undoes changes introduced by the specified commit):

```shell
git revert commit_hash
```

- ⚠️ Reset the current branch to a specific commit (delete commits):

```shell
# undo commits, keep changes in your working directory
git reset commit_hash
# undo commits, keep changes staged
git reset --soft commit_hash
# undo commits, discard all changes
git reset --hard commit_hash
# undo last commit, keep changes in your working directory
git reset HEAD~1
```

## Branches

- Create a new branch:

```shell
git branch branchname
```

- Create and switch to a new branch in one step:

```shell
git checkout -b branch_name

```

- Switch to a different branch:

```shell
git checkout branchname
```

- Merge a branch into the current branch:

```shell
# if you are on the main branch, this will merge branchname into main
git merge branchname
```

- List all branches:

```shell
git branch
```

- Delete a branch:

```shell
# delete a branch only if it has already been fully merged into the current branch
git branch -d branchname
# delete a branch forcefully, even if it contains unmerged changes
git branch -D branchname
```

<br>

<div align="center">
  Made by <a href="https://github.com/Szabold1" target="_blank">Boldizsar Szabo</a>
</div>
