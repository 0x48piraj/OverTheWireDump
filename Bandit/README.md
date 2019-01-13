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
