![](resources/logos.png)

## Git Hands-on

- If you wish to play with the code, you can simply click on the button below and it will `clone` the repository into your Google Cluod Shell and you will be able to practice.
- **<kbd>CTRL</kbd>** + **click** to open in new window<br/>
    [![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://console.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https://github.com/nirgeier/Git-Basics)
---

## Clone

> `git clone` is a Git command which grab an existing repository and create a `clone` (copy) of the original repository.

- The `clone` synatx is the following:
```sh
git clone <url> <destination>
```

- If no `<destination>` is given a new folder with the repository name will be created

---

### Tasks
- [01. Clone the following repository: https://github.com/nirgeier/Git-Basics.git](#clone)
- [02. Verify that the repository was cloned](#verify-that-the-repository-was-cloned)
- [03. View the branches of the given repository](#view-the-branches-of-the-given-repository)

---

## Solutions

### Clone

```sh
git clone https://github.com/nirgeier/Git-Basics.git

# Output
$ git clone https://github.com/nirgeier/Git-Basics.git
Cloning into 'Git-Basics'...
remote: Enumerating objects: 12, done.
remote: Counting objects: 100% (12/12), done.
remote: Compressing objects: 100% (10/10), done.
remote: Total 12 (delta 0), reused 12 (delta 0), pack-reused 0
Unpacking objects: 100% (12/12), done.
```

### Verify that the repository was cloned
```sh
# Navigate to the cloned folder
cd Git-Basics

# View the folder content
# Unix based OS
ls -la 

# Windows
dir
```

### View the branches of the given repository
```sh
# View the branches of the given repository
git branch -a
```
<!-- navigation start -->

---

<div align="center">
<img src="../../resources/prev.png">&nbsp;
<a class="btn btn-success" href="../02-git-Init">02-git-Init</a>
&nbsp;&nbsp;||&nbsp;&nbsp;
<a href="../04-git-status">04-git-status</a>
&nbsp;<img src="../../resources/next.png">
</div>

---

<div align="center">
    <small>&copy;CodeWizard LTD</small>
</div>
<!-- navigation end -->