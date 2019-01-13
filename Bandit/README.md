## Bandit :: Cracked

> The Bandit wargame is aimed at absolute beginners. It will teach the basics needed to be able to play other wargames. If you notice something essential is missing or have ideas for new levels, please let us know!

### Bandit Level 0

#### Level Goal
http://overthewire.org/wargames/bandit/bandit0.html


The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0. Once logged in, go to the Level 1 page to find out how to beat Level 1.

#### Solution :

###### Tool : PuTTY

```
login as: bandit0
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames


bandit0@bandit.labs.overthewire.org's password: bandit0
Linux bandit 4.18.12 x86_64 GNU/Linux

      ,----..            ,----,          .---.
     /   /   \         ,/   .`|         /. ./|
    /   .     :      ,`   .'  :     .--'.  ' ;
   .   /   ;.  \   ;    ;     /    /__./ \ : |
  .   ;   /  ` ; .'___,/    ,' .--'.  '   \' .
  ;   |  ; \ ; | |    :     | /___/ \ |    ' '
  |   :  | ; | ' ;    |.';  ; ;   \  \;      :
  .   |  ' ' ' : `----'  |  |  \   ;  `      |
  '   ;  \; /  |     '   :  ;   .   \    .\  ;
   \   \  ',  /      |   |  '    \   \   ' \ |
    ;   :    /       '   :  |     :   '  |--"
     \   \ .'        ;   |.'       \   \ ;
  www. `---` ver     '---' he       '---" ire.org


Welcome to OverTheWire!

...

  Enjoy your stay!

bandit0@bandit:~$

```

### Bandit Level 0 → Level 1

#### Level Goal
http://overthewire.org/wargames/bandit/bandit1.html

The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

#### Solution :

```
bandit0@bandit:~$ ls
readme
bandit0@bandit:~$ cat readme
boJ9jbbUNNfktd78OOpsqOltutMc3MY1
bandit0@bandit:~$
```

##### Username : bandit1
##### Password : boJ9jbbUNNfktd78OOpsqOltutMc3MY1

### Bandit Level 1 → Level 2

#### Level Goal

The password for the next level is stored in a file called - located in the home directory

#### Solution :

```
bandit1@bandit:~$ cat ./-
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
```
##### Username : bandit2
##### Password : CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9


Bandit Level 2 → Level 3

Level Goal

The password for the next level is stored in a file called spaces in this filename located in the home directory

Solution :

```
bandit2@bandit:~$ cat "spaces in this filename"
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
```

Username : bandit3
Password : UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

Bandit Level 3 → Level 4
Level Goal
The password for the next level is stored in a hidden file in the inhere directory.

Solution :

```
bandit3@bandit:~$ ls
inhere
bandit3@bandit:~$ cd inhere/
bandit3@bandit:~/inhere$ ls -la
total 12
drwxr-xr-x 2 root    root    4096 Oct 16 14:00 .
drwxr-xr-x 3 root    root    4096 Oct 16 14:00 ..
-rw-r----- 1 bandit4 bandit3   33 Oct 16 14:00 .hidden
bandit3@bandit:~/inhere$ cat .hidden
pIwrPrtPN36QITSp3EQaw936yaFoFgAB
bandit3@bandit:~/inhere$
```
Username : bandit4
Password : pIwrPrtPN36QITSp3EQaw936yaFoFgAB

Bandit Level 4 → Level 5

Level Goal

The password for the next level is stored in the only human-readable file in the inhere directory. Tip: if your terminal is messed up, try the “reset” command.

Solution : 

