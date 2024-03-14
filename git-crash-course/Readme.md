## Git Hidden Folder

There is a hidden folder called `.git` which tells us that the project is a git repo.

If we wanted to create a git repo in a  new project we would create the folder and initialize that repo using `git init`

```sh
mkdir /workspaces/temp/new-project

cd /workspaces/temp/new-project
git init
touch Readme.md
code Readme.md
# make changes to Readme.md
git status
git add .
git commit -a -m "add readme file"
```

## Cloning

Clone a repo in 3 ways: HTTPS, SSH, Github CLI

Since we are using GitHub Codespaces we will create a temporary directory in our workspace

```sh
mkdir /workspaces/temp
cd /workspaces/temp
```

### HTTPS

```sh
git clone https://github.com/SpringerAlac/gitpractice.git
cd gitpractice/
```

### SSH

```

```

## Commits

When we want to commit our changed code, git commit will open up our changed code and wait for us to add a message.

```sh
git commit
```
Set the global editor
```sh
git config --global core.editor emacs
```


Make a commit and message without using an editor.
```sh
git commit -m "added another exclamation"
```


## Branches

## Remotes

## Stashing

## Merging

## Add

Add lets you add all changed files to Staging, from there the changes can be committed.

```sh
git add Readme.md
git add .
```

## Status

Git status shows you what files will or will not be committed.

```sh
git status
```

## Reset

Reset allows you to remove staged changes from Staging.
This is nice when you want to correct what files are to be committed.

```sh
git add .
git reset
```

## Gitconfig File

The gitconfig file is that stores your global configurations for git such as email, name, editor, and more.

Showing contents of our .gitconfig file
```sh
git config --list
```
When you first install Git on a machine, you are supposed to set up your name and email
```sh
git config --global user.name "Alac Springer"
git config --global user.email alacspringer123@gmail.com
```

## Log 

Will show recent commits to the git tree

## Push 

When we want to push a repo to our remote origin

```sh
git push
```