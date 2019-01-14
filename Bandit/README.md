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

Bandit Level 11 → Level 12

Level Goal

The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

Solution :
```
bandit11@bandit:~$ ls
data.txt
bandit11@bandit:~$ cat data.txt
Gur cnffjbeq vf 5Gr8L4qetPEsPk8htqjhRK8XSP6x2RHh
bandit11@bandit:~$  cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
bandit11@bandit:~$
```

bandit12::5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu


Bandit Level 12 → Level 13

Level Goal

The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

I left a classic msg, like all hackers leave. Other than this, I found `sshkey`

```
bandit12@bandit:~$ cat data.txt
00000000: 1f8b 0808 d7d2 c55b 0203 6461 7461 322e  .......[..data2.
00000010: 6269 6e00 013c 02c3 fd42 5a68 3931 4159  bin..<...BZh91AY
00000020: 2653 591d aae5 9800 001b ffff de7f 7fff  &SY.............
00000030: bfb7 dfcf 9fff febf f5ad efbf bbdf 7fdb  ................
00000040: f2fd ffdf effa 7fff fbd7 bdff b001 398c  ..............9.
00000050: 1006 8000 0000 0d06 9900 0000 6834 000d  ............h4..
00000060: 01a1 a000 007a 8000 0d00 0006 9a00 d034  .....z.........4
00000070: 0d1a 3234 68d1 e536 a6d4 4000 341a 6200  ..24h..6..@.4.b.
00000080: 0069 a000 0000 0000 d003 d200 681a 0d00  .i..........h...
00000090: 0001 b51a 1a0c 201e a000 6d46 8068 069a  ...... ...mF.h..
000000a0: 6834 340c a7a8 3406 4000 0680 0001 ea06  h44...4.@.......
000000b0: 8190 03f5 4032 1a00 0343 4068 0000 0686  ....@2...C@h....
000000c0: 8000 0320 00d0 0d00 0610 0014 1844 0308  ... .........D..
000000d0: 04e1 c542 9ab8 2c30 f1be 0b93 763b fb13  ...B..,0....v;..
000000e0: 50c4 c101 e008 3b7a 92a7 9eba 8a73 8d21  P.....;z.....s.!
000000f0: 9219 9c17 052b fb66 a2c2 fccc 9719 b330  .....+.f.......0
00000100: 6068 8c65 e504 5ec0 ae02 fa6d 16bc 904b  `h.e..^....m...K
00000110: ba6c f692 356e c02b 0374 c394 6859 f5bb  .l..5n.+.t..hY..
00000120: 0f9f 528e 4272 22bb 103c 2848 d8aa 2409  ..R.Br"..<(H..$.
00000130: 24d0 d4c8 4b42 7388 ce25 6c1a 7ec1 5f17  $...KBs..%l.~._.
00000140: cc18 ddbf edc1 e3a4 67f1 7a4d 8277 c823  ........g.zM.w.#
00000150: 0450 2232 40e0 07f1 ca16 c6d6 ef0d ecc9  .P"2@...........
00000160: 8bc0 5e2d 4b12 8586 088e 8ca0 e67d a55c  ..^-K........}.\
00000170: 2ca0 18c7 bfb7 7d45 9346 ea5f 2172 01e4  ,.....}E.F._!r..
00000180: 5598 673f 45af 69b7 a739 7814 8706 04ed  U.g?E.i..9x.....
00000190: 5442 1240 0796 6cc8 b2f6 1ef9 8d13 421d  TB.@..l.......B.
000001a0: 461f 2e68 4d91 5343 34b5 56e7 46d0 0a0a  F..hM.SC4.V.F...
000001b0: 72b7 d873 71d9 6f09 c326 402d dbc0 7cef  r..sq.o..&@-..|.
000001c0: 53b1 df60 9ec7 f318 00df 3907 2e85 d85b  S..`......9....[
000001d0: 6a1a e105 0207 c580 e31d 82d5 8646 183c  j............F.<
000001e0: 6a04 4911 101a 5427 087c 1f94 47a2 270d  j.I...T'.|..G.'.
000001f0: ad12 fc5c 9ad2 5714 514f 34ba 701d fb69  ...\..W.QO4.p..i
00000200: 8eed 0183 e2a1 53ea 2300 26bb bd2f 13df  ......S.#.&../..
00000210: b703 08a3 2309 e43c 44bf 75d4 905e 5f96  ....#..<D.u..^_.
00000220: 481b 362e e82d 9093 7741 740c e65b c7f1  H.6..-..wAt..[..
00000230: 5550 f247 9043 5097 d626 3a16 da32 c213  UP.G.CP..&:..2..
00000240: 2acd 298a 5c8a f0c1 b99f e2ee 48a7 0a12  *.).\.......H...
00000250: 03b5 5cb3 0037 cece 773c 0200 00         ..\..7..w<...
bandit12@bandit:~$ file data.txt
data.txt: ASCII text
bandit12@bandit:~$ mkdir /tmp/myname123
mkdir: cannot create directory ‘/tmp/myname123’: File exists
bandit12@bandit:~$ cd /tmp/myname123
t12@bandit:/tmp/myname123$ ls
0x48piraj.was.here  data5.bin      data7  datacarlesreverse.gz   datacarles.txt  data.txt   file2  newdata    sshkey
a                   data6.bin.out  data9  datacarlesreverse.txt  data.out        file1.out  file3  revhex.gz  tmp
bandit12@bandit:/tmp/myname123$ cat sshkey
-----BEGIN RSA PRIVATE KEY-----
MIIEogIBAAKCAQEAvmOkuifmMg6HL2YPIOjon6iWfbp7c3jx34YkYWqUH57SUdyJ
imZzeyGC0gtZPGujUSxiJSWI/oTqexh+cAMTSMlOJf7+BrJObArnxd9Y7YT2bRPQ
Ja6Lzb558YW3FZl87ORiO+rW4LCDCNd2lUvLE/GL2GWyuKN0K5iCd5TbtJzEkQTu
DSt2mcNn4rhAL+JFr56o4T6z8WWAW18BR6yGrMq7Q/kALHYW3OekePQAzL0VUYbW
JGTi65CxbCnzc/w4+mqQyvmzpWtMAzJTzAzQxNbkR2MBGySxDLrjg0LWN6sK7wNX
x0YVztz/zbIkPjfkU1jHS+9EbVNj+D1XFOJuaQIDAQABAoIBABagpxpM1aoLWfvD
KHcj10nqcoBc4oE11aFYQwik7xfW+24pRNuDE6SFthOar69jp5RlLwD1NhPx3iBl
J9nOM8OJ0VToum43UOS8YxF8WwhXriYGnc1sskbwpXOUDc9uX4+UESzH22P29ovd
d8WErY0gPxun8pbJLmxkAtWNhpMvfe0050vk9TL5wqbu9AlbssgTcCXkMQnPw9nC
YNN6DDP2lbcBrvgT9YCNL6C+ZKufD52yOQ9qOkwFTEQpjtF4uNtJom+asvlpmS8A
vLY9r60wYSvmZhNqBUrj7lyCtXMIu1kkd4w7F77k+DjHoAXyxcUp1DGL51sOmama
+TOWWgECgYEA8JtPxP0GRJ+IQkX262jM3dEIkza8ky5moIwUqYdsx0NxHgRRhORT
8c8hAuRBb2G82so8vUHk/fur85OEfc9TncnCY2crpoqsghifKLxrLgtT+qDpfZnx
SatLdt8GfQ85yA7hnWWJ2MxF3NaeSDm75Lsm+tBbAiyc9P2jGRNtMSkCgYEAypHd
HCctNi/FwjulhttFx/rHYKhLidZDFYeiE/v45bN4yFm8x7R/b0iE7KaszX+Exdvt
SghaTdcG0Knyw1bpJVyusavPzpaJMjdJ6tcFhVAbAjm7enCIvGCSx+X3l5SiWg0A
R57hJglezIiVjv3aGwHwvlZvtszK6zV6oXFAu0ECgYAbjo46T4hyP5tJi93V5HDi
Ttiek7xRVxUl+iU7rWkGAXFpMLFteQEsRr7PJ/lemmEY5eTDAFMLy9FL2m9oQWCg
R8VdwSk8r9FGLS+9aKcV5PI/WEKlwgXinB3OhYimtiG2Cg5JCqIZFHxD6MjEGOiu
L8ktHMPvodBwNsSBULpG0QKBgBAplTfC1HOnWiMGOU3KPwYWt0O6CdTkmJOmL8Ni
blh9elyZ9FsGxsgtRBXRsqXuz7wtsQAgLHxbdLq/ZJQ7YfzOKU4ZxEnabvXnvWkU
YOdjHdSOoKvDQNWu6ucyLRAWFuISeXw9a/9p7ftpxm0TSgyvmfLF2MIAEwyzRqaM
77pBAoGAMmjmIJdjp+Ez8duyn3ieo36yrttF5NSsJLAbxFpdlc1gvtGCWW+9Cq0b
dxviW8+TFVEBl1O4f7HVm6EpTscdDxU+bCXWkfjuRb7Dy9GOtt9JPsX8MBTakzh3
vBgsyi/sN3RqRBcGU40fOoZyfAMT8s1m/uYv52O6IgeuZ/ujbjY=
-----END RSA PRIVATE KEY-----

```
Want to find out what I left? Go and find out! (Also check `/tmp/0x48piraj`)

