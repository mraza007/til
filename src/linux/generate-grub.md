# Generating a Grub File


We can use this command to generate a `grub` configuration file. 

```sh
sudo grub-mkconfig -o /boot/grub/grub.cfg
```
As `grub-mkconfig` scans hardrives for bootable operating systems such as windows, mac or linux distros