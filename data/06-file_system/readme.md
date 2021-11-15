

## Introduction


If you're a regular windows user you may have seen some folder like C:, D:. But in linux the hierarchy is different and it's more likely to an UNIX system. 
As in windows C: / D: / E: these are the root folder but in linux the root folder are bin, root, use, hoome, temp, var etc.



The Linux file system contains the following sections:

   - The root directory (/)
   - A specific data [storage format](https://biztechmagazine.com/article/2021/08/file-storage-types-ntfs-vs-fat32-perfcon) (EXT3, EXT4, BTRFS, XFS and so on)
   - A partition or logical volume having a particular file system.


[Learn more about Linux File System Strucure](https://www.javatpoint.com/linux-file-system)



## File System Hierarchy

The Filesystem Hierarchy Standard defines the directory structure and directory contents in Linux distributions. It is maintained by the Linux Foundation. The latest version is 3.0, released on 3 June 2015.

<img src="https://user-images.githubusercontent.com/72222987/141767915-bd4a3269-e360-48c3-9793-973911f5bb2b.png" width="70%">

- here some important directories are discussed:

  - <b>/bin</b>: (Binaries) contains executables that are essential t the entire operating system.
  - <b>/sbin</b>: (System Binaries) Contains Executables that are essential and should be executable by [root user]()
  - <b>/lib</b>: (Library) Many binaries from /Bin & /Sbin are shared to this diractory to store.
  - <b>/usr</b>: (User Directory) Binaries which are not OS and intended for end user are contain here.
     - <b>bin</b>: all those kind of binaries contains here
     - <b>local</b> 
       - <b>bin</b>: contains those binaries which are compiles by user manually. All these binaries are seperated to aboid conflict with softwares installed by system package manager
  - <b>/etc </b>: (Etcetra) contains editable text configuration. Many files with `.conf` which are text based flie are present here user can modify them as per requirement.
  - <b>/home</b>: User's personal space. In a multiuser OS here contains multiple user's directory registered on system.
  - <b>/boot</b>: contains files which are needed to boot the system. e.g.: system's bootloader, kernel are present here.
  - <b>/dev</b>: (device File) contains all those devices (both block type and character type devices) connected to that computer. Here we interact/mount any device.
  - <b>/opt</b>: (Optional) contains optional or add-on softwares with which we rarely interact.
  - <b>/var</b>: (Variables) Contains variable files that will change as the use of OS. Example- logs, caches.
     - <b>temp</b>: The /var/tmp directory is made available for programs that require temporary files or directories that are preserved between system reboots. Therefore, data stored in /var/tmp is more persistent than data in /tmp
  - <b>/temp</b>: (Temporary Files) The /tmp directory must be made available for programs that require temporary files.
  - <b>/proc</b>: (Process) This is an illusionary file system that doesn't actually existson the disk but is created in the memory by kernel to keep track of all runnung processes.


<br>
<br>


------------------------------------------------------



### Here is an image to understand relevant folder for a file in linux

![image](https://user-images.githubusercontent.com/72222987/141137987-6caed901-eb65-4d09-a4a5-f6f4c9a09084.png)

[source](http://blog.danyll.com/linux-directory-map/)








[get a video lecture of 2 minutes](https://www.youtube.com/watch?v=42iQKuQodW4&t=76s)