Solution :

```
bandit12@bandit:/tmp/myname123$ mkdir /tmp/0x48piraj
bandit12@bandit:/tmp/myname123$ cp /home/bandit12/data.txt /tmp/0x48piraj
bandit12@bandit:/tmp/myname123$ cd /tmp/0x48piraj
bandit12@bandit:/tmp/0x48piraj$ ls
data.txt
bandit12@bandit:/tmp/0x48piraj$ xxd -r data.txt data.bin
bandit12@bandit:/tmp/0x48piraj$ file data.bin
data.bin: gzip compressed data, was "data2.bin", last modified: Tue Oct 16 12:00                                                                                                             :23 2018, max compression, from Unix

bandit12@bandit:/tmp/0x48piraj$ zcat data.bin | file -
/dev/stdin: bzip2 compressed data, block size = 900k
bandit12@bandit:/tmp/0x48piraj$ zcat data.bin | bzcat | file -
/dev/stdin: gzip compressed data, was "data4.bin", last modified: Tue Oct 16 12:00:23 2018, max compression, from Unix
bandit12@bandit:/tmp/0x48piraj$ zcat data.bin | bzcat | zcat | file -
/dev/stdin: POSIX tar archive (GNU)
bandit12@bandit:/tmp/0x48piraj$ zcat data.bin | bzcat | zcat | tar xO | file -
/dev/stdin: POSIX tar archive (GNU)
bandit12@bandit:/tmp/0x48piraj$ zcat data.bin | bzcat | zcat | tar xO | tar xO | file -
/dev/stdin: bzip2 compressed data, block size = 900k
bandit12@bandit:/tmp/0x48piraj$ zcat data.bin | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | zcat | file -
/dev/stdin: ASCII text
bandit12@bandit:/tmp/0x48piraj$ zcat data.bin | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | zcat
The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
bandit12@bandit:/tmp/0x48piraj$
```
Script for automation ? Not now.

