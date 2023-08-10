# Fresh Dev Installation
Guide for tools and apps to install on a fresh linux install.  

This is based on Ubuntu 22.04.

## Install Git

### 1) From Ubuntu Repository (Easy but not the latest)
Install the latest version from the Ubuntu repositories:

```bash
sudo apt-get update
sudo apt-get install git
```

Check the version

```bash
git --version
```

### 2) Using PPA (Latest)

Add the PPA for the latest version of git:

```bash
sudo add-apt-repository ppa:git-core/ppa
sudo apt-get update
sudo apt-get install git
```

Set the defaults for git:

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --global init.defaultBranch main
```

## Install VS Code
Install from the Snap Store
    
```bash 
sudo snap install code --classic
```
## Install IntelliJ

Install from the Snap Store

```bash
sudo snap install intellij-idea-community --classic
```

## References
- [How to Install Latest Git Version on Ubuntu](https://itsfoss.com/install-git-ubuntu/)
