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

Solution :

```
bandit8@bandit:~$ sort data.txt | uniq -c
     10 07iR6PwHwihvQ3av1fqoRjICCulpoyms
     10 0ob6rCn4D4jQ6KCiaT5hmOdWFrm2quR1
     10 1drBmDT7PYS7hVgoTWkJSjUZUK7ZAIAa
     10 1JnkIYLDOdn5M7TGabYxOWkn7HazMjYW
     10 1wBrW0VGjKeYiXltbEWrUipwSHQfTu44
     10 2Dxbtw8cnKyHwvt0lfFNYOGc4cE59uua
     10 2TRkCQhbMjcM0hwL31NnJQ0DVagWN3Ca
     10 4c7EsUtqLnLR9hiepV5EQVhdMgyi8onL
     10 4cQDXE4IPH8fCBUBZaTPgnY2gwnPnlj6
     10 6495bfC0lI1Qkw5kzZHnbVWooaOZHLvj
     10 6rEzM4Qro8dH0e3uemAyYseTiNiNAYap
     10 78rgduVcLZjLzZmooObdaN541MKV6IfQ
     10 8qkrbCAUG9I28M49j9flUro5fWxenFzF
     10 aIl4xN5maZVCQITz0xH0KNXIlLc0MhNf
     10 aPsCQmSWVYGQQHUD6k1fHC2kqSyMlxwV
     10 awglWaTRSAWBcol8hSMTJP4FYhIGJHVO
     10 bCJdTkork5IRbZaaPZK0WVPgYIIO4mHF
     10 BPl0XNou7xAZAI5fdzWzSmPkW1PnvTE1
     10 bvIaDTzHBOGSO7CfpH9vUrJRRlwYTUA7
     10 CS8HVrDmKGLG53qziqQCLWNRlUP1FHsV
     10 CwwHDVp0pO6zmFp87L9AtFzqU5aB5j9w
     10 CyziIvGRdotoy9yA00RAnvvkvrYdKCPp
     10 DRqDxJYAv7IUfAMmrXtXEiz63TUjqeDn
     10 DXI6y5CNPU06rVpkoZgnZJBWfkdW131j
     10 enNw6tuj8mSxxS7f2Yd05puXVeuCZ39G
     10 ewllxPExW9eaHxAH8WZkW9lDuK5cZcUy
     10 eyKcuNPKnjt25kaOZxkMYQ9xqp45aIk9
     10 fIBXc239DbhORY4t9xjgi7fSm4thHsIb
     10 fiK30QpqzoULACXZwkBEKJZvpPQx9Uqm
     10 FlHOKVUDNLx6Ga7CxC4ISRYNflN1GAnF
     10 G4BHP66B4l3XkvB05CMgzrEKyjHhuCwz
     10 gCx35PlKn08nrFFrAgHYLrUVWWZjLdqM
     10 GEzwi36aKB8PLlCPH2wzl9gHzVm97IYu
     10 glONDdR72FJL3Gc03nVNO4PKNzXFGH1A
     10 gqGBgY1IdFDGG2XzB2o1VNGY4j6OL76V
     10 h7jtcUsBhrryyLhtt1mT6Jdmp0l6ozBs
     10 HKryX0XX2HT4WBT0OUzRz5Ac5B2rvIHU
     10 iM3PaCO3VAxAdbdVsdGtEwuwrFQPYJV7
     10 irGm6F73sbUrFhHukhp6JXgMQyLxJTz1
     10 jtNdk5KDgrMkxgbZSJOvjOcM58svrzDY
     10 jVscZ5eK5DWN7IvDSehXmyplCXRSbHJS
     10 KerqNiDbY0zV2VxnOCmWX5XWxumldlAe
     10 kha3sCpHsydUNrxLLXV3cFqWyucGjdxr
     10 kt1VUEZpimCS4BaoAvhN3rgHOmhqaMIR
     10 KUzqHCrxHSpgfkF5ZAzUfjlBaXW3zIaZ
     10 L0nxAwlfV9V3J5onKIT8KYQ9InTcQ7yE
     10 lnB8MWOYjETxoC8bQYrMFnxxQXAWHjP4
     10 lZ9DhnzeHgIuLqYPmNzONpMCkuBYoeJI
     10 M8JMUd7MSd4mOwZj1843ejBH5RXJOloa
     10 mdug9JbW836YVZh3ALULBAxODlinqonJ
     10 MIpMch66sYTmmqepKYczlRA9aJrnkt68
     10 MpAqsgjJIVLT1MxSZcRoOOzl6g1db98Q
     10 MQrydyojsVIYJSY8y1nCMjZGxnL1My7F
     10 MsxcvOe3PGrt78wpZG2bBNF5wfXpZhET
     10 n5fEmvCXKbJErzIDt3MLTmZZVMRNynrR
     10 NL91hwGrqW5lVgoicb592Sd0djnHnbjZ
     10 Nnih4Q0jf3xEOTcmM3yw2HkOm3VPox0w
     10 NT4p09XwRb0k0wG9yIuvfs3MblMGpMc1
     10 nU5zbsdUfmzv7cjNwkV9Hgb65OVe5EDt
     10 nyvBweoC3kzt5QRTjbDfrWO7jhwOGN4g
     10 OcVxHzDW027KWNFS03G31KQEb5TgN1WV
     10 peXkYozDKE2u2BEOed5vvkY0nyjkGawn
     10 PXHEt0PztCiArDZ7UCBmqKdBCiXNQWBN
     10 QmFayGbrzFoiQ5Z2PGmnD2N6Pf77cxl9
     10 QNTac9UtCmQ5VGAnzj10Z9BwV4TuaVvu
     10 qsbKthWb80f3vQKBP7O12SjfFo1V5VkL
     10 quhCb8ZIUJXXM2SbY1ER1D5GaDlQjdDa
     10 QYeOFhgJCJEfKM1ZpT0K322R6SuKdCFT
     10 r0VIMA1yzv838m7UfvutUhCf0zaY3Rqw
     10 rfUNSGOvmQXz0m7PtFoEoPg1BpTbll7X
     10 rJMbGeeDTMsj1RA4YibIQr0o9azHgP0I
     10 rQAYnkKAXIViP4ROmehnDMIAXLpOOLEp
     10 sBB2H7HateUFxr2oxrqUVoumFM60f1lj
     10 SjFHXKRcIc7jlAYGknVMnGXSFd6xRmnF
     10 tDZbF2SuhsvfaA3eTnwfcjQa1pZoPJeX
     10 tiyVGzZcRwUPVAiqkroFMUbMI9ut9hcT
     10 tLKyRATtoCuxMR4zZg1Dnlnr3je3bSHe
     10 tmzBM5rcV9y7AM1xDHudL2yX9oefGieT
     10 tWwjd16fG17vGdjutfOygVTjEGxlijOS
     10 uBRx9inQTeaDZAuzEb2MadWXmkH8uW4O
      1 UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
     10 vBo3qbjNEF2d3meGEkRfc3mKpjtiDz1i
     10 VElUBEIhJ4yBgOBSN05WgtV2rF6kkGdz
     10 vl9liaz8TKv1enUi0S2REhn01hKjjFIK
     10 vVwG2mb8rU8eCuIlBhCJrZJ4GWR35nWY
     10 W0vbGkT5mfRVWHAXCcMekevbenMJHFhN
     10 W6pn7siBPh5G6ndjv1xx26iHxke8PviX
     10 WaKxNQhiI9dXwvzB1PMpbQRy4CutGrWt
     10 WbfstqfIvgiEuCVVuxwLgLyzUMtho2jP
     10 WBjoFnis277W9vWB8M67h3z1glOYG2Fy
     10 wSpAMdiBSeywE4d1DQZoSp5o8ZVOCqGP
     10 wWfTfhYKmBkmyGH9D6Qjb6x7bMt5narC
     10 x0bga8Oxz5lgM8k52HrYy4ez7XJI0lM0
     10 XURYdoIx95clq6s90MORDydQ187DxQhS
     10 xWmqkcrZ7TmjE7LKjqHVXSLw9fqsjYXp
     10 XWy99VXVCnwdr780PK86hP6rBMkV5E3n
     10 y9sn56N0ZhyxaySYRs518D4vqkMShHwb
     10 YiQvaaidmD39i0ryGZz97Upc5NjgPklY
     10 YR0sflfJZ34iuY3wM3DNNO19dBYnJDmt
     10 yXGLvp7UaeiDKxLGXQYlWuRWdIgeCaT0
     10 YzZX7E35vOa6IQ9SRUGdlEpyaiyjvWXE
bandit8@bandit:~$
```