bandit13::8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

Bandit Level 13 → Level 14

Level Goal

The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level.

Note: localhost is a hostname that refers to the machine you are working on


Solution :

```
bandit13@bandit:~$ ls
sshkey.private
bandit13@bandit:~$ cat sshkey.private
-----BEGIN RSA PRIVATE KEY-----
MIIEpAIBAAKCAQEAxkkOE83W2cOT7IWhFc9aPaaQmQDdgzuXCv+ppZHa++buSkN+
gg0tcr7Fw8NLGa5+Uzec2rEg0WmeevB13AIoYp0MZyETq46t+jk9puNwZwIt9XgB
ZufGtZEwWbFWw/vVLNwOXBe4UWStGRWzgPpEeSv5Tb1VjLZIBdGphTIK22Amz6Zb
ThMsiMnyJafEwJ/T8PQO3myS91vUHEuoOMAzoUID4kN0MEZ3+XahyK0HJVq68KsV
ObefXG1vvA3GAJ29kxJaqvRfgYnqZryWN7w3CHjNU4c/2Jkp+n8L0SnxaNA+WYA7
jiPyTF0is8uzMlYQ4l1Lzh/8/MpvhCQF8r22dwIDAQABAoIBAQC6dWBjhyEOzjeA
J3j/RWmap9M5zfJ/wb2bfidNpwbB8rsJ4sZIDZQ7XuIh4LfygoAQSS+bBw3RXvzE
pvJt3SmU8hIDuLsCjL1VnBY5pY7Bju8g8aR/3FyjyNAqx/TLfzlLYfOu7i9Jet67
xAh0tONG/u8FB5I3LAI2Vp6OviwvdWeC4nOxCthldpuPKNLA8rmMMVRTKQ+7T2VS
nXmwYckKUcUgzoVSpiNZaS0zUDypdpy2+tRH3MQa5kqN1YKjvF8RC47woOYCktsD
o3FFpGNFec9Taa3Msy+DfQQhHKZFKIL3bJDONtmrVvtYK40/yeU4aZ/HA2DQzwhe
ol1AfiEhAoGBAOnVjosBkm7sblK+n4IEwPxs8sOmhPnTDUy5WGrpSCrXOmsVIBUf
laL3ZGLx3xCIwtCnEucB9DvN2HZkupc/h6hTKUYLqXuyLD8njTrbRhLgbC9QrKrS
M1F2fSTxVqPtZDlDMwjNR04xHA/fKh8bXXyTMqOHNJTHHNhbh3McdURjAoGBANkU
1hqfnw7+aXncJ9bjysr1ZWbqOE5Nd8AFgfwaKuGTTVX2NsUQnCMWdOp+wFak40JH
PKWkJNdBG+ex0H9JNQsTK3X5PBMAS8AfX0GrKeuwKWA6erytVTqjOfLYcdp5+z9s
8DtVCxDuVsM+i4X8UqIGOlvGbtKEVokHPFXP1q/dAoGAcHg5YX7WEehCgCYTzpO+
xysX8ScM2qS6xuZ3MqUWAxUWkh7NGZvhe0sGy9iOdANzwKw7mUUFViaCMR/t54W1
GC83sOs3D7n5Mj8x3NdO8xFit7dT9a245TvaoYQ7KgmqpSg/ScKCw4c3eiLava+J
3btnJeSIU+8ZXq9XjPRpKwUCgYA7z6LiOQKxNeXH3qHXcnHok855maUj5fJNpPbY
iDkyZ8ySF8GlcFsky8Yw6fWCqfG3zDrohJ5l9JmEsBh7SadkwsZhvecQcS9t4vby
9/8X4jS0P8ibfcKS4nBP+dT81kkkg5Z5MohXBORA7VWx+ACohcDEkprsQ+w32xeD
qT1EvQKBgQDKm8ws2ByvSUVs9GjTilCajFqLJ0eVYzRPaY6f++Gv/UVfAPV4c+S0
kAWpXbv5tbkkzbS0eaLPTKgLzavXtQoTtKwrjpolHKIHUz6Wu+n4abfAIRFubOdN
/+aLoRQ0yBDRbdXMsZN/jvY44eM+xRLdRVyMmdPtP8belRi2E2aEzA==
-----END RSA PRIVATE KEY-----
bandit13@bandit:~$exit
```
ON MY SYSTEM :

