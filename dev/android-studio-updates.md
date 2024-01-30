# Android Studio Updates
Sometimes while updating Android Studio the following error can occur and the update is cancelled:

```
Some conflicts were found in the installation area:
jbr/bin/java Access denied
```

To fix this:

Close the project, and close any running emulators

Close the welcome screen

Run the following command in the terminal:

```bash
ps -A |grep java
```

This will return a list of processes that are running with the name java. You will need to kill all of these processes. To do this, run the following command:

```bash
kill -9 <process id>
```
Now, Reopen Android Studio and from the welcome screen, click the cog, then check for updates


- [Android Studio update issue with jre/bin/java - Ask Ubuntu](https://askubuntu.com/questions/1083125/android-studio-update-issue-with-jre-bin-java)