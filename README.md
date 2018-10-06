
 MOUNT COMMAND 

DESCRIPTION:
The Linux Mount command is used to mount USBs, DVDs, SD cards, and other types of storage devices on a computer running the Linux operating system. Linux uses a directory tree structure. Unless the storage device is mounted to the tree structure, the user can't open any of the files on the computer.

SYNTAX:
    mount option filesystems

OPTIONS:
1. mount -l: List all the mounted file-systems.  
2. mount -M: It causes the contents of older directory to be accessed under the new directory. The physical location of the files is not changed.
3. mount -n: Mount without writing in /etc/mtab. This is necessary for example when /etc is on a read-only filesystem.
4. mount -O: Used in conjunction with -a, to limit the set of file-systems to which the -a is applied. Like -t in this regard except that it is useless except in the context of -a.
            Example:mount -a -O no_netdev
                  mounts all file systems except those which have the option _netdev specified in the options field in the /etc/fstab file.
5. mount -o: Options are specified with a -o flag followed by a comma separated string of options. Some of these options are only useful when they appear in the /etc/fstab file.
