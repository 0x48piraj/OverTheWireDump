
## Leviathan

> **Dare you face the lord of the oceans?**

Leviathan is a wargame that has been rescued from the demise of intruded.net, previously hosted on leviathan.intruded.net. Big thanks to adc, morla and reth for their help in resurrecting this game!


What follows below is the original description of leviathan, copied from intruded.net:

```
Summary:
Difficulty:     1/10
Levels:         8
Platform:   Linux/x86
```

Author:
Anders Tonfeldt

Special Thanks:
We would like to thank AstroMonk for coming up with a replacement idea for the last level,
deadfood for finding a leveljump and Coi for finding a non-planned vulnerability.

Description:

This wargame doesn't require any knowledge about programming - just a bit of common
sense and some knowledge about basic *nix commands. We had no idea that it'd be this
hard to make an interesting wargame that wouldn't require programming abilities from 
the players. Hopefully we made an interesting challenge for the new ones.
Leviathan’s levels are called leviathan0, leviathan1, … etc. and can be accessed on leviathan.labs.overthewire.org through SSH on port 2223.

---



### Leviathan Level 0

#### Level Goal

To login to the first level use:
```
Username: leviathan0
Password: leviathan0
```

Data for the levels can be found in the homedirectories. You can look at /etc/leviathan_pass for the various level passwords.

Solution :


```
leviathan0@leviathan:~$ ls -la
total 24
drwxr-xr-x  3 root       root       4096 Oct 29 21:17 .
drwxr-xr-x 10 root       root       4096 Oct 29 21:17 ..
drwxr-x---  2 leviathan1 leviathan0 4096 Oct 29 21:17 .backup
-rw-r--r--  1 root       root        220 May 15  2017 .bash_logout
-rw-r--r--  1 root       root       3526 May 15  2017 .bashrc
-rw-r--r--  1 root       root        675 May 15  2017 .profile
leviathan0@leviathan:~$ cd .backup
leviathan0@leviathan:~/.backup$ ls
bookmarks.html
leviathan0@leviathan:~/.backup$ cat bookmarks.html | grep "password"
<DT><A HREF="http://leviathan.labs.overthewire.org/passwordus.html | This will be fixed later, the password for leviathan1 is rioGegei8m" ADD_DATE="1155384634" LAST_CHARSET="ISO-8859-1" ID="rdf:#$2wIU71">password to leviathan1</A>
leviathan0@leviathan:~/.backup$
```

Credential : `leviathan1:rioGegei8m`

## Leviathan Level 1

#### Level Goal

> There is no information for this level, intentionally.


Solution :

```
leviathan1@leviathan:~$ ltrace ./check
__libc_start_main(0x804853b, 1, 0xffffd794, 0x8048610 <unfinished ...>
printf("password: ")                                                                                                 = 10
getchar(1, 0, 0x65766f6c, 0x646f6700password: test
)                                                                                = 116
getchar(1, 0, 0x65766f6c, 0x646f6700)                                                                                = 101
getchar(1, 0, 0x65766f6c, 0x646f6700)                                                                                = 115
strcmp("tes", "sex")                                                                                                 = 1
puts("Wrong password, Good Bye ..."Wrong password, Good Bye ...
)                                                                                 = 29
+++ exited (status 0) +++
$ cd /etc/leviathan_pass
$ ls
leviathan0  leviathan1  leviathan2  leviathan3  leviathan4  leviathan5  leviathan6  leviathan7
$ cat *
cat: leviathan0: Permission denied
cat: leviathan1: Permission denied
ougahZi8Ta
cat: leviathan3: Permission denied
cat: leviathan4: Permission denied
cat: leviathan5: Permission denied
cat: leviathan6: Permission denied
cat: leviathan7: Permission denied
$

```
Credential : `leviathan2:ougahZi8Ta`


## Leviathan Level 2 → Level 3

#### Level Goal

