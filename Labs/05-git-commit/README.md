![](resources/logos.png)

## Git Hands-on

- If you wish to play with the code, you can simply click on the button below and it will `clone` the repository into your Google Cluod Shell and you will be able to practice.
- **<kbd>CTRL</kbd>** + **click** to open in new window<br/>
    [![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://console.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https://github.com/nirgeier/Git-Basics)
---

## Commit

- `git commit` is a Git command which **Record changes to the *local* repository**
- `git commit` create a **new commit** containing the **current contents** of the index (staging) and the desired `log` message describing the changes. 
---

## The Task

- [01. View current status](#01-view-current-status)
- [02. Create a new file](#02-create-a-new-file)
- [03. `add` the file to the staging area](#03-add-the-file-to-the-staging-area)
- [04. View `git status` and explain what you see](#04-view-git-status-and-explain-what-you-see)
- [05. `commit` the file to the repository](#05-commit-the-file-to-the-repository)
- [06. View the log ](#06-view-the-log)
- [07. Change the content of the file you created earlier](#07-change-the-content-of-the-file-you-created-earlier)
- [08. `add` the file change](#08-add-the-file-change)
- [09. Change the file again](#09-change-the-file-again)
- [10. Make a another `commit`](#10-make-a-another-commit)
- [11. Edit the file again](#11-edit-the-file-again)
- [12. Add the second file to the **prevoius commit**](#12-add-the-second-file-to-the-prevoius-commit)

---
## Solutions

### 01. View current status 
    git status

### 02. Create a new file
    echo 'Text' > file1.txt

### 03. `add` the file to the staging area
    git add .

### 04. View `git status` and explain what you see
    git status

### 05. `commit` the file to the repository
    git commit -m"Added file 1"

### 06. View the log 
    git log

### 07. Change the content of the file you created earlier
    echo 'line2' >> file1.txt

### 08. `add` the file change
    git add .

### 09. Change the file again
    echo 'line3' >> file1.txt

### 10. Make a another `commit`
    git add . && git commit -m"Another commit"

### 11. Edit the file again
    echo 'line4' >> file1.txt
### 12. Add the second file to the **prevoius commit**
```sh
# Here we have few options, this is the shortest one
git add . && git commit --amend --no-edit
```

<!-- navigation start -->

---

<div align="center">
<img src="../../resources/prev.png">&nbsp;
<a class="btn btn-success" href="../04-git-status">04-git-status</a>
&nbsp;&nbsp;||&nbsp;&nbsp;
<a href="../06-Branches">06-Branches</a>
&nbsp;<img src="../../resources/next.png">
</div>

---

<div align="center">
    <small>&copy;CodeWizard LTD</small>
</div>
<!-- navigation end -->