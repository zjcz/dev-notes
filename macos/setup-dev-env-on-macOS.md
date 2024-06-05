# Setting up dev environment on MacOS

## Install VS Code
- [Visual Studio Code on macOS](https://code.visualstudio.com/docs/setup/mac)

## Install Homebrew
- [Homebrew](https://brew.sh/)
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Flutter
- [Install Flutter on macOS](https://flutter.dev/docs/get-started/install/macos)

- Install xcode from the website rather than the appstore, it is much faster, but you may have to manage updates yourself: [Developer Downloads](https://developer.apple.com/download/all/?q=xcode).

- If you get an error while installing cocoapods: 'drb requires Ruber version >=2.7.0. The current ruby version is 2.6.10.210' (or similar), try using 'brew' instead'. See [Stack Overflow](https://stackoverflow.com/questions/77339560/error-installing-cocoapodsdrb-requires-ruby-version-2-7-0-the-current-ruby)

- Network errors while installing Cocoapods or Brew: need to increase git buffer size and ensure using http/1.1.  See [StackOverflow](https://stackoverflow.com/questions/70303947/error-installing-homebrew-unexpected-disconnect-while-reading-sideband-packet#:~:text=It%20might%20be%20your%20network,an%20issue%20with%20post%20buffer.)

- [Android Studio](https://developer.android.com/studio/install#mac)

## Customise ZSH
- [How I customise my Terminal with Oh My Zsh](https://dev.to/hannahgooding/how-i-customise-my-terminal-with-oh-my-zsh-macos-427i)

## Java

### Install Intellij
Download the required version from the [Intellij Website](https://www.jetbrains.com/idea/download/?section=mac).

### Install Java
Open Intellij.  If it doesn't prompt you to download Java, start a new project and open "Project Structure" (Cmd+;).  Click on the "SDKs" tab and select the Java SDK.  If you don't have one, click on the "+" and download the required version.

### Install Maven
Intellij installs it's own version of Maven but if you need to install it separately, use Homebrew:
```bash
brew install maven
```
