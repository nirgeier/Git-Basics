![](resources/logos.png)

## Git Hands-on

- If you wish to play with the code, you can simply click on the button below and it will `clone` the repository into your Google Cluod Shell and you will be able to practice.
- **<kbd>CTRL</kbd>** + **click** to open in new window<br/>
    [![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://console.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https://github.com/nirgeier/Git-Basics)
---

## Branches

- Git branches are effectively a**pointer to a snapshot of your changes**. 
- When you want to add a new content to git (feature bugfix), no matter how big or how small your chage is, you will create a new branch to make your changes. 
---

## The Task

- [01. Use `git status` to see which branch you are on and which files are modified](#01-use-git-status-to-see-which-branch-you-are-on-and-which-files-are-modified)
- [02. Create a new branch named `branch1`](#02-create-a-new-branch-named-branch1)
- [03. Create new file named `file1.txt`](#03-create-new-file-named-file1txt)
- [04. Add the file to the staging area](#04-add-the-file-to-the-staging-area)
- [05. View `git status` and explain what you see](#05-view-git-status-and-explain-what-you-see)
- [06. Commit the file to the repository](#06-commit-the-file-to-the-repository)
- [07. View the log ](#07-view-the-log)
- [08. Switch back to the `main` branch](#08-switch-back-to-the-main-branch)
- [09. View the log](#09-view-the-log)
- [10. View the status](#10-view-the-status)
- [11. Edit `file1.txt` again](#11-edit-file1txt-again)
- [12. Add the file to the staging area](#12-add-the-file-to-the-staging-area)
- [13. View the status](#13-view-the-status)
- [14. View the status and explain what you see](#14-view-the-status-and-explain-what-you-see)
---
## Solutions
### 01. Use `git status` to see which branch you are on and which files are modified
    git status
### 02. Create a new branch named `branch1`
    git checkout -b branch1
### 03. Create new file named `file1.txt`
    echo 'Text' > file1.txt
### 04. Add the file to the staging area
    git add .
### 05. View `git status` and explain what you see
    $ git status
    On branch branch1 <--------------- The current branch we are on 

    No commits yet

    Changes to be committed:
    (use "git rm --cached <file>..." to unstage)

            new file:   file1.txt
### 06. Commit the file to the repository
    git commit -m"Added file1.txt"
### 07. View the log 
    git log 
### 08. Switch back to the `main` branch
    $ git checkout main
    Switched to a new branch 'main'
### 09. View the log 
    git log
### 10. View the status
    $ git status
    On branch main
    nothing to commit, working tree clean
### 11. Edit `file1.txt` again
    echo 'Line2' >> file1.txt
### 12. Add the file to the staging area
    git add .
### 13. View the status
    
    $ git status
    On branch main
    Changes to be committed:
    (use "git reset HEAD <file>..." to unstage)

            modified:   file1.txt
### 14. View the status and explain what you see
```
git status
```
<!-- navigation start -->

---

<div align="center">
<img src="../../resources/prev.png">&nbsp;
<a class="btn btn-success" href="../05-git-commit">05-git-commit</a>

</div>

---

<div align="center">
    <small>&copy;CodeWizard LTD</small>
</div>
<!-- navigation end -->