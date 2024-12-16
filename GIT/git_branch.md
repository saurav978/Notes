# Branches in git

Branches are a way to work on different versions of a project at the same time. They allow you to create a separate line of development that can be worked on independently of the main branch. This can be useful when you want to make changes to a project without affecting the main branch or when you want to work on a new feature or bug fix.

![bracnh image](https://docs.chaicode.com/_astro/branches.yYu2erFZ_Z1NQDag.svg)

## HEAD in git

The HEAD is a pointer to the current branch that you are working on. It points to the latest commit in the current branch. When you create a new branch, it is automatically set as the HEAD of that branch.

## Creating a new branch

```
git branch
git branch bug-fix
git switch bug-fix
git log
git switch master
git switch -c dark-mode
git checkout orange-mode
```

- `git branch` - This command lists all the branches in the current repository.
-  `git branch bug-fix` - This command creates a new branch called `bug-fix`
-  `git switch bug-fix` - This command switches to the `bug-fix` branch.
- `git log` - This command shows the commit history for the current branch.
- `git switch master` - This command switches to the `master` branch.
- `git switch -c dark-mode` - This command creates a new branch called `dark-mode`. the `-c` flag is used to create a new branch.
- `git checkout orange-mode` - This command switches to the `orange-mode` branch.
## Merging branches

  ### Fast-forward merge
  When you are done working on a branch, you can merge it back into the main branch. This is done using the following command
  
   ```
git checkout main
git merge bug-fix
```

Some points to note:

- `git checkout main` - This command switches to the `main` branch.
- `git merge bug-fix` - This command merges the `bug-fix` branch into the `main` branch.