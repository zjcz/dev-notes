# Troubleshhoting - Blank Screen with a Random Number in the Top Corner on Bootup

After Ubuntu crashes unexpectedly, when rebooting a blank screen with a random number in the top corner of the screen is shown.

Press `Ctrl + Alt + F2` to get to a terminal and login. Then run the following commands:

```bash
sudo apt update
sudo apt upgrade
```

Reboot the computer and it should be fixed.

```bash
shutdown -r now
```

## References
- [Reddit - Black screen at startup with a random number on the top left corner](https://www.reddit.com/r/pop_os/comments/tyz7g5/black_screen_at_startup_with_a_random_number_on/)