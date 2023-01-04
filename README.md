# dynamic-tracking-system
dynamic tracking system

# dtrace
```
dtrace -n 'exec-success { printf("%d %s", timestamp, curpsinfo->pr_psargs); }'


dtrace -n 'exec-success { printf("%d %s", timestamp, curpsinfo->pr_psargs); }'

dtrace -n 'readch {trace(pid)}'
```

# debug
```
ps H -eo pid,pcpu | sort -nk2 | tail
```

# 参考

- https://docs.oracle.com/cd/E24847_01/html/E22192/gcfbn.html
