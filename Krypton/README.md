## Krypton

> The Krypton wargame.

### Krypton Level 0 → Level 1

#### Level Info
> Uplink: http://overthewire.org/wargames/krypton/krypton0.html

Welcome to Krypton! The first level is easy. The following string encodes the password using Base64:

`S1JZUFRPTklTR1JFQVQ=`

Use this password to log in to **krypton.labs.overthewire.org** with username **krypton1** using SSH on port 2222. You can find the files for other levels in `/krypton/`

#### Solution :

My ticket to Krypton :

```
$ echo "S1JZUFRPTklTR1JFQVQ=" | base64 -d
KRYPTONISGREAT
```


### Krypton Level 1 → Level 2

#### Level Info

The password for level 2 is in the file ‘krypton2’. It is ‘encrypted’ using a simple rotation. It is also in non-standard ciphertext format. When using alpha characters for cipher text it is normal to group the letters into 5 letter clusters, regardless of word boundaries. This helps obfuscate any patterns. This file has kept the plain text word boundaries and carried them to the cipher text. Enjoy!


```
krypton1@krypton:/home$ cd ..
krypton1@krypton:/$ ls
README.txt  bin  boot  d  dev  etc  home  krypton  lib  lib32  lib64  libx32  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
krypton1@krypton:/$ cat README.txt

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


Welcome to the OverTheWire games machine!

If you find any problems, please report them to Steven on
irc.overthewire.org.

--[ Playing the games ]--

  This machine holds several wargames.
  If you are playing "somegame", then:

    * USERNAMES are somegame0, somegame1, ...
    * Most LEVELS are stored in /somegame/.
    * PASSWORDS for each level are stored in /etc/somegame_pass/.

  Write-access to homedirectories is disabled. It is advised to create a
  working directory with a hard-to-guess name in /tmp/.  You can use the
  command "mktemp -d" in order to generate a random and hard to guess
  directory in /tmp/.  Read-access to both /tmp/ and /proc/ is disabled
  so that users can not snoop on eachother.

  Please play nice:

    * don't leave orphan processes running
    * don't leave exploit-files laying around
    * don't annoy other players
    * don't post passwords or spoilers

--[ Tips ]--

  This machine has a 64bit processor and many security-features enabled
  by default, although ASLR has been switched off.  The following
  compiler flags might be interesting:

    -m32                    compile for 32bit
    -fno-stack-protector    disable ProPolice
    -Wl,-z,norelro          disable relro

  In addition, the execstack tool can be used to flag the stack as
  executable on ELF binaries.

  Finally, network-access is limited for most levels by a local
  firewall.

--[ Tools ]--

 For your convenience we have installed a few usefull tools which you can find
 in the following locations:

    * peda (https://github.com/longld/peda) in /usr/local/peda/
    * gdbinit (https://github.com/gdbinit/Gdbinit) in /usr/local/gdbinit/
    * pwntools (https://github.com/Gallopsled/pwntools) in /usr/local/pwntools/
    * radare2 (http://www.radare.org/) should be in $PATH

--[ More information ]--

  For more information regarding individual wargames, visit
  http://www.overthewire.org/wargames/

  For questions or comments, contact us through IRC on
  irc.overthewire.org.

krypton1@krypton:/$ ls
README.txt  bin  boot  d  dev  etc  home  krypton  lib  lib32  lib64  libx32  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
krypton1@krypton:/$ cd kr*
krypton1@krypton:/krypton$ ls
krypton1  krypton2  krypton3  krypton4  krypton5  krypton6
krypton1@krypton:/krypton$ cd kr*
krypton1@krypton:/krypton/krypton1$ ls
README  krypton2
krypton1@krypton:/krypton/krypton1$ cat README
Welcome to Krypton!

This game is intended to give hands on experience with cryptography
and cryptanalysis.  The levels progress from classic ciphers, to modern,
easy to harder.

Although there are excellent public tools, like cryptool,to perform
the simple analysis, we strongly encourage you to try and do these
without them for now.  We will use them in later excercises.

** Please try these levels without cryptool first **


The first level is easy.  The password for level 2 is in the file
'krypton2'.  It is 'encrypted' using a simple rotation called ROT13.
It is also in non-standard ciphertext format.  When using alpha characters for
cipher text it is normal to group the letters into 5 letter clusters,
regardless of word boundaries.  This helps obfuscate any patterns.

This file has kept the plain text word boundaries and carried them to
the cipher text.

Enjoy!
krypton1@krypton:/krypton/krypton1$ cat kr* | tr '[A-Za-z]' '[N-ZA-Mn-za-m]'
LEVEL TWO PASSWORD ROTTEN
krypton1@krypton:/krypton/krypton1$
```

