# Customise Grub
The following is a list of customisations that can be made to the Grub bootloader.

## Remember the last choice
To remember the last choice made in the Grub menu, edit the following file:

```bash
sudo nano /etc/default/grub
```

Add the following lines to the file:

```
GRUB_DEFAULT=saved
GRUB_SAVEDEFAULT=true
```

Save the file and update grub:

```bash 
sudo update-grub
```

### Note
If your computer is setup to dual boot with other OSes, the os-prober should detect these when you run `update-grub`. If it is disabled, you may need to add the following entry to the `/etc/default/grub` file and re-run `update-grub`:

```
GRUB_DISABLE_OS_PROBER=false
```

## References
- [ask ubuntu: How to get grub2 to remember last choice?](https://askubuntu.com/questions/148662/how-to-get-grub2-to-remember-last-choice)
- [Grub2/Setup - Community Help Wiki](https://help.ubuntu.com/community/Grub2/Setup)
- [OS Prober is Disabled in Ubuntu 22.04, Here’s a Workaround](https://www.omgubuntu.co.uk/2021/12/grub-doesnt-detect-windows-linux-distros-fix)