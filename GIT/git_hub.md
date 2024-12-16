## What is Github?
Github is a web-based Git repository hosting service. It is a popular platform for developers to collaborate on projects and to share code. Github provides a user-friendly interface for managing and tracking changes to your code, as well as a platform for hosting and sharing your projects with others.

Some other alternative of Github are:
- Gitlab
- Bitbucket
- Azure Repos
- Gitea
## Configure your config file
```
git config --global user.email "your-email@example.com"
git config --global user.name "Your Name"
```

Now you can check your config settings:
```
git config --list
```

## Adding code to remote repository
Now that you have setup your ssh key and added it to your github account, you can start pushing your code to the remote repository.

Create a new Repo on your system first, add some code and commit it.
```
git init
git add <files>
git commit -m "commit message"
```

### Check remote url setting
You can check the remote url setting by running the following command:
```
git remote -v
```

### Add remote repository
```
git remote add origin https://github.com/saurav/git-something.git
```

### Push code to remote repository
Here `remote-name` is the name of the remote repository that you want to push to and `branch-name` is the name of the branch that you want to push.
```
git push origin main
```

### Setup an upstream remote

Setting up an upstream remote is useful when you want to keep your local repository up to date with the remote repository. It allows you to fetch and merge changes from the remote repository into your local repository.

To set up an upstream remote, you can use the following command:

```
git remote add upstream <remote-url>
```

or you can use shorthand:

```
git remote add -u <remote-url>
```

You can do this at the time of pushing your code to the remote repository.

```
git push -u origin main
```

This will set up an upstream remote and push your code to the remote repository.

This will allow you to run future commands like `git pull` and `git push` without specifying the remote name.