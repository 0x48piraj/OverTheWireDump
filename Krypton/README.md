## Krypton

> The Krypton wargame.

### Krypton Level 0 → Level 1

#### Level Info
> Uplink: http://overthewire.org/wargames/krypton/krypton0.html

Welcome to Krypton! The first level is easy. The following string encodes the password using Base64:

`S1JZUFRPTklTR1JFQVQ=`

Use this password to log in to **krypton.labs.overthewire.org** with username **krypton1** using SSH on port 2222. You can find the files for other levels in `/krypton/`

#### Solution :

```
$ echo "S1JZUFRPTklTR1JFQVQ=" | base64 -d
KRYPTONISGREAT
```

Krypton Level 1 → Level 2

Level Info

The password for level 2 is in the file ‘krypton2’. It is ‘encrypted’ using a simple rotation. It is also in non-standard ciphertext format. When using alpha characters for cipher text it is normal to group the letters into 5 letter clusters, regardless of word boundaries. This helps obfuscate any patterns. This file has kept the plain text word boundaries and carried them to the cipher text. Enjoy!