bandit9::UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

Bandit Level 9 → Level 10

Level Goal

The password for the next level is stored in the file data.txt in one of the few human-readable strings, beginning with several ‘=’ characters.

Solution :

```
>>> f=open("data.txt", "r").read()
>>> for i in f.split("=="): # heuristics: "beginning with several ‘=’ characters."
...  print(i)
...
ʿ▒|g▒{Li&▒▒G▒[▒W▒K▒▒z
Ђ▒`B6haѩ▒▒▒T2▒*D▒"▒▒i▒EJ▒MPC▒n鮝▒▒O▒{Ov▒▒q▒lk▒.MBB▒▒I>▒[▒dW▒V▒t▒8s▒▒m▒▒▒Bt▒▒{
          ▒e▒c%F▒▒▒▒T▒nK)U2u▒▒L;▒▒[ۙ0i▒y▒-▒▒&y@@2v/▒▒▒%Z▒▒}▒▒▒▒8▒X▒.▒▒y_!}▒▒H▒▒ɝ▒5Lo%▒▒e4▒R@▒J▒@▒(D▒?۟▒۳?▒ߎ▒uv▒▒▒޷9▒ٱ▒ि▒`a▒▒|▒Ӓ▒▒▒▒CW▒▒▒▒▒y▒$▒▒|▒s▒L▒▒8▒▒▒x÷2▒E▒֯QS▒]▒'▒C`▒▒▒▒▒ru@n▒▒▒:▒`▒98▒▒▒D}U'▒!,▒n▒P▒x▒?▒/▒
▒|▒/~▒r՝T▒▒▒T▒▒,|
"*J▒j߀hW▒X▒E▒▒▒▒e#s.    ▒o▒▒▒BNZ▒`|{▒ߡ▒̞ł!Gr▒_▒  ▒▒▒oH▒D{▒▒!:/%p▒▒▒▒▒!▒▒K▒5▒▒~▒aX▒▒▒▒▒▒"P▒▒▒▒N▒ D͜▒▒*'dZ▒!!ivp▒*▒▒▒bgM>H▒▒▒▒wx
G@?>▒|wٝ▒c▒▒N▒▒▒̷X`▒▒UyH%u▒▒L/▒▒^▒5▒h▒M0d>uG▒▒^▒\▒▒
▒*▒▒▒Ĝ"a`*▒+F▒OH▒▒Xy▒9▒▒D▒P▒^L▒Ȗ▒▒'
                                   ▒▒▒P*▒▒<▒▒▒a▒z▒▒▒38zT▒}4▒\H▒-S▒|▒Ҙ▒  ▒)Šb▒bz%▒▒\\▒▒▒G▒▒-0▒▒@▒▒^R▒l▒"S▒▒B+▒D▒t▒▒H▒▒▒▒FB▒▒▒ȭ▒▒▒*▒/E\N▒▒▒ٔz▒▒▒}▒7▒g`mNg H▒=d▒▒.▒G▒▒▒▒r1▒J▒▒H▒▒Y▒c▒▒8▒M.M▒?]▒J▒▒▒:U[,▒▒▒g@▒b▒▒qs*Y)▒%▒▒W̄D
▒h`▒▒e▒N▒▒V%▒!▒+c?Vh▒r▒▒[▒▒-▒▒3▒sw▒▒▒W▒P▒       ▒o&9▒8▒▒T㖶▒K3▒`▒CEhL5d(}▒▒,▒▒▒▒h▒W▒▒h▒Ə
c4|▒"▒X▒▒▒▒m▒▒▒Y▒▒GB7▒ճ&▒ե▒▒p▒▒▒▒s#▒k&K▒▒1▒▒s▒▒֯F▒B0▒2




 the▒X▒#▒▒!▒n▒~▒
Q▒tR▒epO▒~c▒▒|▒K▒$▒U▒▒D▒^wo▒▒▒Ӹ▒`▒▒^Q▒▒▒"
                                         Sf2 ▒▒6▒▒r▒¼▒<CN▒x▒B▒l1͑▒
▒▒2|▒▒▒T▒]Sĳ@)▒▒m'T▒▒I▒▒ʲ<▒k▒%U▒▒/UG▒▒▒Y▒o▒▒▒+▒`        O▒aX▒▒bZ▒?▒▒▒LB▒▒C9▒▒5iu^B▒▒▒▒▒=2D=`▒▒▒oD˂▒n▒Kh▒▒Ȳ=}▒▒▒"▒vH▒▒▒▒u9#e1[u▒>▒▒
▒▒.S:▒▒OM▒▒J*▒▒k45▒V▒yB▒▒Z▒WJ▒▒▒▒p▒=▒▒▒▒▒KΫ&䄍▒▒Bes▒▒▒y $▒▒▒▒D]~▒▒▒ʔ▒_▒^▒hv▒▒▒▒߷▒z=▒▒X8▒֔▒t▒▒▒C▒3¯       ▒▒s▒▒%▒▒▒<?%▒_▒E▒▒▒▒▒.fF        ▒▒▒▒Z^kV▒e▒H▒▒d▒▒▒4}▒▒▒▒▒׬ʗ▒
▒O▒▒▒Ӎ▒ 6▒I▒▒▒#▒▒▒▒▒o h2▒▒▒0/6▒0▒▒▒-▒F▒▒^▒0▒▒▒k+0dbunJ!▒˒▒7;▒▒h.TF▒4x&▒",▒▒Q▒▒pE\▒▒▒bo▒>V       Iы▒^▒Zaf3
▒w3▒(>▒bჃ▒2▒Q▒~▒.ƴϺ]h$ 4▒▒ud▒3▒▒j▒▒Uk?▒▒▒▒⩮
   Wj6▒/▒GY     E▒,ebr▒k▒▒▒▒/▒Cg▒▒GCQ▒▒rS▒▒▒▒▒▒▒▒▒r▒޻▒I▒▒E▒\▒▒'▒P▒1▒▒3▒▒▒m▒▒}ԉ▒▒▒▒i$Vh▒h▒▒▒▒▒:H▒/▒▒ȿ▒$zJ▒▒▒▒▒ǋ▒)~▒]v▒,▒X*▒▒▒    I6g▒▒c▒x▒▒Q▒▒▒~▒▒▒▒▒▒@A▒Ca▒▒▒▒▒▒b▒߼p▒▒▒po▒&S▒▒N▒]▒▒▒~▒}▒▒▒▒BJ▒ ▒▒%m▒▒v▒▒▒▒?(▒▒M&▒1)▒k▒▒_▒▒Ŧ▒}▒▒#[▒Q/^▒aַ▒▒▒▒▒3▒▒▒i▒▒h▒▒▒▒'{▒H=▒Z▒,▒CL}0Vx<M6▒▒N▒▒▒▒ V▒ ▒~▒▒:▒*ԟ▒mB#L▒?W▒▒Z^▒▒.
                                                                                                                #▒o6▒4t▒▒0▒▒▒=▒▒bl▒▒▒▒▒▒?▒]|Ě:V▒▒4
                                                                                                                                                  /U^▒ba▒▒▒S%T{`G▒▒q▒L▒z▒▒▒f▒▒▒▒ҋLUu]\▒R▒▒▒▒▒▒▒KR/▒▒▒▒l▒▒▒