**Plaintext Credentials :** `krypton2:ROTTEN`


### Krypton Level 2 → Level 3

#### Level Info

ROT13 is a simple substitution cipher.

Substitution ciphers are a simple replacement algorithm. In this example of a substitution cipher, we will explore a ‘monoalphebetic’ cipher. Monoalphebetic means, literally, “one alphabet” and you will see why.

This level contains an old form of cipher called a ‘Caesar Cipher’. A Caesar cipher shifts the alphabet by a set number. For example:

plain:  a b c d e f g h i j k ...
cipher: G H I J K L M N O P Q ...
In this example, the letter ‘a’ in plaintext is replaced by a ‘G’ in the ciphertext so, for example, the plaintext ‘bad’ becomes ‘HGJ’ in ciphertext.

The password for level 3 is in the file krypton3. It is in 5 letter group ciphertext. It is encrypted with a Caesar Cipher. Without any further information, this cipher text may be difficult to break. You do not have direct access to the key, however you do have access to a program that will encrypt anything you wish to give it using the key. If you think logically, this is completely easy.

One shot can solve it!

Have fun.

Additional Information:

The encrypt binary will look for the keyfile in your current working directory. Therefore, it might be best to create a working direcory in /tmp and in there a link to the keyfile. As the encrypt binary runs setuid krypton3, you also need to give krypton3 access to your working directory.

Here is an example:

krypton2@melinda:~$ mktemp -d
/tmp/tmp.Wf2OnCpCDQ
krypton2@melinda:~$ cd /tmp/tmp.Wf2OnCpCDQ
krypton2@melinda:/tmp/tmp.Wf2OnCpCDQ$ ln -s /krypton/krypton2/keyfile.dat
krypton2@melinda:/tmp/tmp.Wf2OnCpCDQ$ ls
keyfile.dat
krypton2@melinda:/tmp/tmp.Wf2OnCpCDQ$ chmod 777 .
krypton2@melinda:/tmp/tmp.Wf2OnCpCDQ$ /krypton/krypton2/encrypt /etc/issue
krypton2@melinda:/tmp/tmp.Wf2OnCpCDQ$ ls
ciphertext  keyfile.dat


Solution :

```
Brute-Force : All shifts are computed below.
↓	
+1	NLPDLCTDPLDJ
+2	MKOCKBSCOKCI
+3	LJNBJARBNJBH
+4	KIMAIZQAMIAG
+5	JHLZHYPZLHZF
+6	IGKYGXOYKGYE
+7	HFJXFWNXJFXD
+8	GEIWEVMWIEWC
+9	FDHVDULVHDVB
+10	ECGUCTKUGCUA
+11	DBFTBSJTFBTZ
+12	CAESARISEASY
+13	BZDRZQHRDZRX
+14	AYCQYPGQCYQW
+15	ZXBPXOFPBXPV
+16	YWAOWNEOAWOU
+17	XVZNVMDNZVNT
+18	WUYMULCMYUMS
+19	VTXLTKBLXTLR
+20	USWKSJAKWSKQ
+21	TRVJRIZJVRJP
+22	SQUIQHYIUQIO
+23	RPTHPGXHTPHN
+24	QOSGOFWGSOGM
+25	PNRFNEVFRNFL
```

##### For Shell Ninjas :

```
#!/bin/bash
# Sample usage:
# ./Ccrack3r.sh <key (1-25)> <input file>

tr 'A-Z' 'a-z' < $2  | tr 'a-z' $( echo {a..z} | sed -r 's/ //g' | sed -r "s/(.{$1})(.*)/\2\1/" )
```

Plaintext Credentials : `krypton3:CAESARISEASY`




