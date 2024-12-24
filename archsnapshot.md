# archsnaps
step by step guide for auto grub btrfs snapshots.
Let's say you have installted arch linux with btrfs file system and you want to set it up so it auto snapshots and add a snapshot list in your grub menu.

# Let's start
* Install timeshift (paru is my aur helper you can use yours)
```
paru -S timeshift
```
* Open and setup timeshift with terminal
```
sudo -E timeshift-gtk
```
* Set up timeshift with btrfs
* Install grub btrfs inotify-tools timeshift-autosnap
```
paru -S grub-btrfs inotify-tools timeshift-autosnap
```
* Set up grub btrfsd daemon to automatically update grub menu
```
sudo systemctl edit --full grub-btrfsd
```
* Make this part
```
ExecStart=/usr/bin/grub-btrfsd --syslog /.snapshots
```
* Look like this
```
ExecStart=/usr/bin/grub-btrfsd --syslog --timeshift-auto
```
* Then enable and start the daemon
```
sudo systemctl enable grub-btrfsd
```
```
sudo systemctl start grub-btrfsd
```
* For more info go to the [grub btrfs repo](https://github.com/Antynea/grub-btrfs)
