
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


