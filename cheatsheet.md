# Git Cheatsheet

### Start a new project

```shell
$ mkdir project-name
$ git init
$ touch readme.md
$ git add readme.md
$ git commit -m "initial commit"
```

## Do some work and then save it

First, do some work!

```shell
$ git status
$ git add <whatever file>
$ git status
$ git commit -m" I made a bunch of changes, so this little note to self is here to help me keep track of them"
```


### Share my work with the world!

First, create a GitHub repo.

```shell
$ git remote add origin git@github.com:<github username>/<name of repository>.git
$ git push -u origin master
```

### Help someone else with their code

First, find the code on github that you want to contribute to.

Then Fork it!

```shell
$ git clone git@github.com:<your username>/<repo_name>.git
```
Then, make some changes you think are important.

```shell
$ git add <your files>
$ git commit -m"A really through explanation of what we did since this is someone else's work."
$ git push origin master
```
Finish what you started working on, then push up any additional commits.




