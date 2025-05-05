# rusthound
#plateform/linux #target/remote #cat/RECON

## Execute RustHound
```
rusthound -d <domain> -u <user>@<domain> -p '<passwd>' -f <target> -n <ip> -z -o <output_dir|rusthound>
```

## RustHound Skip DNS
```
rusthound -d <domain> -u <user>@<domain> -p '<passwd>' -f <ip> -i <ip> -z -o <output_dir|rusthound>
```