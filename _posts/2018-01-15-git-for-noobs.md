---
title: "Git for Noobs"
layout: single
header:
  teaser: /assets/images/git.gif
author: Shariful Islam Foysal
---

Clone | add | commit | push Remote Repositories
---
- Login to Github account. 
- Go to the repository or create one. 
- Coply the link of the repository from the `Clone or download` dropdown .
- Go to the directory where the repository to be placed and open `terminal` if in linux or `git bash` if in windows ( [git bash for windows](http://gitforwindows.org/) needs to be already installed).
- Then use `git clone` command to clone the repository. 


```sh  
$ git clone url
```
This will download the entire repository from github. Enter the downloaded repository folder. Change or Edit anything necessary. Then stage folder/files for commit. 
To add specific files/folder to commit use the following command:

```sh
$ git add fileName
```
Or all the changes can be added at once with:
```sh
$ git add . // git add -a also do the work
```
Now selected file/folders are ready for commit. To commit:
```sh
$ git commit -m "Commit Message" //-m is the message flag
```
Two previous commands can be put together like this:
```sh
$ git commit -a -m "Commit Message" //staging all changes and then commit
```
Now we can push it to remote our repository:
```sh
$ git push -u Branch Name //to push it to any branch
$ git push -u origin master //to merge the changes with master branch
```

**TO Be Continued...**