> There is no information for this level, intentionally.

Solution :

```
leviathan2@leviathan:~$ ltrace ./printfile /etc/leviathan_pass/leviathan2
__libc_start_main(0x804852b, 2, 0xffffd764, 0x8048610 <unfinished ...>
access("/etc/leviathan_pass/leviathan2", 4)                                                                          = 0
snprintf("/bin/cat /etc/leviathan_pass/lev"..., 511, "/bin/cat %s", "/etc/leviathan_pass/leviathan2")                = 39
geteuid()                                                                                                            = 12002
geteuid()                                                                                                            = 12002
setreuid(12002, 12002)                                                                                               = 0
system("/bin/cat /etc/leviathan_pass/lev"...ougahZi8Ta
 <no return ...>
--- SIGCHLD (Child exited) ---
<... system resumed> )                                                                                               = 0
+++ exited (status 0) +++
leviathan2@leviathan:~$ ltrace ./printfile /etc/leviathan_pass/leviathan3
__libc_start_main(0x804852b, 2, 0xffffd764, 0x8048610 <unfinished ...>
access("/etc/leviathan_pass/leviathan3", 4)                                                                          = -1
puts("You cant have that file..."You cant have that file...
)                                                                                   = 27
+++ exited (status 1) +++
leviathan2@leviathan:~$ mkdir /tmp/0x48piraj/ && cd /tmp/0x48piraj/
leviathan2@leviathan:/tmp/0x48piraj$ ln -s /etc/leviathan_pass/leviathan3 givemepass
leviathan2@leviathan:/tmp/0x48piraj$ echo "" > "idk givemepass"
leviathan2@leviathan:/tmp/0x48piraj$ /home/leviathan2/printfile "/tmp/0x48piraj/idk givemepass"
/bin/cat: /tmp/0x48piraj/idk: No such file or directory
Ahdiemoo1j
leviathan2@leviathan:/tmp/0x48piraj$
```

Credential : `leviathan3:Ahdiemoo1j`


## Leviathan Level 3 → Level 4

#### Level Goal

> There is no information for this level, intentionally.

```
leviathan3@leviathan:~$ ls
level3
leviathan3@leviathan:~$ ./level3
Enter the password> idk
bzzzzzzzzap. WRONG
leviathan3@leviathan:~$ ltrace ./level3
__libc_start_main(0x8048618, 1, 0xffffd794, 0x80486d0 <unfinished ...>
strcmp("h0no33", "kakaka")                                                                                           = -1
printf("Enter the password> ")                                                                                       = 20
fgets(Enter the password> idk
"idk\n", 256, 0xf7fc55a0)                                                                                      = 0xffffd5a0
strcmp("idk\n", "snlprintf\n")                                                                                       = -1
puts("bzzzzzzzzap. WRONG"bzzzzzzzzap. WRONG
)                                                                                           = 19
+++ exited (status 0) +++
leviathan3@leviathan:~$ ./level3
Enter the password> snlprintf
[You've got shell]!
$ whoami
leviathan4
$ cat /etc/leviathan_pass/leviathan4
vuH0coox6m
$
```
Credential : `leviathan4:vuH0coox6m`

