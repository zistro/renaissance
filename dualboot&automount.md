# Dual-booting and drive auto mounting
* If your're dual-booting or you want to mount your other drives do these
* First let's mount drive. For windows drives that use ntfs file system install this
  ```
  sudo pacman -S ntfs-3g
  ```
* Create a mount point in /mnt
  ```
  cd /mnt
  ```
  ```
  sudo mkdir windir
  ```
* Then get the uuid of the partition you want to mount
 ```
lsblk-f
```
* Then edit this file and add your drive uuid like below to mount at the previously created mounting point
 ```
sudo nano /etc/fstab
```
 ```
 UUID=yourUUID /mnt/windir ntfs defaults,x-gvfs-show 0 0 
 ```
* Then unmount all drives and mount again if there's no error then you're good to go
  ```
  sudo umount -a
  ```
  ```
  sudo mount -a
  ```
* Mounting other os like windows on grub
* Install os-prober
  ```
    sudo pacman -S os-prober
  ```
* Edit grub file
  ```
  sudo nano /etc/default/grub
  ```  
* Uncomment the line
  ```
  GRUB_DISABLE_OS_PROBER=false
  ```
* Update grub config
  ```
  sudo grub-mkconfig -o /boot/grub/grub.cfg
  ```
* Reboot and check if it worked
* Done

        