```
bandit4@bandit:~$ ls
inhere
bandit4@bandit:~$ cd inhere/
bandit4@bandit:~/inhere$ ls
-file00  -file01  -file02  -file03  -file04  -file05  -file06  -file07  -file08  -file09
bandit4@bandit:~/inhere$ find . -type f -exec cat {} +
N▒{▒▒Y▒d4▒▒▒]3▒▒▒▒▒9(▒
Q▒▒▒▒▒@▒%@▒▒▒ZP*E▒▒1▒V▒▒▒̫*▒▒▒ۻ▒▒U"7▒w▒▒▒H▒▒ê▒Q▒▒(▒▒▒#▒▒▒▒T▒v▒▒(▒ִ▒▒▒▒▒A*▒
2J▒Ş؇_▒y7+▒▒pm▒▒▒;▒▒:D▒▒^▒▒@▒gl▒Q▒▒.A▒▒u▒▒#▒▒▒w$N?c▒-▒▒Db3▒▒=▒▒FPn▒
                                                                   '▒U▒▒▒M▒▒/u
XS
▒mu▒z▒▒▒хkoReBOKuIDDepwhWk7jZC0RTdopnAYKh
▒=<▒W▒▒▒▒▒ht▒Z▒▒!▒▒{▒U
▒▒▒▒▒▒~%        C[▒걱>▒▒| ▒

bandit4@bandit:~/inhere$
```

Creds : bandit5::koReBOKuIDDepwhWk7jZC0RTdopnAYKh


Bandit Level 5 → Level 6
Level Goal
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

- human-readable
- 1033 bytes in size
- not executable


Solution :

```
bandit5@bandit:~$ cd inhere/
bandit5@bandit:~/inhere$ ls
maybehere00  maybehere02  maybehere04  maybehere06  maybehere08  maybehere10  maybehere12  maybehere14  maybehere16  maybehere18
maybehere01  maybehere03  maybehere05  maybehere07  maybehere09  maybehere11  maybehere13  maybehere15  maybehere17  maybehere19
bandit5@bandit:~/inhere$ cd maybehere00
bandit5@bandit:~/inhere/maybehere00$ ls
-file1  -file2  -file3  spaces file1  spaces file2  spaces file3
bandit5@bandit:~/inhere/maybehere00$ cd ..
bandit5@bandit:~/inhere$ find ./ -type f -size 1033c
./maybehere07/.file2
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
DXjZPULLxYr17uwoI01bNLQbtFemEgo7
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        bandit5@bandit:~/inhere$

```

bandit6::DXjZPULLxYr17uwoI01bNLQbtFemEgo7


Bandit Level 6 → Level 7

Level Goal

The password for the next level is stored somewhere on the server and has all of the following properties:

- owned by user bandit7
- owned by group bandit6
- 33 bytes in size


#### Something strange happened. God access ?