f▒6,▒ݺ▒▒▒V▒ٷm▒▒▒▒{▒5C
▒Yo▒▒▒=H▒▒!AwV▒ٜاy]▒&▒:▒z▒e▒▒Qhy▒?▒Q▒Q▒▒1ň▒▒_n▒'▒▒A&Ҟ▒▒Z▒%▒q▒▒Q▒▒▒▒D▒}▒w▒⪫▒T▒:▒▒l▒j,▒I▒▒▒▒▒o▒8▒C▒▒8▒r▒9+▒@T.a-▒CX▒E▒껩<9▒6NJ~▒Ї▒b2▒▒0▒ѳ▒H▒▒▒▒iR▒UE▒e▒▒G▒IGh▒▒▒▒w▒1▒▒%QFc-▒▒▒▒▒▒]▒$~9+▒▒▒s▒T#▒9
▒▒<E:C{{▒▒0I▒/▒-▒
         ▒Q▒▒D▒c▒▒E▒▒^▒
▒k▒▒▒p^ͳ(▒▒▒▒▒'▒x"▒▒m<▒▒
▒2$▒▒▒▒H▒[s▒r%▒▒▒▒▒!▒'▒C▒w▒<.q▒S+▒m[▒9?▒ƻ▒▒2▒▒▒▒'▒T$(▒▒ԛ\ҟ▒M▒,▒L▒▒P▒$ju▒w
                                                                         ?▒▒▒▒0▒▒P̥▒!|#D▒KŠ▒▒#GF▒q߫▒▒P▒R▒.b▒J▒F{▒▒fA▒^▒▒▒▒▒ҖxP▒▒4▒TƟ
▒▒▒Y▒Z׻▒▒lJo▒▒▒1▒▒▒ 6▒j▒▒Y`▒▒▒▒▒▒L8kk#A▒sRb^▒▒▒=2▒▒▒▒+*▒▒▒}j▒3R
▒]▒{vbT▒>ӏ;▒w'▒▒@▒▒▒▒▒❘t▒n▒r▒_▒▒▒ ▒▒;▒▒▒w檅▒sq.▒˳ ▒▒▒▒▒▒▒▒1mBO▒▒"?@▒▒▒▒\▒▒▒y▒l^'▒g▒▒▒
^VS'▒
▒▒▒v>h▒▒▒▒3▒▒▒▒l▒▒3bF▒▒▒▒▒▒t▒A▒$h▒"▒▒-尅▒oFP/;l▒▒▒▒▒¥▒ֳ▒▒▒ ▒rˀ▒▒6▒J&▒5P▒▒)Y▒▒▒#▒a▒▒▒ŧ▒▒▒▒[m
                                                                              ▒|}d*m&-▒׵?kr▒E▒▒▒|▒R▒▒Į▒▒8▒▒▒Sy-▒\i▒K▒   ▒iΞ▒▒ʴ▒▒▒^▒▒J~N▒▒p▒O▒
▒j▒~;▒▒~z▒e▒▒0▒Y▒▒▒p▒▒▒WYC▒▒▒▒▒a▒z▒▒<▒▒K▒▒"3▒▒b▒▒'׺▒N|▒▒▒Q"7d▒▒9▒R-▒~"%▒▒w▒^▒▒
▒; 4Us▒▒JI▒▒▒▒#▒Pl▒|7a!(Yl▒▒of▒▒▒l▒8▒zއ▒җ2▒▒_)Z▒_▒▒▒c▒▒▒&▒▒d▒▒▒▒▒▒▒▒(W▒j▒Z▒▒!▒▒ߗ8▒▒G▒j▒]▒B▒B8▒yY(▒▒2▒/▒▒|▒*m▒S▒
                                                                                                               ▒'"▒e▒۰▒▒▒▒▒▒c▒i▒▒▒▒@Z׉▒W]▒▒(▒▒G\@P▒ɂ▒u▒h2aO▒;sx ▒▒▒|▒C?▒A▒▒▒0▒▒▒ř#▒>▒ɓ)ˊ▒;l▒▒XvMTP▒▒▒C▒X-▒▒3cp֗;▒▒Y▒E>?▒▒▒D▒%▒▒▒Hm["VHL▒ f▒▒M▒▒▒▒▒Q▒%Z▒▒d▒▒▒}0ν▒▒▒nU▒;C▒▒▒;m▒▒▒▒~冸▒I5▒r7t▒▒GR▒▒;֔▒3Z>▒b@I▒▒7▒N(▒▒%s.▒K▒▒▒d%)є▒k▒▒V=▒]t▒,]▒▒▒▒|,ZO▒eE}▒▒[Q▒▒J.▒▒▒g▒R▒%JZ▒▒▒v▒B▒`I▒h▒͛J▒▒̨▒Yז▒b▒       $▒&▒&▒▒▒▒:▒▒~▒▒▒▒▒/▒▒.▒▒▒▒ԣǝë~"
▒C▒▒9'▒▒▒▒u▒b}7▒▒J▒▒�-▒n1p      A▒?R▒▒8▒o▒@▒# ▒D▒O-I▒ِH▒9▒w▒1▒▒▒ߋ▒       \=▒▒/O▒L▒@▒▒▒0▒▒▒%▒▒TE[S▒h▒     ▒T$▒▒▒[<▒2n▒5▒▒▒b▒
%E▒j8▒▒n▒a;0\▒F*s▒^"5                                                                                                     a{▒e㢦▒78A▒I▒(▒7Q▒-▒▒▒        ▒³▒=▒]▒▒▒L,7▒▒3EQi▒u▒)'0U▒▒▒u
l▒_▒az|Y▒▒▒k▒B▒▒B▒8.M▒9▒=▒k▒▒7▒1▒-1T▒▒▒
                                       ▒U▒!▒w]Ov▒û▒
12▒▒▒J▒Q▒▒▒< ~k▒y@g▒Y&▒T"u▒M<▒▒1▒▒▒n▒▒;▒=QXa▒▒.▒D#w▒3▒[▒▒`4F<N▒▒▒51▒k▒|f▒▒▒a▒[▒iF▒>{F̮~▒▒c#p
                                                                                           &K▒▒▒▒ds▒▒h▒▒6z4▒▒P▒▒ƞ'▒▒▒}Q▒w▒2▒av5▒=|▒/
                                                                                                                                    ▒W▒5A▒▒▒
Ԩ▒P▒FrZ▒YL▒@▒▒)2▒▒▒i▒▒▒gG▒▒˴H▒+▒▒▒▒OaT▒v▒▒▒▒)▒▒E▒M▒y▒k'r▒yU▒▒Tf.▒6r▒▒▒G ▒▒▒▒}▒▒▒▒
▒

 ▒tf▒▒#▒/▒▒▒▒:▒'[▒!ǐ/;▒▒+▒M▒▒~▒B>▒SJ▒p▒▒▒9▒▒̼}>▒7c▒▒c▒W▒w▒=▒
     W▒_H▒Y▒Y▒▒ĤdX▒▒*▒4▒B▒▒▒ ▒z0e▒▒g▒▒S▒V]▒O▒▒J Q`▒*TdI▒K.:}F1▒▒▒'▒▒    \Ӽ�▒7P
                                                                              []▒▒i$2w▒▒t▒Z▒▒$▒▒5▒▒▒▒e▒▒.f▒O▒▒qݡ6▒▒▒▒▒▒-▒G▒uG▒▒)▒^▒▒▒@!g7▒▒L▒Ѯ▒2▒▒▒#Gd▒▒; ▒▒岬▒MS▒▒֌v▒epg~▒|ݞ$q▒q▒k▒mU▒▒hu▒z▒▒Ys▒|▒▒ƅ▒▒b:▒i^eE▒▒▒0Q▒>Q▒{]▒▒gU▒▒▒7f~▒▒e~▒▒%▒▒V▒&▒i▒
                  '(U▒#O▒TӲ▒▒T▒m▒▒z▒▒*▒S\▒▒▒g▒▒▒M&T▒▒▒▒þ




 password▒▒Z▒▒
              ە▒
▒'▒▒ϰm
▒▒z4▒p׶▒\▒Q0▒3▒z▒5▒)▒E▒)▒0`▒▒B▒▒p▒▒w▒▒FÍ~Y▒Ks7▒▒PUn֘▒;zO▒▒9E▒ŗE▒
%▒K▒▒NHGu▒▒▒zuH▒WZ▒(▒▒▒#ƈ▒▒{z▒[]/▒#▒▒▒▒▒▒E;NԬ▒3;▒c▒Z▒▒΄z
                                                        ▒
▒▒=▒Nh̏;1▒u(▒
+xDZ▒X▒½▒▒a▒P▒▒▒
▒▒▒▒P▒▒7▒"▒▒%P▒Z▒6u▒I▒=ػsz▒3pg▒˪
8▒▒▒r▒CM▒-▒▒P{▒▒@▒k▒▒-!▒K▒ג▒▒▒F;▒ر뿓`▒0▒s▒▒▒=▒ag▒%Ff▒▒y▒▒6G-▒▒Xy3▒
▒▒M ▒u▒|f;P]!▒▒+
rǹa▒^▒2Uk▒▒▒~5&:֢▒}▒▒hja▒▒*▒=-ק▒U▒▒v▒x▒▒?▒▒yi▒▒<▒▒V,j?^▒▒▒#l▒▒U▒/-?d▒▒ag\▒5▒▒a▒PÖS▒8▒▒ [▒
▒▒▒▒+o▒▒oc8,`:?-L▒▒D▒u▒N;?▒▒▒\&▒▒▒6▒6▒K
▒▒x▒▒B#
▒IR7▒▒Ȓ▒KC0▒▒▒=▒▒▒▒~▒"Ԓ▒▒▒e▒▒▒,▒▒.▒▒TEӁ~f ϼb
                                            k▒▒▒&▒▒i▒6▒4▒▒▒'▒>t=        yP▒▒iI▒▒▒▒▒
O▒^▒J▒4I▒▒!▒3▒▒[▒▒uB\▒▒▒^▒▒▒W▒#f▒x▒▒*▒▒'▒&F▒▒t▒▒/▒▒L▒G▒p▒▒▒@▒▒▒5▒▒;▒X4▒▒g ▒^04>-▒;֚ ▒▒+'0▒4▒▒G▒gM▒▒▒▒▒_0▒Y=▒b▒▒V5▒L▒▒H"▒uP▒
H▒{▒▒▒▒9▒▒▒|▒▒)▒▒ N▒0▒▒n▒5▒▒V▒?o~▒r▒띊^8x▒;tw3y▒▒▒SŹF   >t▒ܲ5RR▒▒%F▒▒▒▒▒{b▒'婄1▒ImV▒▒2▒Uk▒[[N▒▒▒▒ ▒
>▒▒xo?C▒O▒7;▒h\h<M▒▒(▒▒t▒V ⁆O-▒▒y▒▒&B&l▒▒U3"▒
eNe▒|S▒{w▒▒▒g8▒▒▒N▒E▒▒▒\<▒fo▒▒D▒▒T&n▒]▒▒
DgdJ▒&E▒"▒Z9I▒▒▒2▒--▒0@▒▒]<▒
                            ▒▒▒w▒c      _<9>Ds▒▒Qc▒9▒:/▒|\4▒▒▒`Lܔ▒▒▒▒Igzz▒▒▒▒G▒!▒M^,▒9Ų6i▒▒//Jr▒▒Ы▒]▒MF▒9▒:DLq▒▒1xI▒▒▒~▒qEk9s▒▒0▒ѐNT▒(▒tQ▒P▒▒▒p%?▒h▒纸▒▒▒Lq▒▒▒▒1▒6▒▒▒.▒▒▒e▒S▒E▒QO▒▒▒ci`2▒u▒▒▒H▒.▒▒~@▒▒Q▒H▒▒u▒▒ړo▒▒T▒
_K▒T▒th▒▒ߦ▒{▒▒▒%
$▒WI▒T}▒0p▒▒ʦ▒m▒t▒/▒G2▒▒8▒
▒F▒▒P3c([t▒' ▒kmx▒▒Ê^E"▒R▒▒ TN▒^6       ▒z▒▒▒▒r▒Dw0▒▒y>?+▒~X▒▒▒▒ʒ▒▒fut▒Mf▒▒     ▒䳷%LˤnW▒s▒=$▒P▒:▒H▒▒jgF5X.▒T}~_Z]▒▒9▒r▒4/▒K
                                                                                                                            ▒93▒4▒▒n▒@▒JT▒;▒▒▒▒▒▒




 isa▒4>▒P-+i▒▒_▒▒Z▒0u▒#▒$OGuEz&.▒▒▒y v▒▒▒▒u3 5wB▒▒▒+˸▒▒▒▒▒
K▒)▒▒I▒▒▒-Mz▒"▒▒▒▒      ~▒▒AG▒
▒"k"}ηQ▒▒ƋF▒▒▒  ▒▒Xy
▒?\▒YG▒▒9▒c▒▒▒▒3▒▒ɩ▒3▒v▒m=▒▒?F!XW▒H݄▒▒˸7yA1H]W▒▒▒r▒▒l▒r▒▒▒▒
▒▒▒O▒▒▒▒aZ▒nĮH▒X▒DM(▒$▒D▒▒۞c▒=▒|$▒▒1v▒▒(>▒▒"▒~׻▒ ▒WMSXEO▒▒▒@0▒j▒9'▒3▒t▒i=q▒Q▒h▒'▒▒▒
                                                                  ▒▒0
                                                                     ▒▒p;8▒▒▒▒▒▒9T▒▒▒▒Q,9_▒u/▒c▒▒Ҏ▒
                                                                                                   ▒$!T1+▒d}▒▒Ē▒?֩       ▒֝▒#R5▒R▒u>▒▒I▒
▒▒ͥ▒ʖNX▒▒̛O▒▒k:▒d▒Hw▒▒4T▒▒▒▒z▒▒▒;▒2▒뇃▒▒6▒▒k▒|I▒a>:▒▒▒▒▒߆ܝU▒5#,]▒▒R#▒▒QP`▒▒s▒▒ʵ▒E▒▒▒=&#▒▒ך;H▒▒▒▒7▒:j▒YR▒Y▒▒▒▒iI▒▒,▒;OoR▒C-▒▒`W▒<▒'=▒PV▒▒-▒qw6▒W▒rt▒▒▒BCC▒▒.▒=9▒▒▒▒ԫ▒k▒.▒[m$jJL*\▒▒oM\U
a+▒g%tq_A▒▒y▒▒▒!'▒▒▒`▒▒▒"▒ϲ▒ݶ▒kIN▒▒▒▒f"I▒▒u▒1_d▒▒
▒▒Nt,▒▒▒d▒▒▒ɖj;ލzÕ̡7+▒*9ڵ[-▒▒▒LL!▒y▒vw▒l▒▒&ѸU▒▒c▒▒68▒▒▒▒L▒H▒▒▒▒V▒x▒▒`fU▒rE
U▒x▒ ▒▒r▒E▒π▒▒?{▒▒▒▒▒v▒▒g▒/▒+▒Bh▒▒▒▒▒"dPy~▒▒B▒▒▒▒▒▒4▒3▒I▒▒
▒V1▒▒▒▒q▒▒▒▒ݎ▒▒▒t+▒U▒W▒8▒▒▒-▒▒▒ʪ▒MH`▒▒▒EJ{▒e&/R▒▒▒:▒X▒▒▒▒ZU▒▒▒"u▒▒\X▒E▒▒▒▒▒▒▒▒k▒ɏ▒▒Ĵ▒@▒Ӏ3g▒:Y▒_▒\▒▒▒▒j▒`▒<W▒czdy▒E]▒OǤ"▒WӤh;W   ▒▒Q▒̱▒dr▒
▒$▒▒▒5▒p▒▒▒▒▒k8▒GJ▒▒▒1▒T▒▒▒tj▒▒e▒&▒▒▒▒▒s쁌β▒;▒3▒▒#*́Pj                                                                                   ▒
                                                     ▒g[W%▒▒▒▒▒
                                                               ▒▒FLF▒▒.▒d▒▒▒8▒A▒o▒▒^▒m8▒6▒▒▒▒▒▒
                                                                                               ▒f▒▒k▒▒h▒▒Pϻ▒▒ ▒3▒▒ʞ▒▒▒ I▒▒▒▒J▒▒=FQ?P\U▒
;▒▒K+▒F3▒▒"▒w▒ܲT▒B▒&▒&▒e▒u)▒▒▒▒▒I▒0▒▒▒u▒#u&      ZQ~f▒sMF}X݉▒▒
եY▒:6▒▒9#▒O▒b▒Moܓ(▒F{.▒m▒▒▒▒N▒J,▒▒Ԋ▒▒&▒�▒▒▒I`H▒▒▒b▒x▒ǵd▒}▒▒n▒▒▒yuĹ{▒▒▒_p▒▒AAt]▒▒▒#<}▒▒▒▒h▒▒~▒▒vg▒▒&▒▒▒▒sE▒H0▒׉Ƽ▒+z
▒_P▒
▒79ζ▒8a▒▒v▒▒ɰ▒Q▒։▒cv▒Ӡ▒`▒P▒̓P▒J▒▒▒Gy▒▒ԆcB▒#Z:
▒▒INo▒ɋ▒*A$▒▒.q▒▒(▒                         ▒<‾`▒▒b▒▒zu▒▒▒T▒2▒H.yKk▒r▒3w▒t▒UWf▒▒▒4▒U▒▒▒/ۃQ▒e▒:RleK▒X▒▒CJ▒j▒▒!8▒▒e▒82▒▒▒▒▒q▒▒▒▒▒i`▒i▒EG▒݇▒▒GU▒▒▒
k▒▒t(▒@}▒▒▒c▒\3;W▒4_▒?bP▒d$▒▒;▒z▒$▒oZ_N܅▒tz▒
                                            ▒▒▒"Wˮ▒▒K▒q▒l▒5▒▒ͫң4▒▒گ▒▒▒?▒▒1خ▒F▒)o▒_[▒▒▒ׯ▒▒▒▒▒     ▒U4@v▒▒l▒▒,
;▒▒R▒'*▒E▒▒▒▒▒  w▒▒▒▒▒C>▒R▒D:▒▒r▒▒EC;d▒▒l▒▒_r ▒▒▒CN▒ʿ▒ī IOG+▒8SE▒0P▒C
▒E^▒▒▒!▒3▒6▒w▒▒$▒_▒ ▒▒▒▒▒~l▒$]▒▒9
I▒▒K7e▒▒▒▒q▒▒▒Ǭ▒:▒▒▒▒_▒-▒▒f)▒▒A?X▒T▒▒▒▒▒▒ϵ▒H▒▒0t▒)+5▒N▒▒▒1▒\?▒
▒F▒R'▒▒▒8_▒▒3▒▒▒▒>▒h▒<▒P=d▒r4▒d6▒▒▒}:▒y▒▒ʓ"▒▒▒xw▒y▒1iO˾'fQ▒dA▒▒▒G▒▒▒▒^՜▒▒F▒U,{▒▒▒▒▒▒\▒▒▒▒M▒
                                                                                           (▒/▒*▒▒▒wt2N▒j▒w8aU▒j▒▒▒▒
▒▒▒L▒▒▒U▒;▒C}.▒▒w▒Y|▒l`▒▒▒i▒▒▒th▒▒C▒G=!▒_▒i▒▒▒▒▒▒﹆▒u ▒▒▒▒|5▒{▒-q}u▒▒%9▒vy▒=x`㉧▒▒▒b▒$▒▒▒▒▒▒l(▒▒5eQP▒h"▒▒▒
                                                                                                          :
]B▒
   A▒▒▒;▒5▒u▒LP▒▒▒⅜G▒▒\▒snn`*▒?▒▒▒с▒}g
                                      ▒)▒▒▒i▒E▒e▒>▒|▒▒A=:▒▒▒z0▒▒|{▒T,▒W
                                               v▒(@▒ҏ▒>▒▒
▒pV▒]▒▒P▒▒▒E▒▒▒vp▒▒k▒▒▒\t▒KƊ*Nn"T?X^▒▒▒D2HM▒hnQ
▒o=D▒▒▒t▒▒▒A▒▒▒W▒▒M/3▒>▒AÜj▒    ka▒▒
                                    ▒`W2▒▒▒▒c▒x▒▒▒_D▒▒y^▒t▒▒▒\܀▒▒▒H▒D▒▒l▒?u▒M▒,▒w|▒▒7▒B}'▒▒aZ▒▒eW▒q▒▒أ0▒▒▒TT▒V▒▒Se*▒▒N▒▒X▒U▒5
D$▒▒+=@▒p▒▒z<X%▒▒▒▒/▒$Y)&wA     Y▒\▒[N<T▒▒▒n▒:▒x,r▒D%t`{▒wo                                                                  ▒F▒        ▒j>▒ɬ2|▒▒.▒;▒H0&t.▒▒4▒▒▒߫▒i▒#▒9▒▒
Q▒▒S▒
     ▒▒▒4_▒E▒▒j擡\<Nj▒?$=▒▒f▒▒▒.▒▒㴥▒▒▒▒▒j▒a3▒+▒$▒\Zo\h]▒▒Q|G▒▒b▒"▒X▒xh▒ߟT▒▒!厳▒R)▒g%▒▒*▒ڣ▒▒W▒▒W՗'NL}B▒▒▒▒C▒▒R▒^*▒▒▒RR▒▒▒9▒▒▒\r^y▒g▒,▒* +ta▒▒▒▒▒▒^Px▒n▒▒▒▒▒▒▒փ▒▒mƨ\S▒x▒t▒v▒b▒P?(▒F▒Vp▒▒%▒▒▒▒`▒M+)▒/▒▒▒Fj~%EޕD▒د4▒Ɵ▒i▒▒▒▒kI▒sF▒nT▒G;▒]▒▒▒%ĺ
}ד▒▒!▒ǭUd▒▒z▒▒v▒▒YG▒▒▒P▒o▒▒e▒▒ɪ5▒#▒rB▒5m*rU?w[▒▒Y▒/<▒▒▒▒®▒BE3K▒vJ▒▒O▒▒G▒▒Bk▒▒C▒P1▒v▒ӊ▒▒K(       ▒▒H▒b▒Ip▒▒▒@▒▒▒¼▒▒▒
                                                                                                                   ӏ▒▒
▒▒2R▒'▒▒k▒V▒%p
    ▒▒}
▒0▒▒▒oX▒7▒+"*▒▒>2▒'▒▒▒▒as▒g▒|▒b▒▒=▒▒Z▒▒]o#s▒▒▒j▒▒▒▒▒·▒p▒!ߝ▒▒�,▒8▒▒pw@   ▒▒~▒▒D▒Y▒{`▒H▒T3\;▒x..▒▒▒m>▒5d▒▒▒▒#▒+▒xٷu�▒▒&&▒i_9r▒C▒6=Y▒I5▒▒)▒▒D▒▒
  2▒5A▒D▒▒:▒▒V▒▒Z▒"v▒@D▒▒▒▒▒▒▒P▒▒|L▒v▒▒▒▒ʗ4▒WƁ▒*▒Y"s▒j▒H▒/▒h{|▒▒▒*ʧ▒,S▒CB▒▒Aq▒%|▒▒
                                                                                  ▒▒L▒▒
▒▒▒▒▒RM▒0L&,▒A]▒HfA0▒P▒                                                                p▒▒▒▒▒9▒▒ׂ▒▒▒▒1ۙ▒˂▒O▒>▒▒▒0-h▒▒▒*՛,▒g1▒▒>▒m<Z▒.▒lWL▒Fi▒▒Q▒▒^DP▒▒E▒~7▒f▒▒Uڼ▒▒-▒▒#▒GY▒▒)
▒@1▒*▒`&▒▒▒|3▒▒▒ T▒@j▒▒▒M▒▒#
▒▒▒w▒▒D▒▒▒T ▒▒▒k
                .T▒?A▒▒?▒p▒▒t▒7▒▒6{▒<h%7▒b▒▒▒▒  ▒mJ▒tk▒▒▒▒;8▒▒9▒▒o"$▒H▒:▒b▒֤▒*=ÿ▒^ʬ▒▒b3Z▒*▒▒▒:▒▒~▒▒>▒▒S▒▒zF▒'Z▒▒▒r▒/▒▒C▒2p▒{Kv▒K-VۧX▒g:▒ ▒w▒f▒Q▒▒▒▒▒%;▒&▒▒C▒▒
pb=x▒▒▒▒▒▒}▒AAbd<▒▒▒ !▒▒▒▒▒▒-e>▒▒▒▒Q▒
▒▒a▒XPq▒▒▒n_'h▒▒▒▒▒`:O▒v▒▒˞^▒t▒▒▒?▒▒▒▒f^<-KJ▒_▒ӛc▒ܿ▒▒[▒ƊD▒3H▒-▒▒*▒ܞ▒q▒eq▒▒p<Tv▒▒5 0▒▒▒/▒z▒▒▒'#p▒▒▒l!▒▒▒2▒ӗ3(ŋ▒X▒0y▒▒{▒▒耇▒[▒đ▒▒t ▒▒▒#▒9▒▒▒M▒uKg▒▒▒%▒▒▒▒▒wÈa(▒▒Jز▒~#S▒ūџM▒▒vc▒N.G▒A'▒+▒▒f4▒▒3/7▒▒▒▒▒e▒όC
▒▒Ņ▒Pu▒▒▒d,▒x▒렢J;m=+▒▒▒h▒,U▒z▒▒▒O▒K@▒8 z▒▒~ޭ[mV▒%▒▒▒▒▒#▒#▒W▒G▒▒▒▒▒?▒▒Z▒#y▒;\q▒'▒+▒a▒▒9▒ͱlv▒▒M▒▒
▒JWŹ▒4▒ft▒$▒#▒l?▒ k#▒▒L▒
▒Qo▒HƝ▒▒`▒▒▒f"▒@@▒▒▒▒▒▒#&Op▒<6▒▒▒!▒X▒~ !▒~z▒▒\u~#▒h▒0sS▒b
        G▒^f▒▒▒nd19▒▒x▒Ǭ▒H=▒t▒▒o?Mwf▒@;▒▒▒▒▒▒Ѱ▒Qav▒]=8▒▒▒▒|ߕ,▒▒▒▒9?^▒a▒'▒▒▒▒9▒▒m▒▒▒5▒m\uG▒▒z▒▒▒▒.▒%▒GXm▒,H▒;:▒u87▒▒&▒.▒#έ▒▒R▒▒W▒l▒▒▒▒Y▒3O▒_w▒ԇ▒▒QdwŒB▒▒▒
▒▒)▒NN▒G▒S▒▒;▒>s▒▒▒▒▒*`�.ԁs79▒<▒]tC▒▒▒▒-▒▒▒O▒:X▒F9▒,▒lȢ▒֥▒▒X▒&▒t
▒▒▒▒▒▒$s7▒▒▒bz▒j▒▒▒p▒e,▒[mLZ▒▒=
▒
▒8a▒▒?▒▒4P▒▒a▒▒_▒;▒~W▒▒w▒▒
▒▒▒▒▒B▒ɡ;▒~▒▒   |▒▒▒#▒#▒▒_▒▒H▒j▒▒▒d-▒▒▒p6▒U▒&▒▒FLE'▒▒▒▒▒#▒▒6▒▒V▒&▒▒\Е4▒tQ▒▒2▒▒^▒▒N▒f%▒▒Q8"▒7▒9▒U▒y▒▒▒ݪ▒j▒9▒▒M▒▒,▒▒▒<s▒▒]Y▒qL▒O7▒*v▒4C▒▒j[6▒▒▒▒RZ▒▒t▒h<▒▒▒ez▒▒#g▒▒hq▒▒]▒X▒'8▒8▒9x▒▒`▒        m3▒뗲k▒9▒3▒P▒\▒▒ɾ▒ /▒}(▒,▒n▒A▒~▒▒▒▒g
▒▒4FS;▒w3▒▒#▒▒▒D▒6X▒&V             ▒SӐި▒m▒Â▒▒▒   W▒؏l▒▒,▒P▒▒!▒~m~▒%?▒mr▒▒]cۉ▒FN+r٦G▒9▒d▒9▒Д▒;9▒▒▒▒▒▒
in6▒e"▒▒▒Z▒0▒(Ts粑▒▒▒▒▒▒)▒c▒▒
▒▒RLH▒▒▒k▒▒▒▒▒"Q▒ʘH▒▒   ▒▒▒▒▒▒Jc▒▒0aD▒b▒=▒▒▒M▒▒2I▒ˬ▒▒▒▒▒▒%▒V▒▒1ޣ!▒▒lj/f▒▒!▒"▒hԉ▒*▒!ڇ▒W▒▒▒▒z▒\,▒i▒▒▒▒▒▒r▒▒▒|▒kO▒ ▒▒▒Bp▒O▒▒▒'|8▒ϭ8\▒▒▒*▒(▒▒]▒Z▒▒▒P▒▒▒▒(▒▒k▒]▒?u▒▒▒ ▒d3hM▒9▒摷'▒▒s▒`▒h▒;G▒'▒0▒ͥӒm▒▒%]▒ȩ▒▒▒▒梙Zq▒▒w▒▒
)▒ ▒i03▒G▒▒▒    ▒:▒G▒H򬲈̀▒▒▒y[é▒T▒$▒T▒4l▒▒
[▒▒1▒▒▒)G▒DO▒1▒|▒"j▒    ▒▒▒X▒▒▒3
ѧ▒▒~:&▒(▒▒^▒▒R▒"▒▒W▒ˣ~▒~~bi▒h$▒)/<PO4&▒j▒˨▒X
$O@]▒▒▒▒7(▒ut▒a:▒YG▒▒▒7a▒▒#
]lH▒GZ▒M▒]▒▒▒▒<H▒▒Ь]Knto▒Ow▒.WM"Y藨IxN▒tވ:m;r▒)▒▒▒t▒,;▒▒ib▒h▒=▒X(▒>▒v▒▒5v▒▒▒▒▒▒▒▒
                                                         ▒▒▒▒h▒&▒t▒V▒=qJ▒X
▒▒O3▒Ze▒P▒▒n▒X▒y▒▒l▒▒x^▒u▒8F▒rA▒▒Ӂ▒▒E▒
                                      ▒▒▒L▒▒▒▒*$▒▒
▒&▒6▒▒▒,dN▒:▒w: vC▒n+▒▒▒O▒?▒▒̉h▒▒▒}▒▒▒>▒▒▒2P▒8f▒▒a▒▒▒%q?▒▒v▒x▒▒D2▒▒▒▒(▒▒6▒@:▒>{Tz
pT{%5▒▒Y▒a
▒~7▒▒p▒Gϒ▒▒*$XjH        Xݥ      ▒c▒^▒/z▒▒▒tYrQT(▒▒3▒dsTaFp�▒▒t▒▒▒▒v▒▒▒jCA▒▒▒/▒▒▒▒ j▒▒▒I,▒lI_z▒▒g▒iB▒▒F▒9▒▒UoUf▒E▒>]▒XZ
              Fy▒ܡ$▒)C▒▒s▒YeN.▒▒▒▒_▒▒▒guߠ~▒{▒ɂ▒2f▒$▒▒▒~Y▒i▒q▒▒5{0+s#Y▒▒g;▒      2F<▒▒g;I▒4S▒▒0G▒8R▒▒Xj/^▒O
▒▒▒V?ܺ▒s[▒▒▒:▒▒%(▒▒g1Ԉ9<▒S=▒▒▒/▒▒e▒i▒f▒
▒ړ▒▒▒Mx▒/▒@Gη▒W▒g[п▒_▒K▒▒V▒▒
▒!▒▒8▒▒▒▒R▒Wߨ▒▒▒h▒'▒▒hT
                       ▒AGp㇃cT>ZH*2    ▒▒l$▒▒K▒b▒▒Ǹ▒-k*▒▒▒▒▒l ▒▒x▒'t▒▒(▒߇c9▒:▒

▒▒▒[F▒SGq▒ߘ▒▒▒▒\▒▒▒pP▒Ϯ▒/▒▒b▒p▒P▒▒▒N▒▒?▒" ▒)e0▒▒i9▒▒nL▒▒▒▒B▒f▒wO▒&▒x▒7k6폓f▒)▒  ▒*▒_Ҏ;▒▒}֥5▒?▒▒s▒؂)d▒▒▒,▒▒▒Rט\xa▒x灍6▒`h¨▒
                   &▒Bt▒U▒?+5▒▒>Z=▒▒%qs#▒▒*fD▒v!▒▒▒▒▒U▒:▒E3L▒u▒r▒&▒;▒o▒ ▒▒g▒d▒S_Bӌ▒y%▒8▒ǈ:▒n▒▒?▒j8▒▒yk▒▒"/▒R▒▒~$0bDWT▒▒▒!n4▒l/▒@Mgk▒▒▒o0▒▒▒[▒C▒tb▒W▒/▒▒▒▒▒ ϴ▒v▒U▒}g▒:Z▒▒0▒▒^\%▒^▒▒*▒$▒▒I{▒▒F▒▒5>#▒▒D▒~/&w▒N޽?▒▒▒%̑▒▒▒▒▒▒▒9▒▒8▒b(▒}▒▒3C;▒V▒▒F▒5,▒#▒▒a▒▒+w▒-▒[▒▒▒~▒U▒S-▒▒▒▒J▒▒▒▒+eQ▒▒;▒▒i▒T▒    :uy▒H▒▒zH▒▒▒▒▒?▒▒▒e`▒▒:▒u▒=▒Ab▒▒▒kd
▒J۱c▒OV▒▒▒▒&▒a  ▒~v▒`'8u▒ĽK▒*▒▒▒4Id▒▒R▒▒e▒▒▒\i▒Y▒R8▒▒Rq^▒▒▒7▒▒▒▒▒n▒\?s▒▒▒_?▒G6▒^sW
                                                                                  4▒    ▒▒▒▒▒s▒J▒N:^菫f▒▒7▒ƹ▒p▒MN▒X▒x0y▒#▒▒+StÙ▒▒▒a▒Eo▒▒▒▒l▒▒▒▒▒o▒▒▒.▒:2y▒▒}▒39x▒▒▒!"Di▒d▒▒▒8▒u:▒▒▒▒2▒▒▒4b▒.▒0MJ▒N@^▒i▒I\▒2▒`G▒^▒ݱhT▒▒
▒y▒▒▒▒▒▒c▒▒G▒I#8Bڡp
▒▒▒`7I▒^▒▒▒▒$h▒▒H!GCO▒▒▒;f▒}▒▒h▒Qp▒N▒▒^▒▒▒e▒▒▒~▒▒q▒9▒▒R▒▒PD|▒▒F▒>▒▒J▒▒W▒?▒rb▒Y▒▒kw@▒▒▒Cݢ3▒^▒r<▒>qs▒▒▒M緃▒▒▒Q▒
▒tHq▒▒2▒▒~ڠ▒▒p▒m▒▒ٴG▒▒▒▒U*
                         ޮ▒▒r"▒Ϻ▒▒t▒Ul▒ @▒ف▒▒UU▒▒s▒▒▒▒$▒0▒R▒▒▒▒▒▒▒▒#▒▒@▒
▒J[q▒▒▒V▒Y▒˹▒+"aH▒1A▒▒U Z▒▒i
                            ▒▒V▒pZ▒r!.
▒▒zܽSKI▒ϊ▒C▒@▒4▒*v,▒▒oK▒ ▒?L'[i!#S▒▒]▒▒r▒▒S"▒{▒׎▒▒m▒▒ ▒▒+▒!H>k0J▒▒X~/▒A'e▒▒▒:O▒[▒▒Ȇ▒     ZW▒PC▒▒\▒Yq▒▒▒▒▒̀)▒W▒C▒2t▒DQ"▒▒9▒▒▒UW▒O▒▒▒*▒▒▒▒m▒Y+Y▒
                                                                                                                                            ▒▒:-▒6j▒Z▒V▒▒▒o▒▒▒▒B▒X}▒▒l▒%▒q▒▒▒/q▒Ɋ传▒%▒▒▒▒sG▒!^8▒▒▒h▒,▒R▒▒▒▒▒ 0l`c▒4;R▒dϨ▒▒]!t▒{VG▒kH )▒݆▒5]▒▒▒m^▒P>▒&▒pG▒▒▒▒3▒▒▒B;▒xT▒▒}#▒E▒▒▒▒O
                                                                                  ▒1▒6-▒▒▒i܊▒eáZ▒▒&:b &X        ▒8▒▒▒ܸ▒͗▒▒ه▒▒iTb▒▒TF7▒n▒▒UB▒v▒▒▒▒▒Q▒FŚ▒y▒:▒▒=)$=▒%k6▒▒▒▒.yE▒Q▒}mOUԒ▒▒▒▒▒#!▒[_g25е▒S▒▒7▒▒5▒▒72\P▒
mdW▒xQf]▒9▒▒▒9I▒▒▒▒3▒U▒3▒,lΧ▒▒_;▒▒▒▒N▒ ▒▒cÁ_▒▒▒E)▒o▒{p[x▒b▒▒2
WQ▒g w▒▒▒▒▒▒́X▒h▒Ӳ
▒ń▒>▒+&y▒▒▒u▒▒▒▒▒▒2o▒▒9▒Y,A▒ڊ▒▒0▒~▒+ղ▒▒▒|`m▒FR▒8/▒▒<▒3▒Y▒▒▒▒▒▒▒7li&ʙ▒▒▒ʍ▒I▒▒▒a▒▒K▒▒▒r2▒▒-z@▒m▒_/▒[▒S▒q▒▒vۍ▒.▒▒▒A-S▒▒a
z"




 truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
▒A▒'.▒f▒<P▒X▒▒K▒q▒▒2▒▒P▒▒▒gq▒&#H^▒▒J▒ypi*▒RA▒▒▒lTq;▒빫5:▒oA▒▒▒▒▒@▒UqUY`▒▒Lq/▒>˩▒d&lk▒▒5▒n▒▒ɖZ▒%[▒[▒▒▒▒▒▒pa▒1▒▒3▒▒&▒-e▒q
▒▒ck▒V,R▒U▒▒H▒▒cR▒▒)]▒uq▒▒▒:Y▒▒
▒▒|n!▒▒▒`M▒▒▒▒6▒FM▒1▒)▒▒▒^>▒1▒
▒h▒%▒!t▒▒▒iv8!=▒8▒#ٵ0▒;D▒fBBB▒▒4T~▒▒F▒Vj▒▒▒
                                           *2s▒<|5▒^$a?▒뾟E▒▒▒Ư"▒▒▒▒{▒:▒v▒▒i▒▒▒V▒▒ֺq▒wr▒▒▒0w▒fQ▒▒▒g&=▒▒  ▒▒g▒▒B▒u
                                                                                                                ▒▒$▒W▒瑽UVK
&zv▒~$▒▒5i▒▒^х▒h}~▒(S▒▒2D▒_m▒qt▒▒ж▒▒ٞޒ▒˨F▒▒J8м]▒}▒c▒▒r$▒,FAl▒▒▒▒▒▒$Z▒▒▒▒-▒i0R▒▒▒▒▒▒T▒▒▒-x▒▒▒▒{Er4▒-▒H▒▒Z>▒{▒▒▒5M_8▒,@▒▒▒
▒▒]I▒▒▒JI;s▒F▒j▒▒\▒▒/▒RcJ h▒▒▒▒ߧI
       ▒[PkQ4▒▒bG▒▒u▒t؃▒'r▒▒.?▒0􌼊▒&▒+
@0$▒T▒▒▒2t▒ZVD▒▒▒▒▒\▒Lդ▒r▒▒y8s#▒▒$f▒P/▒WA▒Ӊ▒D>▒8("Ym▒D,.▒▒▒+~▒Ā▒m▒1i▒▒HS▒▒
▒e▒▒0̳W7▒3C▒؇▒▒۳▒▒▒ǻ▒^f▒y▒▒▒h`?Y>▒Q
▒▒HPw▒hʳ,▒▒Y"▒▒VkcO▒Y▒J▒▒Ŏ▒▒ղ▒▒+▒6▒▒▒Z▒9▒▒^▒▒3▒u▒%▒]@l▒▒X▒▒짠▒ZI▒▒~▒▒▒*F-^ip▒-▒▒K▒▒KV▒▒*▒▒zr@͖ s(▒▒`▒8 $▒▒▒▒v▒▒tI`▒r?|2y3▒ݢ:Bp▒▒▒!▒O▒4▒\:▒▒ӖƓ▒H▒▒
                                                                                                      ▒▒▒T▒▒▒▒▒X▒0▒▒$)H▒r▒▒▒▒▒W▒E&▒▒u▒7▒▒▒v▒▒
c▒▒▒▒O▒*t[z▒V▒▒▒|▒$1▒▒!▒▒▒1▒#QmF▒~?/U_▒>▒m▒▒{d2~▒▒▒▒g▒▒▒l[▒Z▒▒▒▒▒▒W▒▒QT▒▒▒jEF▒  ▒▒▒▒F▒j
we▒▒▒Dљ▒▒o▒▒▒̭EL▒d▒W▒▒WW▒X▒▒F▒▒K▒▒6x"1oq▒|y▒▒S▒wh▒▒EȐ5▒▒▒▒▒z▒r▒▒`K▒▒z▒▒ǷK8P77f+▒▒]BL▒▒▒x▒t▒O▒▒]hޅss4▒▒▒V▒▒:▒v[y▒mU▒٢qj▒▒Sǅd▒ˢ;▒<K
▒▒O:▒#a▒r▒&q▒▒▒▒\▒▒97a                                 Z(b▒▒Z▒▒̙▒▒5▒▒
                      ▒)Ѭ▒▒lqћ  /▒
▒▒▒▒▒▒T=J▒2>▒▒Rh▒▒▒4ͨ▒▒▒*▒ϥ▒
XU▒▒r8▒▒▒▒Z▒▒8r▒▒▒ԕs
뜕▒C▒Ղ▒▒▒6▒u]誀^
                8▒/▒@?▒<▒1▒▒▒▒,▒▒Z'`:▒&▒9
▒Lh▒ǐc▒Ӟ▒((97▒▒L>▒
9
kʞf
   ▒▒▒<▒/▒J▒▒▒rg▒qG▒`M▒#c▒c▒▒▒▒▒o▒'▒▒▒~~▒▒l▒5▒|▒▒p4▒
hꨁ▒r▒15▒@$~▒▒▒▒P@'▒▒ا▒I▒Q
                         x>▒▒b▒E▒<▒▒▒>▒ !▒▒oC▒Wκ▒▒▒r"▒▒}▒▒▒▒8}\w▒▒7Z▒a▒▒^▒Me▒i"
                                                                               ▒けt▒▒KH▒▒@▒*▒xk▒▒۶^ňFԻ/8▒▒▒M▒▒k▒▒dv▒▒K▒▒Z▒b*▒
                                                                                                                             W#▒!▒8▒▒▒▒@Qv▒s▒P▒▒47M<}▒▒W@H▒6▒^▒▒▒&~Zd▒▒q.▒▒x▒з▒▒▒ѝ▒ѵ▒▒zڡ▒▒▒▒~ɠZP▒▒T1Sh+b▒Ί▒▒D▒▒>▒'▒8E▒▒▒$f▒t6▒▒�▒W▒▒▒▒#▒▒[x▒g▒Vk▒Rŕ|v{▒@mθ▒▒▒▒U▒▒8a?E▒
▒&▒▒▒▒vú▒▒▒y▒d▒p▒x▒fój▒▒▒▒▒x▒a|▒▒▒(▒▒P▒G▒-+!▒Յ▒|▒▒7▒N▒▒Z▒▒▒▒W▒▒=_▒w▒~▒v%▒▒▒▒a▒A(▒▒3M▒▒▒@0▒▒A▒▒D▒▒VS▒Z▒▒;3▒x▒B▒▒)&q▒<▒G▒▒▒▒F▒▒▒▒▒<▒▒▒X^B▒Iv▒q▒▒t▒vU▒▒▒▒:▒ۓva▒▒Mi▒;s[▒▒▒z▒#m^▒7▒▒k▒QJi▒W▒▒▒▒+vex1]▒▒Y(Zs▒▒Cl/(;T"g▒
                    &o▒,▒▒▒▒(▒▒R>▒#'?▒▒▒▒▒▒S[▒▒▒q3Z▒▒▒S▒P$▒▒ʾ▒▒▒        !▒{4x   ▒Q▒ʹ▒▒▒=▒"?A▒}▒}▒O▒r▒▒▒"▒▒E%▒Z▒▒▒
]Bb▒▒E(▒▒l▒▒▒=▒jL▒Q▒▒Ѭ▒▒▒wc▒▒ym▒▒xF¦▒G▒c+|ŶU▒▒▒Я"▒▒▒Y▒▒▒
▒▒%▒▒▒
>>> len("truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk")
32
>>>
```

bandit10::truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk



Bandit Level 10 → Level 11

Level Goal

The password for the next level is stored in the file data.txt, which contains base64 encoded data


Solution :

```
bandit10@bandit:~$ ls
data.txt
bandit10@bandit:~$ cat data.txt  | base64 -d
The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
```

bandit11::IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
