# Decompiler_rpy
## Prerequisites
+ Windows 11 (which is my os)
+ Python 2.7
+ Python 3+

## Steps
### Prepare a renpy game package
Find the `/game` path, which has several `.rpa` files in it

### **unrpa** - convert `.rpa` to `.rpyc`
+ Type ```py -3 -m pip install "unrpa"``` in command line to install
+ Use `py -3 -m unrpa` to check if it already exists
```
usage: unrpa [-h] [-v] [-s] [-l | -t] [-p PATH] [-m] [--version]
[--continue-on-error] [-f VERSION] [-o OFFSET] [-k KEY]
FILENAME [FILENAME ...]
unrpa: error: the following arguments are required: FILENAME
```
if it prints this message, it shows that `unrpa` is installed

To use it, input `py -3 -m unrpa scripts.rpa`, the `.rpa` file is what you want to decompile

It will extract several `.rpyc` files

### unrpyc - convert `.rpyc` to `.rpy`
+ [unrpyc github repo](https://github.com/CensoredUsername/unrpyc)
+ clone the repo under the path with `.rpyc` files
+ `py -3 unrpyc/unrpyc.py script01.rpyc` to decompile the `.rpyc` file you want to decompile
+ The path and file names may vary due to your setting

### Here is the `.rpy` file
and it can be seen directly

## Reference
[From Reddit Renpy Forum](https://www.reddit.com/r/RenPy/wiki/guides/decompiling/)
