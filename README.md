# closesocks

A simple script to list idle open sockets for a process, and optionally close
them.

It generates [ss](https://linux.die.net/man/8/ss) command lines to kill the
processes. By default it shows them, and can also directly run them.

```
usage: closesocks [-h] [--verbose] [--debug] [--pid pid] [--idle seconds]
                  [--force]

List idle open sockets, and optionally close them

optional arguments:
  -h, --help         show this help message and exit
  --verbose, -v      verbose output
  --debug            debug output
  --pid pid, -p pid  pid to list
  --idle seconds     select connections idle for more than this amount of
                     seconds (default: 3600)
  --force, -f        run the commands instead of listing them
```
