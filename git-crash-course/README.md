## Git Hidden Folder

There is a hidden folder called `.git` wich tells you that our
project is a git repo.

I we wanted to create a git repo in a new project we create the
folder and the initialize that repo using `git init`

```
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
code Readme.md
git status
git add .
# makes changes to readme.md
git commit -a -m "add readme file"
```

## Cloning

We can clone three ways: HTTPS, SSH, Github CLI

Since we are using GitHub Codespaces we'll a create
temporary directory in our workspace

```sh
mkdir /workspace/tmp
cd /workspace/tmp
```

### HTTPS

```sh
git clone https://github.com/aprendizsw/Github-Examples.git
cd Github-Examples
```

## Commits

When we want to commit code we can write git commit will open up the commit edit message in the editor of choice.

```sh
git commit
```

Set the global editor
```
git config --global core.editor emacs
```

## Branches

## Remotes

## Stashing

## Add

When we want to stage changes that will be included in the commit
We can use the . to add all posible files

```
git add Readme.md
git add .
```

## Merging


## Reset

Reset allows you to move Staged changes to be unstaged.
This is useful when you to revert all files not to be not commited

```
git add .
git reset
```

> git reset will revert a `git add .`

## Status

Git status shows you what files will or will not be commited.

```
git status
```

## Gitconfig file

The gitconfig file is what stores your global configurations for git such as email, name, editor and more.

Showing the contents of our .gitconfig file

```
git config --list
```

When you first install Git on a machine you are suppose to set up your name and email

```sh
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

Make a commit and commit message without opening an editor
```
git commit -m "add another exlamation"
```

## Log

git log will show recent git commits to the git tree

## Push

When we want to push a repo to our remote origin

```
git push
```