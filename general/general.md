# FreeBSD General



## System version



```Bash

freebsd-version -k
freebsd-version -u
uname
uname -r

```

## Permitlogin

```Bash

ee /etc/ssh/sshd_config
ee /etc/rc.d/sshd restart

```

## Upgrade system

```Bash

freebsd-update fetch install

```

## Stable vs Current

FreeBSD has two development branches: FreeBSD-CURRENT and FreeBSD-STABLE.
FreeBSD-CURRENT is the active development branch of FreeBSD, and all new development work, such as adding new feature, will occur in FreeBSD-CURRENT branch firstly.
FreeBSD-STABLE is span off from FreeBSD-CURRENT, and for production version. It mainly accepts bug and security fixes.
You should notice, branches are not points but constant streams of development. And the FreeBSD RELEASE version is a point, and it is just a snapshot of FreeBSD-STABLE branch at some time.


## Installing software via pkg

```Bash

pkg
pkg update -f
pkg install pkg_name
pkg search pkg_name
pkg info

```

## Installing software via port

```Bash

portsnap fetch extract
portsnap fetch update
make install clean BATCH=yes 

```
## Change shell

```Bash

echo $SHELL
chsh -s /usr/local/bin/shell_name

```

## System utils

```Bash

ps
ps -ax
ps auwwx
pstat -s
swapinfo
swapinfo -h
swapinfo -m
procstat
procstat -a
sockstat

```