```
leviathan4@leviathan:~$ ls -la
total 24
drwxr-xr-x  3 root root       4096 Oct 29 21:17 .
drwxr-xr-x 10 root root       4096 Oct 29 21:17 ..
-rw-r--r--  1 root root        220 May 15  2017 .bash_logout
-rw-r--r--  1 root root       3526 May 15  2017 .bashrc
-rw-r--r--  1 root root        675 May 15  2017 .profile
dr-xr-x---  2 root leviathan4 4096 Oct 29 21:17 .trash
leviathan4@leviathan:~$ cd .trash
leviathan4@leviathan:~/.trash$ ls -la
total 16
dr-xr-x--- 2 root       leviathan4 4096 Oct 29 21:17 .
drwxr-xr-x 3 root       root       4096 Oct 29 21:17 ..
-r-sr-x--- 1 leviathan5 leviathan4 7352 Oct 29 21:17 bin
leviathan4@leviathan:~/.trash$ ./bin
01010100 01101001 01110100 01101000 00110100 01100011 01101111 01101011 01100101 01101001 00001010
leviathan4@leviathan:~/.trash$ python
Python 2.7.13 (default, Sep 26 2018, 18:42:22)
[GCC 6.3.0 20170516] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> import binascii
>>> cipher="01010100 01101001 01110100 01101000 00110100 01100011 01101111 01101011 01100101 01101001 00001010".replace(" ", "")
>>> binascii.unhexlify('%x' % int(cipher, 2))
'Tith4cokei\n'
>>>
```

Credential : `leviathan5:Tith4cokei`


```
leviathan5@leviathan:~$ echo "0x48piraj" > /tmp/file.log
leviathan5@leviathan:~$ ltrace ./leviathan5
__libc_start_main(0x80485db, 1, 0xffffd794, 0x80486a0 <unfinished ...>
fopen("/tmp/file.log", "r")                                                                                          = 0x804b008
fgetc(0x804b008)                                                                                                     = '0'
feof(0x804b008)                                                                                                      = 0
putchar(48, 0x8048720, 0xf7e40890, 0x80486eb)                                                                        = 48
fgetc(0x804b008)                                                                                                     = 'x'
feof(0x804b008)                                                                                                      = 0
putchar(120, 0x8048720, 0xf7e40890, 0x80486eb)                                                                       = 120
fgetc(0x804b008)                                                                                                     = '4'
feof(0x804b008)                                                                                                      = 0
putchar(52, 0x8048720, 0xf7e40890, 0x80486eb)                                                                        = 52
fgetc(0x804b008)                                                                                                     = '8'
feof(0x804b008)                                                                                                      = 0
putchar(56, 0x8048720, 0xf7e40890, 0x80486eb)                                                                        = 56
fgetc(0x804b008)                                                                                                     = 'p'
feof(0x804b008)                                                                                                      = 0
putchar(112, 0x8048720, 0xf7e40890, 0x80486eb)                                                                       = 112
fgetc(0x804b008)                                                                                                     = 'i'
feof(0x804b008)                                                                                                      = 0
putchar(105, 0x8048720, 0xf7e40890, 0x80486eb)                                                                       = 105
fgetc(0x804b008)                                                                                                     = 'r'
feof(0x804b008)                                                                                                      = 0
putchar(114, 0x8048720, 0xf7e40890, 0x80486eb)                                                                       = 114
fgetc(0x804b008)                                                                                                     = 'a'
feof(0x804b008)                                                                                                      = 0
putchar(97, 0x8048720, 0xf7e40890, 0x80486eb)                                                                        = 97
fgetc(0x804b008)                                                                                                     = 'j'
feof(0x804b008)                                                                                                      = 0
putchar(106, 0x8048720, 0xf7e40890, 0x80486eb)                                                                       = 106
fgetc(0x804b008)                                                                                                     = '\n'
feof(0x804b008)                                                                                                      = 0
putchar(10, 0x8048720, 0xf7e40890, 0x80486eb0x48piraj
)                                                                        = 10
fgetc(0x804b008)                                                                                                     = '\377'
feof(0x804b008)                                                                                                      = 1
fclose(0x804b008)                                                                                                    = 0
getuid()                                                                                                             = 12005
setuid(12005)                                                                                                        = 0
unlink("/tmp/file.log")                                                                                              = 0
+++ exited (status 0) +++
leviathan5@leviathan:~$ ln -s /etc/leviathan_pass/leviathan6 /tmp/file.log
leviathan5@leviathan:~$ ./leviathan5
UgaoFee4li
leviathan5@leviathan:~$
```
Credential : leviathan6:UgaoFee4li

