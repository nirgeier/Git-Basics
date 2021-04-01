![](resources/logos.png)

## Git Hands-on

- If you wish to play with the code, you can simply click on the button below and it will `clone` the repository into your Google Cluod Shell and you will be able to practice.
- **<kbd>CTRL</kbd>** + **click** to open in new window<br/>
    [![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://console.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https://github.com/nirgeier/Git-Basics)
---

## `git init`

> `git init` is a Git command which create a new local git repository

- The `init` synatx is the following:
```sh
# if no [directory] is supplied, the repository will be created in the current directory
git init [directory]

####
$ git init folderA
Initialized empty Git repository in .../folderA/.git/
```

---
## Tasks

[01. Create new repository in a directoryd folderA](#01-create-new-repository-in-a-folder-named-foldera)  
[02. What is the current branch name?](#02-what-is-the-current-branch-name)

---
## Solutions

#### 01. Create new repository in a directoryd folderA
```sh
# init new repository
git init folderA
```

#### 02. What is the current branch name?
```sh
# Print the list of all the local and remote branches
# Since its a new respository there should be only 1 default branch
git branch -a
```


<!-- navigation start -->

---

<div align="center">
<img src="../../resources/prev.png">&nbsp;
<a class="btn btn-success" href="../01-Configuration">01-Configuration</a>
&nbsp;&nbsp;||&nbsp;&nbsp;
<a href="../03-git-clone">03-git-clone</a>
&nbsp;<img src="../../resources/next.png">
</div>

---

<div align="center">
    <small>&copy;CodeWizard LTD</small>
</div>
<!-- navigation end -->