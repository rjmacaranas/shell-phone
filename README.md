# Shell Scripting Basics

### Contents
1. [Introduction](#intro)
2. [Navigation](#nav)
3. [Script Descriptions](#scripts)

## Introduction <a name="intro"></a>
Shell scripting can make life a heck of a lot easier. From automating tasks like
uploading things to GitHub to simply navigating to a certain directory, shell
scripts have got your back. Shell scripts are essentially bite-size programs built using commands available in your shell environment.

## Navigation <a name="nav"></a>
- The [cd]() command which is used to change directories requires a different
path in the shell and so it may be easier to create navigation shortcuts by
editing your .bash_profile. For example:

```shell
alias projects='cd ~/Desktop/projects'
```

## Script Descriptions <a name="scripts"></a>

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
```shell
sshpass -p 'yourPasswordHere' ssh rmacaran@unix1.csc.calpoly.edu
```
- junit.sh: compiles all java files in working directory and runs JUnit tests on all files named TestCases.java
```shell
javac *.java
java org.junit.runner.JUnitCore TestCases
```