```
bandit6@bandit:~$ ls -la
total 20
drwxr-xr-x  2 root root 4096 Oct 16 14:00 .
drwxr-xr-x 41 root root 4096 Oct 16 14:00 ..
-rw-r--r--  1 root root  220 May 15  2017 .bash_logout
-rw-r--r--  1 root root 3526 May 15  2017 .bashrc
-rw-r--r--  1 root root  675 May 15  2017 .profile
bandit6@bandit:~$ cd ..
bandit6@bandit:/home$ ls
bandit0   bandit14  bandit2   bandit25      bandit29      bandit31-git  bandit7
bandit1   bandit15  bandit20  bandit26      bandit29-git  bandit32      bandit8
bandit10  bandit16  bandit21  bandit27      bandit3       bandit33      bandit9
bandit11  bandit17  bandit22  bandit27-git  bandit30      bandit4
bandit12  bandit18  bandit23  bandit28      bandit30-git  bandit5
bandit13  bandit19  bandit24  bandit28-git  bandit31      bandit6
bandit6@bandit:/home$ cd ..
bandit6@bandit:/$ ls
bin      home            lib64       opt         sbin   usr
boot     initrd.img      libx32      proc        share  var
cgroup2  initrd.img.old  lost+found  README.txt  srv    vmlinuz
dev      lib             media       root        sys    vmlinuz.old
etc      lib32           mnt         run         tmp
bandit6@bandit:/$ find ./ -type f -size 33c
find: ‘./run/lvm’: Permission denied
find: ‘./run/screen/S-bandit20’: Permission denied
find: ‘./run/screen/S-bandit2’: Permission denied
find: ‘./run/screen/S-bandit17’: Permission denied
find: ‘./run/screen/S-bandit15’: Permission denied
find: ‘./run/screen/S-bandit14’: Permission denied
find: ‘./run/screen/S-bandit9’: Permission denied
find: ‘./run/screen/S-bandit8’: Permission denied
find: ‘./run/screen/S-bandit31’: Permission denied
find: ‘./run/screen/S-bandit30’: Permission denied
find: ‘./run/screen/S-bandit21’: Permission denied
find: ‘./run/screen/S-bandit26’: Permission denied
find: ‘./run/screen/S-bandit3’: Permission denied
find: ‘./run/screen/S-bandit5’: Permission denied
find: ‘./run/screen/S-bandit25’: Permission denied
find: ‘./run/screen/S-bandit4’: Permission denied
find: ‘./run/screen/S-bandit1’: Permission denied
find: ‘./run/screen/S-bandit0’: Permission denied
find: ‘./run/screen/S-bandit13’: Permission denied
find: ‘./run/screen/S-bandit27’: Permission denied
find: ‘./run/screen/S-bandit22’: Permission denied
find: ‘./run/screen/S-bandit12’: Permission denied
find: ‘./run/screen/S-bandit23’: Permission denied
find: ‘./run/screen/S-bandit19’: Permission denied
find: ‘./run/screen/S-bandit16’: Permission denied
find: ‘./run/screen/S-bandit24’: Permission denied
find: ‘./run/shm’: Permission denied
find: ‘./run/lock/lvm’: Permission denied
./var/spool/bandit24/bandit23/output_from_run_delete_script.sh
find: ‘./var/spool/rsyslog’: Permission denied
find: ‘./var/spool/cron/crontabs’: Permission denied
find: ‘./var/log’: Permission denied
find: ‘./var/tmp’: Permission denied
find: ‘./var/cache/ldconfig’: Permission denied
find: ‘./var/cache/apt/archives/partial’: Permission denied
./var/lib/dbus/machine-id
./var/lib/dpkg/info/bandit7.password
./var/lib/dpkg/info/libcurl3-gnutls:amd64.shlibs
./var/lib/dpkg/info/libkrb5support0:amd64.shlibs
find: ‘./var/lib/apt/lists/partial’: Permission denied
find: ‘./var/lib/polkit-1’: Permission denied
./usr/include/x86_64-linux-gnu/asm/sockios.h
./usr/include/x86_64-linux-gnu/asm/termios.h
./usr/lib/grub/i386-pc/video.lst
./usr/lib/python2.7/dist-packages/PILcompat/ImageCrackCode.py
./usr/lib/python2.7/dist-packages/PILcompat/PngImagePlugin.py
./usr/lib/tmpfiles.d/man-db.conf
./usr/share/doc/python-pam/AUTHORS
./usr/share/doc/eject/AUTHORS
find: ‘./cgroup2/csessions’: Permission denied
./home/bandit3/inhere/.hidden
./home/bandit16/.bandit15.password
./home/bandit2/spaces in this filename
find: ‘./home/bandit28-git’: Permission denied
./home/bandit21/.prevpass
./home/bandit0/readme
find: ‘./home/bandit30-git’: Permission denied
find: ‘./home/bandit31-git’: Permission denied
./home/bandit17/.bandit16.password
./home/bandit1/-
./home/bandit25/.bandit24.password
find: ‘./home/bandit5/inhere’: Permission denied
find: ‘./home/bandit27-git’: Permission denied
./home/bandit4/inhere/-file09
./home/bandit4/inhere/-file06
./home/bandit4/inhere/-file01
./home/bandit4/inhere/-file02
./home/bandit4/inhere/-file05
./home/bandit4/inhere/-file03
./home/bandit4/inhere/-file08
./home/bandit4/inhere/-file07
./home/bandit4/inhere/-file04
./home/bandit4/inhere/-file00
./home/bandit18/readme
./home/bandit15/.bandit14.password
find: ‘./home/bandit29-git’: Permission denied
find: ‘./tmp’: Permission denied
find: ‘./lost+found’: Permission denied
find: ‘./root’: Permission denied
./etc/bandit_pass/bandit3
./etc/bandit_pass/bandit16
./etc/bandit_pass/bandit2
./etc/bandit_pass/bandit31
./etc/bandit_pass/bandit14
./etc/bandit_pass/bandit21
./etc/bandit_pass/bandit32
./etc/bandit_pass/bandit10
./etc/bandit_pass/bandit8
./etc/bandit_pass/bandit33
./etc/bandit_pass/bandit9
./etc/bandit_pass/bandit7
./etc/bandit_pass/bandit27
./etc/bandit_pass/bandit17
./etc/bandit_pass/bandit1
./etc/bandit_pass/bandit30
./etc/bandit_pass/bandit25
./etc/bandit_pass/bandit24
./etc/bandit_pass/bandit23
./etc/bandit_pass/bandit19
./etc/bandit_pass/bandit5
./etc/bandit_pass/bandit4
./etc/bandit_pass/bandit26
./etc/bandit_pass/bandit22
./etc/bandit_pass/bandit28
./etc/bandit_pass/bandit13
./etc/bandit_pass/bandit20
./etc/bandit_pass/bandit29
./etc/bandit_pass/bandit12
./etc/bandit_pass/bandit11
./etc/bandit_pass/bandit18
./etc/bandit_pass/bandit15
./etc/bandit_pass/bandit6
find: ‘./etc/ssl/private’: Permission denied
find: ‘./etc/lvm/backup’: Permission denied
find: ‘./etc/lvm/archive’: Permission denied
find: ‘./etc/polkit-1/localauthority’: Permission denied
find: ‘./sys/fs/pstore’: Permission denied
find: ‘./proc/tty/driver’: Permission denied
find: ‘./proc/7964/task/7964/fdinfo/6’: No such file or directory
find: ‘./proc/7964/fdinfo/5’: No such file or directory
./boot/grub/i386-pc/video.lst
find: ‘./boot/lost+found’: Permission denied
bandit6@bandit:/$ ./boot/grub/i386-pc/video.lst
-bash: ./boot/grub/i386-pc/video.lst: Permission denied
bandit6@bandit:/$ cat
^C
bandit6@bandit:/$ cat ./boot/grub/i386-pc/video.lst
vbe
vga
video_bochs
video_cirrus
bandit6@bandit:/$ ./var/spool/bandit24/bandit23/output_from_run_delete_script.sh-bash: ./var/spool/bandit24/bandit23/output_from_run_delete_script.sh: Permission denied
bandit6@bandit:/$ cat ./var/spool/bandit24/bandit23/output_from_run_delete_script.sh
UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ
bandit6@bandit:/$
```

