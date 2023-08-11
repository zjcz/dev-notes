# Install and configure Git
Guide on how to install and configure Git on Ubuntu.

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

## Configure Git

Set the defaults for git:

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --global init.defaultBranch main
```