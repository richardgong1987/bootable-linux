# bootable-centos

## AlmaLinux bootable USB installer on Mac OSX

Before burning(Important)

format the USB disk to EXFAT, first

```sh
diskutil list

diskutil unmountDisk /dev/disk4


sudo dd if=./AlmaLinux-10.0-x86_64-dvd.iso of=/dev/disk4 status=progress conv=fsync bs=4M

```

https://wiki.almalinux.org/documentation/installation-guide.html#create-usb-installation-media

