# faketime
linux #target/remote UTILS

## Clock skew too great
```
faketime "$(rdate -n <ip> -p | awk '{print $2, $3, $4}' | date -f - "+%Y-%m-%d %H:%M:%S")" zsh
```

## Ntpdate
```
ntpdate <ip>
```