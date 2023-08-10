# Customise Grub
The following is a list of customisations that can be made to the Grub bootloader.

## Remember the last choice
To remember the last choice made in the Grub menu, edit the following file:

```bash
sudo nano /etc/default/grub
```

Add the following lines to the file:

```bash
GRUB_DEFAULT=saved
GRUB_SAVEDEFAULT=true
```

Save the file and update grub:

```bash 
sudo update-grub
```

## References
- [ask ubuntu: How to get grub2 to remember last choice?](https://askubuntu.com/questions/148662/how-to-get-grub2-to-remember-last-choice)
- [Grub2/Setup - Community Help Wiki](https://help.ubuntu.com/community/Grub2/Setup)