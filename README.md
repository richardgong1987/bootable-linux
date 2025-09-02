# bootable-centos

## AlmaLinux bootable USB installer on Mac OSX

Before burning(Important)

format the USB disk to EXFAT, first

| File System | Best For                      | Max File Size | Cross-Platform Support         |
| ----------- | ----------------------------- | ------------- | ------------------------------ |
| FAT32       | Maximum compatibility         | 4 GB          | Almost all devices             |
| exFAT       | Large files on flash drives   | 16 EB         | Windows/macOS/Linux (new)      |
| NTFS        | Windows internal drives       | 16 TB+        | Windows only (macOS read-only) |
| HFS+        | Old Macs                      | 8 EB          | macOS only                     |
| APFS        | Modern Macs/iPhones           | 8 EB          | macOS/iOS only                 |
| ext4        | Linux servers/desktops        | 16 TB         | Linux only                     |
| Btrfs       | Linux advanced storage        | 16 EB         | Linux only                     |
| XFS         | Enterprise Linux, large files | 8 EB          | Linux only                     |



```sh
diskutil list

diskutil unmountDisk /dev/disk4


sudo dd if=./AlmaLinux-10.0-x86_64-dvd.iso of=/dev/disk4 status=progress conv=fsync bs=4M

```

https://wiki.almalinux.org/documentation/installation-guide.html#create-usb-installation-media


