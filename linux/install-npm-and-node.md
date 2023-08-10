# Install NPM and Node
Guide for installing npm and node on a fresh linux install.

This is based on Ubuntu 22.04.

## 1) From Ubuntu Repository (Easy but not the latest)
Install the version from the Ubuntu repositories:

**Warning: This is not the latest version of node and could be outdated**

```bash
sudo apt update
sudo apt install nodejs
```

Check the version

```bash
node -v
```

To uninstall:

```bash
sudo apt remove nodejs
```

To install npm:

```bash
sudo apt install npm
```

## 2) Using Node Version Manager (nvm) (Latest)

Download and run the install script:

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.4/install.sh | bash
source ~/.bashrc
```

Note: nvm will also install the correct version of npm to work with the selected version of node you install.

### To install the latest LTS version

Install the latest LTS version of node:

```bash
nvm install --lts
```

### To install the latest version

Install the latest version of node:

```bash
nvm install node
```

### To select a specific version

View the list of available versions to install:

```bash
nvm list-remote
```

Then select the required version
    
```bash
nvm install 18.17.1
```

### To use a specific version

It is possible to install multiple versions of node and swap between them.  

To list the installed versions:

```bash
nvm ls
```

To use a specific version:

```bash
nvm use 18.17.1
```

To uninstall a specific version:

```bash 
nvm uninstall 18.17.1
```

## References
- [How to Install Latest Git Version on Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-22-04)
- [NVM Github Page](https://github.com/nvm-sh/nvm)
