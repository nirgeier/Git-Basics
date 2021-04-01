![](resources/logos.png)

## Git Hands-on

- If you wish to play with the code, you can simply click on the button below and it will `clone` the repository into your Google Cluod Shell and you will be able to practice.
- **<kbd>CTRL</kbd>** + **click** to open in new window<br/>
    [![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://console.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https://github.com/nirgeier/Git-Basics)
---

## Status

> `git status` is a Git command which displays the state of the **working directory** and the **staging area**. 
- It display which changes have been made locally.
- Which files were staged, which haven’t, and which files aren’t being tracked by Git yet
- Git starts to track files when they are **added to the staging area**, until then the files are mraked untracked.

- The `status` synatx is the following:
```sh
git stauts <options>
```

### Tasks
- [01. View current status](#01-view-current-status)
- [02. Create new file](#02-create-new-file)
- [03. Check the current status](#03-check-the-current-status)
- [04. Add the file to the statging area](#04-add-the-file-to-the-statging-area)
- [05. Edit the new file and add new content](#05-edit-the-new-file-and-add-new-content)
- [06. Check the new status](#06-check-the-new-status)
- [07. View the changes between the statging and the working directory](#07-view-the-changes-between-the-statging-and-the-working-directory)

---

## Solutions

### 01. View current status
```sh
git status

# Output
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
```

### 02. Create new file
- Lets create a new file and see the status

```sh
# Create new file
#  - You can create new file from CLI or from the File Explore in windows, its the same

# Create new file 
touch newFile.txt

# View folder content
# Windows 
dir

# Unix based 
ls -la
```
### 03. Check the current status
- Lets the check the current status
```sh
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        newFile.txt

nothing added to commit but untracked files present (use "git add" to track)
```
- Now we will see a new entry `Untracked files` displaying the new added file `newFile.txt`

### 04. Add the file to the statging area
```sh
# Add the file to the statging area
$ git add newFile.txt 

# View the changes
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   newFile.txt
```
- Now we will see a new entry `Changes to be committed` displaying the new staged file `newFile.txt`

### 05. Edit the new file and add new content
- Lets edit the new file and add content to it
```sh
# Add content to ann existing file
# You can use echo or any text editor to edit the file
echo 'line' > newFile.txt
```
### 06. Check the new status
```sh
# View the current status of the project
git status
# View the changes
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   newFile.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   newFile.txt
```
- Now we will see a the file both as staged and modified

### 07. View the changes between the statging and the working directory
```sh
git diff
```
- For detailed diff options [read this](https://stackoverflow.com/questions/35978550/how-to-show-uncommitted-changes-in-git-and-some-git-diffs-in-detail/35978722#35978722)  
https://stackoverflow.com/questions/35978550/how-to-show-uncommitted-changes-in-git-and-some-git-diffs-in-detail/35978722#35978722


<!-- navigation start -->

---

<div align="center">
<img src="../../resources/prev.png">&nbsp;
<a class="btn btn-success" href="../03-git-clone">03-git-clone</a>
&nbsp;&nbsp;||&nbsp;&nbsp;
<a href="../05-git-commit">05-git-commit</a>
&nbsp;<img src="../../resources/next.png">
</div>

---

<div align="center">
    <small>&copy;CodeWizard LTD</small>
</div>
<!-- navigation end -->