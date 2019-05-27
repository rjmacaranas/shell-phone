# Shell Scripting Basics

Shell scripting can make life a heck of a lot easier. From automating tasks like
uploading things to GitHub to simply navigating to a certain directory, shell
scripts have got your back.


# Navigation
- The [cd]() command which is used to change directories requires a different
path in the shell and so it may be easier to create navigation shortcuts by
editing your .bash_profile. For example:

```shell
alias projects='cd ~/Desktop/projects'
```


## Script Descriptions

- helloWorld.sh: basic script that echos 'hello, world!'
```shell
echo hello, world!
```
- deploy.sh: automates deployment of a .git repo to github
```shell
echo commit message:
read message
git add .
git commit -m $message
git push
```
- cplogin.sh: automates ssh key login, requires a local installation of sshpass
- junit.sh: compiles all java files in working directory and runs JUnit tests

