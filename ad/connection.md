# Connect With Machine
#plateform/linux #target/remote #cat/CONNECTION

## SMBclinet-ng Fast Login
```
smbclientng -u '<user> -p '<password>' --host <ip>
```

## PowerView Login
```
powerview <domain_name>/<user>:'<password>'@<ip>
```

## PowerView Enum Users
```
powerview <domain_name>/<user>:'<password>'@<ip> -k -q 'Get-DomainUser -Select sAMAccountName' --no-cache
```

## Powerview Web Login
```
powerview <domain_name>/<user>:'<password>'@<ip> -k --web --web-host 0.0.0.0 --web-port 3000 --web-auth user:password1234
```
