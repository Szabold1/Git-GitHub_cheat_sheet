<h1 align="center">Git/GitHub_cheat_sheet</h1>

<p align="center">
  <a href="#about">About</a> &#xa0; | &#xa0; 
  <a href="#basics">Basics</a> &#xa0; | &#xa0;
  <a href="#undo-things">Undo things</a> &#xa0; | &#xa0;
  <a href="#usage">Usage</a> &#xa0; | &#xa0;
  <a href="#allowed-functions">Allowed functions</a> &#xa0; | &#xa0;
  <a href="https://github.com/Szabold1" target="_blank">Author</a>
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

<br>

<div align="center">
  Made by <a href="https://github.com/Szabold1" target="_blank">Boldizsar Szabo</a>
</div>
