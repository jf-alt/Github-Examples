## Git Hidden Folder

There is a hidden folder called `.git` which tell us that the project is a git repo

If we wanted to create a git repo in a new project we can create a folder and initailize that repo using the `git init`

## Cloning

We can clone in three ways: HTTPS, SSH, Github CLI

Since we are using Github Codespaces we'll create a temporary directory in our workspace

```sh
mkdir /workspaces/tmp
cd /workspaces/tmp
git init
touch Readme.md
code Readme.md
git add .
# make sure to save changes to readme.md
git commit -m "Updated changes"
```

### HTTPS

```sh
git clone https://github.com/jf-alt/Github-Examples.git
```

### SSH


## Commits

When we want to commit code we can write the `git commit` which will open up the commit edit message in the editor of choice

```sh
git commit
```

Set global editor
```
git config --global core.editor emacs
```

## Branches

## Remotes

## Stashing

## Merging

## Add

When we want to stage changes that will be included in the commmit 
We can use the . to add all possible files

## Reset

Reset allows you to move Staged changes to unstaged.
This is useful when you need to revert all files not to be commited

```
git add .
git reset
```

> git reset will revert a git add .

## Status

git status shows you what files will or will not be commited

```
git status
```

## Gitconfig file

The gitconfig file is what stores the global configurations for git such as email, name, editor and more

Showing the contents of the gitconfig file
```
git config --list
```

When yoou first install Git on a machine, need to set up name and email

```sh
git config --global user.name "John Doe"
git config --global user.email john@example.com
```

## Log

`git log` will show the recent git commits to the git tree

```sh
git log --oneline
```

## Push

When we want to push a repo to our remote origin

```
git push
```