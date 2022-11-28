# Hey! I'm Filing Here

This program is an implementation of a 1MiB EXT2 file system.

## Building

Run `make` to build the program

## Running

Run `./ext2-create` to create cs111-base.img
Run `mkdir mnt` to make a new directory calld mnt
Run `sudo mount -o loop cs111-base.img mnt` to mount the filesystem

After `cd mnt`, we used the `ls -ain` command to see the files and directory in the filesystem, and the output is:

total 7
     2 drwxr-xr-x 3    0    0 1024 Nov 28 12:54 .
942241 drwxr-xr-x 5 1000 1000 4096 Nov 28 12:54 ..
    13 lrw-r--r-- 1 1000 1000   11 Nov 28 12:54 hello -> hello-world
    12 -rw-r--r-- 1 1000 1000   12 Nov 28 12:54 hello-world
    11 drwxr-xr-x 2    0    0 1024 Nov 28 12:54 lost+found



## Cleaning up

Explain briefly how to unmount the filesystem, remove the mount directory, and
clean up all binary files.

To unmount, run `sudo umount mnt`
To remove mnt director, run `rmdir mnt` 
To clean up binary files, run `make clean` 
