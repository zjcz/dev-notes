# Fresh Dev Installation
Guide for tools and apps to install on a fresh linux install.  

This is based on Ubuntu 22.04.

## Install Git

See [Install and configure Git](../dev/install-and-configure-git.md)

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

## Install Docker
See [Install Docker](https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository) to install the docker engine, and [Install Docker Desktop on Ubuntu](https://docs.docker.com/desktop/install/ubuntu/) to install the desktop app


## Install Java
Java can be installed using the following command:

```bash
sudo apt install default-jdk
```

However, to install a specific version from a different vendor, first download the .tar.gz file from the vendor's website.  Then, extract the file.  For example (assuming the file is in the home directory):

```bash
$ tar xvzf OpenJDK11U-jdk_x64_linux_hotspot_11.0.12_7.tar.gz
```

To confirm the version, run the following command:

```bash 
$ ./jdk-11.0.12+7/bin/java -version
```

To ensure that the correct version is used, add the following to the .bashrc file:

```bash
export JAVA_HOME=/home/username/jdk-11.0.12+7
export PATH=$JAVA_HOME/bin:$PATH
```
Helful commands:
To find where the current version of Java is installed:
```bash
$ which java
```

When multiple versions of Java is installed, use the following command to select the default version:
```bash 
$ sudo update-alternatives --config java
```

## References
- [How to Install Latest Git Version on Ubuntu](https://itsfoss.com/install-git-ubuntu/)
- [Install Java manually on Linux](https://opensource.com/article/21/9/install-java-manually-linux)