Solution : 

```
bandit6@bandit:/$ cat ./var/lib/dpkg/info/bandit7.password
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
```

bandit7::HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

Bandit Level 7 → Level 8
Level Goal
The password for the next level is stored in the file data.txt next to the word millionth

Solution :

```
>>> f=open("data.txt", "r").read()
>>> f.split("millionth")[1]
"\tcvX2JJa4CFALtqS87jk27qwqGhBM9plV\ncomprehend\tFKVbjZbVgb0d2RU2DlCqSW049xMITQkB\nimprudence\tceeNKBMlu3nE9ZmG11iqXwe1FOfsh17k\nbenchmark\tBlZm92fuvV8NXHUP4QM6oL44CiDVh3I3\nchiselling\tx9cJLrnD1Eq3j3LGQWlfRQxCogL7tqAB\nswash\tzr2qOGA0OdSaILm4pTYj3HiCeUQcmMYH\nDixieland\tLKpbThseZz4d45aLJ5K7uBumeomEiTMj\npitilessly\tBmQkNtZEyY2hglJJnIZriuK9Yt8JbCIM\nlay\tNyNCS9E83dLXeha1nf8vjTMMeUFbBnnW\ncommercial\ (...)
```

OR SIMPLY 

```
bandit7@bandit:~$ cat data.txt | grep "millionth"
millionth       cvX2JJa4CFALtqS87jk27qwqGhBM9plV
bandit7@bandit:~$

```

bandit8::cvX2JJa4CFALtqS87jk27qwqGhBM9plV

Bandit Level 8 → Level 9
Level Goal
The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

