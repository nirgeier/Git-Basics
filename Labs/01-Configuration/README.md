![](resources/logos.png)

## Git Hands-on

- If you wish to play with the code, you can simply click on the button below and it will `clone` the repository into your Google Cluod Shell and you will be able to practice.
- **<kbd>CTRL</kbd>** + **click** to open in new window<br/>
    [![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://console.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https://github.com/nirgeier/Git-Basics)
---

## Configuraiton
- In order to be able to commit content to git we ned to set up the following configuraiton

## TOC
- [Configure Identity](#configure-identity)
- [Configure Editor](#configure-editor)
- [Configure-default-branch-name](#Configure-default-branch-name)
- [Fix command typos](#fix-command-typos)
- [Configure reabse as the default option](#configure-reabse-as-the-default-option)

## Git Initial Configuration
- In order to be able to commit you need to set up your identity.

### Configure Identity
- **Set your global username/email configuration:**
    ```sh
    # Configure UserName
    git config --global user.name "Nir Geier"
    # Configure Email
    git config --global user.email "nirgeier@example.com"
    ```

## More Configuration
- We can choose which editor to use.
- If you are using windows the installer let you choose this configuraiton via the installer


### Configure Editor
```sh
# Nano:
git config --global core.editor nano

# Vim
git config --global core.editor vi

# windows - Notepad++
git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst -notabbar -nosession -noPlugin"

```

### Configure default branch name
    git config --global init.defaultBranch main
    
    
### Fix command typos
    git config --global help.autocorrect 1
    
### Configure reabse as the default option
    git config --global pull.rebase true
    


<!-- navigation start -->

---

<div align="center">

<a href="../02-git-Init">02-git-Init</a>
&nbsp;<img src="../../resources/next.png">
</div>

---

<div align="center">
    <small>&copy;CodeWizard LTD</small>
</div>
<!-- navigation end -->