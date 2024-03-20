# How to update snap-store on linux
Guide for updating snap-store on linux.

This is based on Ubuntu 22.04.

## Update snap-store

The problem is the Ubuntu Software Updater cannot update the snap-store because the snap-store process is running

First, close the snap-store process by running the following command:

```bash
kill <process id>
```

The process id is usually mentioned in the error message.  If not, find the process id by running the following command:


```bash
$ ps aux | grep snap-store
```

Then, update the snap-store by running the following command:

```bash
$ sudo snap refresh snap-store
```

## References
[Ubuntu - How to update snap-store linux.. How to update this? - superuser.com](https://superuser.com/questions/1723668/how-to-update-snap-store-linux-how-to-update-this)