```
$ chmod 600 privkey.txt
$ ssh -i privkey.txt bandit14@bandit.labs.overthewire.org -p 2220
```
#### Wait! What? What the ..

##### LOGGED TIME : `Sun Jan 13 20:19:24 2019`

```
Enjoy your stay!

bandit14@bandit:~$ 

bandit14@bandit:~$ ls

Broadcast message from root@bandit (pts/24) (Sun Jan 13 20:19:24 2019):        
                                                                               

sorry, smal reboot coming up.                                                  

no time no time letz do some crime                                             

happy whatever day it is                                                       

cheers                                                                         

morla                                                                          
                                                                             


Broadcast message from root@bandit (pts/24) (Sun Jan 13 20:20:18 2019):
The system is going DOWN for reboot in 10 minutes!

Broadcast message from root@bandit (pts/24) (Sun Jan 13 20:21:18 2019):
The system is going DOWN for reboot in 9 minutes!

Broadcast message from root@bandit (pts/24) (Sun Jan 13 20:22:18 2019):
The system is going DOWN for reboot in 8 minutes!

Broadcast message from root@bandit (pts/24) (Sun Jan 13 20:23:18 2019):
The system is going DOWN for reboot in 7 minutes!

ls -la

total 24

drwxr-xr-x  3 root root 4096 Oct 16 14:00 .

drwxr-xr-x 41 root root 4096 Oct 16 14:00 ..

-rw-r--r--  1 root root  220 May 15  2017 .bash_logout

-rw-r--r--  1 root root 3526 May 15  2017 .bashrc

-rw-r--r--  1 root root  675 May 15  2017 .profile

drwxr-xr-x  2 root root 4096 Oct 16 14:00 .ssh

bandit14@bandit:~$ 

Broadcast message from root@bandit (pts/24) (Sun Jan 13 20:24:18 2019):
The system is going DOWN for reboot in 6 minutes!

Broadcast message from root@bandit (pts/24) (Sun Jan 13 20:25:18 2019):
The system is going DOWN for reboot in 5 minutes!

Broadcast message from root@bandit (pts/24) (Sun Jan 13 20:26:18 2019):
The system is going DOWN for reboot in 4 minutes!

Broadcast message from root@bandit (pts/24) (Sun Jan 13 20:27:18 2019):
The system is going DOWN for reboot in 3 minutes!

Broadcast message from root@bandit (pts/24) (Sun Jan 13 20:28:18 2019):
The system is going DOWN for reboot in 2 minutes!

Broadcast message from root@bandit (pts/24) (Sun Jan 13 20:29:18 2019):
The system is going DOWN for reboot in 1 minute!

Broadcast message from root@bandit (pts/24) (Sun Jan 13 20:30:18 2019):

The system is going down for reboot NOW!
Connection to bandit.labs.overthewire.org closed by remote host.
Connection to bandit.labs.overthewire.org closed.


```
Googled and found https://superuser.com/questions/624493/corrupted-broadcast-message-when-system-is-going-to-halt-in-debian
```
bandit14@bandit:~$ stty --all
speed 38400 baud; rows 58; columns 210; line = 0;
intr = ^C; quit = ^\; erase = ^?; kill = ^U; eof = ^D; eol = M-^?; eol2 = M-^?; swtch = <undef>; start = ^Q; stop = ^S; susp = ^Z; rprnt = ^R; werase = ^W; lnext = ^V; discard = ^O; min = 1; time = 0;
-parenb -parodd -cmspar cs8 -hupcl -cstopb cread -clocal -crtscts
-ignbrk -brkint -ignpar -parmrk -inpck -istrip -inlcr -igncr icrnl ixon -ixoff -iuclc ixany imaxbel iutf8
opost -olcuc -ocrnl onlcr -onocr -onlret -ofill -ofdel nl0 cr0 tab0 bs0 vt0 ff0
isig icanon iexten echo echoe echok -echonl -noflsh -xcase -tostop -echoprt echoctl echoke -flusho -extproc
bandit14@bandit:~$

```
See the tweet to know what may have happened : https://twitter.com/0x48piraj/status/1084539393342230528

Moving on..


Bandit Level 14 → Level 15

Level Goal

The password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhost.

Solution :

```
bandit14@bandit:~$ cat /etc/bandit_pass/bandit14
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
bandit14@bandit:~$ cat /etc/bandit_pass/bandit14 | nc localhost 30000
Correct!
BfMYroe26WYalil77FoDi9qh59eK5xNr
```

bandit15::BfMYroe26WYalil77FoDi9qh59eK5xNr


Bandit Level 15 → Level 16

Level Goal

The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL encryption.

