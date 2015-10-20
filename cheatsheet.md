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
$ git push -u origin master (love)
```

#### Help someone else with their code

First, find the code on github that you want to contribute to. 

Then Fork it

```shell
$ git clone git@github.com:AmericaGL/__How_to_Repo.git 

```
Then, make some changes you think are important.

```shell

$ git add <your files>
$ git commit -"A really through explanation of what we did since this is someone else"
$ git push origin master
```

Finish what you started working on, then push up any additional commits

File a pull request with the commits in it that you want to share. make sure you have a good explanation in the pull request of what this is, what it's intend to do, and some nice language, rather than making fun of the original author.

### Typical Collaboration Patterns

How to work on the two different things at the same time. Branching is for when you want to work on somehthing that migh span over multiple commits, that's significant enough to warrant some kind of really specific deliniation.


>>>> branching_explanation

A typical collaboration pattern is actually to fork, then branch off of master, then push to your fork, then file a pull request. 

The reason for this is that master, as a branch, should always represent code or whatever that "works" and is suitable for deployment or sharing or whatever "going"

Branching is for when you want to work on something that might span over multiple commits, 