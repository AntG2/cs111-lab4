# Hey! I'm Filing Here

In this lab, I successfully implemented the setup for a 1MiB ext2 filesystem 
with 2 directories, 1 regular file, and 1 symbolic link.

## Building
```shell
make
```

## Running
```shell
./ext2-create
mkdir mnt
sudo mount -o loop cs111-base.img mnt
```
or mount it onto an existing directory

## Cleaning up
```shell
sudo umount mnt
# or whichever directory the image is mounted to
rmdir mnt
make clean
```