Helpful note: Getting “HEARTBEATING” and “Read R BLOCK”? Use -ign_eof and read the “CONNECTED COMMANDS” section in the manpage. Next to ‘R’ and ‘Q’, the ‘B’ command also works in this version of that command…


Solution :

```
bandit15@bandit:~$ ls -la
total 24
drwxr-xr-x  2 root     root     4096 Jan 11 14:50 .
drwxr-xr-x 41 root     root     4096 Oct 16 14:00 ..
-rw-r-----  1 bandit15 bandit15   33 Jan 11 14:50 .bandit14.password
-rw-r--r--  1 root     root      220 May 15  2017 .bash_logout
-rw-r--r--  1 root     root     3526 May 15  2017 .bashrc
-rw-r--r--  1 root     root      675 May 15  2017 .profile
bandit15@bandit:~$ cat ./.bandit14.password
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
bandit15@bandit:~$ echo "4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e" | openssl s_client -connect localhost:30001 -ign_eof
CONNECTED(00000003)
depth=0 CN = localhost
verify error:num=18:self signed certificate
verify return:1
depth=0 CN = localhost
verify return:1
---
Certificate chain
 0 s:/CN=localhost
   i:/CN=localhost
---
Server certificate
-----BEGIN CERTIFICATE-----
MIICBjCCAW+gAwIBAgIENHv1njANBgkqhkiG9w0BAQUFADAUMRIwEAYDVQQDDAls
b2NhbGhvc3QwHhcNMTkwMTEzMTkzNDMwWhcNMjAwMTEzMTkzNDMwWjAUMRIwEAYD
VQQDDAlsb2NhbGhvc3QwgZ8wDQYJKoZIhvcNAQEBBQADgY0AMIGJAoGBALOkCuqD
hi2X8nQ1Fu/p2hHx+3SeORNWt76H7Q/Wr8ZYapwViACu7h/d+Gn1Z4/1ZVN5Ukz3
fiS7UiA73eJg2iLo9rXzPw01hVB+IA4RtSTBmsUm7vwIgNDv5RsrYLl6JCGaZ+ns
/z5ihBHILWT3zvLyAn98HUiVAjAahiuwBtHxAgMBAAGjZTBjMBQGA1UdEQQNMAuC
CWxvY2FsaG9zdDBLBglghkgBhvhCAQ0EPhY8QXV0b21hdGljYWxseSBnZW5lcmF0
ZWQgYnkgTmNhdC4gU2VlIGh0dHBzOi8vbm1hcC5vcmcvbmNhdC8uMA0GCSqGSIb3
DQEBBQUAA4GBABiUJgikW8Ig5kuqkB3VCZiACRm5bsC4T5EH531RtzDi6Yywnqm3
xDbfWzLIoWpVq2U2pViIVsPmQ6nGjASQSlQhxsg9kZBaqYB26AcgrmbVIruywtij
JXvZkb10yrXeqtfK5bO8+kILa8XSBVbIXQ55Cn4HiHE7NtDZBOLBTl2/
-----END CERTIFICATE-----
subject=/CN=localhost
issuer=/CN=localhost
---
No client certificate CA names sent
Peer signing digest: SHA512
Server Temp Key: X25519, 253 bits
---
SSL handshake has read 1019 bytes and written 269 bytes
Verification error: self signed certificate
---
New, TLSv1.2, Cipher is ECDHE-RSA-AES256-GCM-SHA384
Server public key is 1024 bit
Secure Renegotiation IS supported
Compression: NONE
Expansion: NONE
No ALPN negotiated
SSL-Session:
    Protocol  : TLSv1.2
    Cipher    : ECDHE-RSA-AES256-GCM-SHA384
    Session-ID: 990EEA60C329C272E5DB60F5D07150C928302ED6D7A73C6D61F76EC8CBE217B4
    Session-ID-ctx:
    Master-Key: 8B4E7E157CFFD696925B3E3C5BB64B927980622E6FEACC9CBC36146399CEE88CE86566EF41F0E7F251F926B9A2522D8C
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    TLS session ticket lifetime hint: 7200 (seconds)
    TLS session ticket:
    0000 - 32 a4 5b 29 4b c8 06 db-a5 7e c7 95 4f fd c4 c1   2.[)K....~..O...
    0010 - 55 74 96 eb 51 c5 51 aa-4c c6 07 45 69 67 73 f3   Ut..Q.Q.L..Eigs.
    0020 - 99 19 b3 ef 7a 77 ca ba-b3 32 e2 38 cc fd ce 27   ....zw...2.8...'
    0030 - fa 1b e1 ce a0 39 36 66-d2 7e ab f5 5d 08 4d 37   .....96f.~..].M7
    0040 - 67 bb ad b3 01 5c fb 1e-1c 4c 71 04 6d d8 a8 6c   g....\...Lq.m..l
    0050 - 71 be 7a 83 87 d7 1e b8-3a 21 5c a1 27 e1 cc 5e   q.z.....:!\.'..^
    0060 - 7a 59 25 fa 51 4b 29 dc-6c a3 31 22 27 0e 45 3e   zY%.QK).l.1"'.E>
    0070 - a7 e8 c2 0e 18 f0 f8 54-cb 8f 9a 24 6c 89 23 49   .......T...$l.#I
    0080 - b0 95 cc 00 f2 0c 2b d1-ef 16 33 82 88 2a 16 16   ......+...3..*..
    0090 - 40 cc 31 c7 2e f9 db 58-2c 02 f8 ff d5 39 0d 4f   @.1....X,....9.O

    Start Time: 1547411586
    Timeout   : 7200 (sec)
    Verify return code: 18 (self signed certificate)
    Extended master secret: yes
---
Wrong! Please enter the correct current password
closed
bandit15@bandit:~$ echo "BfMYroe26WYalil77FoDi9qh59eK5xNr" | openssl s_client -connect localhost:30001 -ign_eof
CONNECTED(00000003)
depth=0 CN = localhost
verify error:num=18:self signed certificate
verify return:1
depth=0 CN = localhost
verify return:1
---
Certificate chain
 0 s:/CN=localhost
   i:/CN=localhost
---
Server certificate
-----BEGIN CERTIFICATE-----
MIICBjCCAW+gAwIBAgIENHv1njANBgkqhkiG9w0BAQUFADAUMRIwEAYDVQQDDAls
b2NhbGhvc3QwHhcNMTkwMTEzMTkzNDMwWhcNMjAwMTEzMTkzNDMwWjAUMRIwEAYD
VQQDDAlsb2NhbGhvc3QwgZ8wDQYJKoZIhvcNAQEBBQADgY0AMIGJAoGBALOkCuqD
hi2X8nQ1Fu/p2hHx+3SeORNWt76H7Q/Wr8ZYapwViACu7h/d+Gn1Z4/1ZVN5Ukz3
fiS7UiA73eJg2iLo9rXzPw01hVB+IA4RtSTBmsUm7vwIgNDv5RsrYLl6JCGaZ+ns
/z5ihBHILWT3zvLyAn98HUiVAjAahiuwBtHxAgMBAAGjZTBjMBQGA1UdEQQNMAuC
CWxvY2FsaG9zdDBLBglghkgBhvhCAQ0EPhY8QXV0b21hdGljYWxseSBnZW5lcmF0
ZWQgYnkgTmNhdC4gU2VlIGh0dHBzOi8vbm1hcC5vcmcvbmNhdC8uMA0GCSqGSIb3
DQEBBQUAA4GBABiUJgikW8Ig5kuqkB3VCZiACRm5bsC4T5EH531RtzDi6Yywnqm3
xDbfWzLIoWpVq2U2pViIVsPmQ6nGjASQSlQhxsg9kZBaqYB26AcgrmbVIruywtij
JXvZkb10yrXeqtfK5bO8+kILa8XSBVbIXQ55Cn4HiHE7NtDZBOLBTl2/
-----END CERTIFICATE-----
subject=/CN=localhost
issuer=/CN=localhost
---
No client certificate CA names sent
Peer signing digest: SHA512
Server Temp Key: X25519, 253 bits
---
SSL handshake has read 1019 bytes and written 269 bytes
Verification error: self signed certificate
---
New, TLSv1.2, Cipher is ECDHE-RSA-AES256-GCM-SHA384
Server public key is 1024 bit
Secure Renegotiation IS supported
Compression: NONE
Expansion: NONE
No ALPN negotiated
SSL-Session:
    Protocol  : TLSv1.2
    Cipher    : ECDHE-RSA-AES256-GCM-SHA384
    Session-ID: FEFB0CD2836210ECEEF0C86C8D42E284CE0199A270287149512C4C61495311F4
    Session-ID-ctx:
    Master-Key: 1C4E006F6E4652778DC657007C305F4EA524F1CFA945A0C1D0E0D2AC3ABE1EF24A12BCD24CD4878037EDD24B7803F0C5
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    TLS session ticket lifetime hint: 7200 (seconds)
    TLS session ticket:
    0000 - 32 a4 5b 29 4b c8 06 db-a5 7e c7 95 4f fd c4 c1   2.[)K....~..O...
    0010 - 33 41 48 ad db 9a 4c 73-df f6 1b 81 15 b8 75 9e   3AH...Ls......u.
    0020 - c4 b7 ef e0 75 c8 32 e2-64 00 24 f6 da 4f 36 34   ....u.2.d.$..O64
    0030 - e1 20 91 1f 3d 42 95 c2-8a ec 08 cc d6 3d 12 c4   . ..=B.......=..
    0040 - 33 5d 99 47 dc 47 c3 cc-de 41 7a 66 8d f6 04 60   3].G.G...Azf...`
    0050 - 20 b1 ed 50 85 cd ef af-39 7d aa e2 bd bc 2b b8    ..P....9}....+.
    0060 - df 28 36 51 2f 1a 8a 3f-fa fb 49 67 7f b6 da 89   .(6Q/..?..Ig....
    0070 - 88 1a 2c 30 74 45 a5 9c-52 3a d7 47 b8 3b f9 47   ..,0tE..R:.G.;.G
    0080 - 53 7b c8 88 35 45 3b a0-7e 58 50 67 3f 6b 05 a6   S{..5E;.~XPg?k..
    0090 - 06 ef ab e0 3e 2c 81 bd-eb 69 c4 57 0d 3d b7 4c   ....>,...i.W.=.L

    Start Time: 1547411609
    Timeout   : 7200 (sec)
    Verify return code: 18 (self signed certificate)
    Extended master secret: yes
---
Correct!
cluFn7wTiGryunymYOu4RcffSxQluehd

```
bandit16::cluFn7wTiGryunymYOu4RcffSxQluehd

Bandit Level 16 → Level 17

Level Goal

The credentials for the next level can be retrieved by submitting the password of the current level to a port on localhost in the range 31000 to 32000. First find out which of these ports have a server listening on them. Then find out which of those speak SSL and which don’t. There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.


Solution :

```
bandit16@bandit:~$ cat ./.bandit15.password 
BfMYroe26WYalil77FoDi9qh59eK5xNr
bandit16@bandit:~$ nc -zv localhost  31000-32000
localhost [127.0.0.1] 31960 (?) open
localhost [127.0.0.1] 31790 (?) open
localhost [127.0.0.1] 31691 (?) open
localhost [127.0.0.1] 31518 (?) open
localhost [127.0.0.1] 31046 (?) open
bandit16@bandit:~$ echo "cluFn7wTiGryunymYOu4RcffSxQluehd" | openssl s_client -connect localhost:31790 -ign_eof
CONNECTED(00000003)
depth=0 CN = localhost
verify error:num=18:self signed certificate
verify return:1
depth=0 CN = localhost
verify return:1
---
Certificate chain
 0 s:/CN=localhost
   i:/CN=localhost
---
Server certificate
-----BEGIN CERTIFICATE-----
MIICBjCCAW+gAwIBAgIELHlSDDANBgkqhkiG9w0BAQUFADAUMRIwEAYDVQQDDAls
b2NhbGhvc3QwHhcNMTkwMTEzMTkzNDMwWhcNMjAwMTEzMTkzNDMwWjAUMRIwEAYD
VQQDDAlsb2NhbGhvc3QwgZ8wDQYJKoZIhvcNAQEBBQADgY0AMIGJAoGBAJ4UdWRN
ZmKD+47wp9PM6kCsCLM6u3WD1ByGlnJn3HeILlCxId2oaklGkOx/BzYcX8m0U+wU
XrC8/lC0o1YHfgfCaVht4ubhmrlD4iUnY7pABtIsrIdLgz/Ee54121GG2+ZZfmpq
mMytFoWyHSQUNFtavUMPYkzNCI8FO7GiLIZrAgMBAAGjZTBjMBQGA1UdEQQNMAuC
CWxvY2FsaG9zdDBLBglghkgBhvhCAQ0EPhY8QXV0b21hdGljYWxseSBnZW5lcmF0
ZWQgYnkgTmNhdC4gU2VlIGh0dHBzOi8vbm1hcC5vcmcvbmNhdC8uMA0GCSqGSIb3
DQEBBQUAA4GBAEtU/dx2IFDG7q3IcOmYkrvzHlmUKMXPiQqJgim/nzAo89is3A2B
S9+oWaaCX+Z5Hz97h7nJNFQHTjpoKKP0wS7ZqdpXFXFOVa4rD12hPEebqE/fCPiC
bOoJkI78ZtUg3fbal8XPHyQK4QcOfgfVAIjSgoUfiNJYQz+0Yqh6EMEp
-----END CERTIFICATE-----
subject=/CN=localhost
issuer=/CN=localhost
---
No client certificate CA names sent
Peer signing digest: SHA512
Server Temp Key: X25519, 253 bits
---
SSL handshake has read 1019 bytes and written 269 bytes
Verification error: self signed certificate
---
New, TLSv1.2, Cipher is ECDHE-RSA-AES256-GCM-SHA384
Server public key is 1024 bit
Secure Renegotiation IS supported
Compression: NONE
Expansion: NONE
No ALPN negotiated
SSL-Session:
    Protocol  : TLSv1.2
    Cipher    : ECDHE-RSA-AES256-GCM-SHA384
    Session-ID: 538FC81ECC2E3405870F6B3904468BBDF9639DDA0B31FE9F3BC147DFF0D97829
    Session-ID-ctx: 
    Master-Key: 9E21E97840227617B0033BF847D9638C34D0242EDE8836171FC84385E4A2C017255990A39C17073D78D9043F823E49FD
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    TLS session ticket lifetime hint: 7200 (seconds)
    TLS session ticket:
    0000 - fe 2e da f4 cd cd e9 23-46 73 02 6e ca e6 93 3a   .......#Fs.n...:
    0010 - 95 51 a8 7c ab 0b 88 1b-ac d1 63 fb bf d5 4d a7   .Q.|......c...M.
    0020 - c6 63 a5 47 d6 49 00 d1-7b 44 77 e6 26 11 76 cd   .c.G.I..{Dw.&.v.
    0030 - da 82 09 04 bb 80 e0 24-1c 8b ba e3 a5 fd cc a6   .......$........
    0040 - 82 f6 88 ba 82 75 c2 d2-2b 99 6f ab 76 3d 20 92   .....u..+.o.v= .
    0050 - ae 05 bb 57 12 16 a5 ee-3c e4 d5 e7 88 32 79 3a   ...W....<....2y:
    0060 - 76 37 ba da 28 b0 84 ba-f8 a9 1e 85 74 21 ae 28   v7..(.......t!.(
    0070 - 17 4b 6f d7 c8 5d 50 18-a5 65 5a 10 dd 39 9c f0   .Ko..]P..eZ..9..
    0080 - 2c 79 45 ba ae af 82 95-76 02 61 44 dd 19 94 75   ,yE.....v.aD...u
    0090 - fc 2d 04 e4 84 18 6c 96-75 1a 68 26 67 9c c4 d1   .-....l.u.h&g...

    Start Time: 1547480514
    Timeout   : 7200 (sec)
    Verify return code: 18 (self signed certificate)
    Extended master secret: yes
---
Correct!
-----BEGIN RSA PRIVATE KEY-----
MIIEogIBAAKCAQEAvmOkuifmMg6HL2YPIOjon6iWfbp7c3jx34YkYWqUH57SUdyJ
imZzeyGC0gtZPGujUSxiJSWI/oTqexh+cAMTSMlOJf7+BrJObArnxd9Y7YT2bRPQ
Ja6Lzb558YW3FZl87ORiO+rW4LCDCNd2lUvLE/GL2GWyuKN0K5iCd5TbtJzEkQTu
DSt2mcNn4rhAL+JFr56o4T6z8WWAW18BR6yGrMq7Q/kALHYW3OekePQAzL0VUYbW
JGTi65CxbCnzc/w4+mqQyvmzpWtMAzJTzAzQxNbkR2MBGySxDLrjg0LWN6sK7wNX
x0YVztz/zbIkPjfkU1jHS+9EbVNj+D1XFOJuaQIDAQABAoIBABagpxpM1aoLWfvD
KHcj10nqcoBc4oE11aFYQwik7xfW+24pRNuDE6SFthOar69jp5RlLwD1NhPx3iBl
J9nOM8OJ0VToum43UOS8YxF8WwhXriYGnc1sskbwpXOUDc9uX4+UESzH22P29ovd
d8WErY0gPxun8pbJLmxkAtWNhpMvfe0050vk9TL5wqbu9AlbssgTcCXkMQnPw9nC
YNN6DDP2lbcBrvgT9YCNL6C+ZKufD52yOQ9qOkwFTEQpjtF4uNtJom+asvlpmS8A
vLY9r60wYSvmZhNqBUrj7lyCtXMIu1kkd4w7F77k+DjHoAXyxcUp1DGL51sOmama
+TOWWgECgYEA8JtPxP0GRJ+IQkX262jM3dEIkza8ky5moIwUqYdsx0NxHgRRhORT
8c8hAuRBb2G82so8vUHk/fur85OEfc9TncnCY2crpoqsghifKLxrLgtT+qDpfZnx
SatLdt8GfQ85yA7hnWWJ2MxF3NaeSDm75Lsm+tBbAiyc9P2jGRNtMSkCgYEAypHd
HCctNi/FwjulhttFx/rHYKhLidZDFYeiE/v45bN4yFm8x7R/b0iE7KaszX+Exdvt
SghaTdcG0Knyw1bpJVyusavPzpaJMjdJ6tcFhVAbAjm7enCIvGCSx+X3l5SiWg0A
R57hJglezIiVjv3aGwHwvlZvtszK6zV6oXFAu0ECgYAbjo46T4hyP5tJi93V5HDi
Ttiek7xRVxUl+iU7rWkGAXFpMLFteQEsRr7PJ/lemmEY5eTDAFMLy9FL2m9oQWCg
R8VdwSk8r9FGLS+9aKcV5PI/WEKlwgXinB3OhYimtiG2Cg5JCqIZFHxD6MjEGOiu
L8ktHMPvodBwNsSBULpG0QKBgBAplTfC1HOnWiMGOU3KPwYWt0O6CdTkmJOmL8Ni
blh9elyZ9FsGxsgtRBXRsqXuz7wtsQAgLHxbdLq/ZJQ7YfzOKU4ZxEnabvXnvWkU
YOdjHdSOoKvDQNWu6ucyLRAWFuISeXw9a/9p7ftpxm0TSgyvmfLF2MIAEwyzRqaM
77pBAoGAMmjmIJdjp+Ez8duyn3ieo36yrttF5NSsJLAbxFpdlc1gvtGCWW+9Cq0b
dxviW8+TFVEBl1O4f7HVm6EpTscdDxU+bCXWkfjuRb7Dy9GOtt9JPsX8MBTakzh3
vBgsyi/sN3RqRBcGU40fOoZyfAMT8s1m/uYv52O6IgeuZ/ujbjY=
-----END RSA PRIVATE KEY-----

closed
bandit16@bandit:~$ exit

root@kali:~# chmod 600 rsa_lvl17.txt
root@kali:~# ssh -i rsa_lvl17.txt bandit17@bandit.labs.overthewire.org -p 2220
```

bandit17::RSA_PRIV_KEY
