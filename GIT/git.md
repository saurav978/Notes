# GIT

## Your config settings

### To configure name and email this

```
git config --global user.email "your-email@example.com"
git config --global user.name "Your Name"
```

### Now you can check your config settings:

```
git config --list
```

This will show you all the settings that you have changed.

## Creating a repository

you can use the following command:

```
git status
git init
```

## Commit

commit is a way to save your changes to your repository. It is a way to record your changes and make them permanent. You can think of a commit as a snapshot of your code at a particular point in time. When you commit your changes, you are telling git to save them in a permanent way. This way, you can always go back to that point in time and see what you changed.

Usual flow looks like this:
![image](https://docs.chaicode.com/_astro/commit.CZ_pUUof_1Y9b3g.svg)

## Complete git flow

A complete git flow, along with pushing the code to github looks like this:
![git flow](https://docs.chaicode.com/_astro/gitflow.CjDHzFoj_dc900.svg)

## Stage

```
git init
git add <file> <file2>
git status
```

> to add all files at onec

```
git add .
```

## Commit

```
git commit -m "commit message"
git status
```

## Logs

```
git Log
```

This command will show you the history of your repository. It will show you all the commits that were made to the repository

```
git log --oneline
```

show only the commit message. This will make the output more compact and easier to read.

## gitignore

Gitignore is a file that tells git which files and folders to ignore. It is a way to prevent git from tracking certain files or folders. You can create a gitignore file and add list of files and folders to ignore by using the following command:

example

```
node_modules
.env
.vscode
```
