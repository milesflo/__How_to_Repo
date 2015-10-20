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

File a pull request with the commits in it that you want to share. Make sure you have a good explaination in the pull request of what this is, what it's intended to do, and some nice language, rather than making fun of the original author.

### Setting up Aliases

Aliases are used to cut down on keystrokes by shortening long commands to simple 2-3 letter phrases. These are created by altering Git's global config file, like this:

```shell
$ git config --global alias.<shortened phrase> <full command>
```