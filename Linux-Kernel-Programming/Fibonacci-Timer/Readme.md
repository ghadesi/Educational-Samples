# Fibonacci Timer Kernel Module

a simple module to make an introduction to Kernel module programming using proc file system and Kernel timer functions


### How it works
This module register a proc interface and create the associated file. This proc file could be read and it will generate a simple output each time. The output will depend on how much has been passed since you install the module. The gap between times formed a fionacci sequence.


### Install
You need to insert this command as root user or use sudo as an administrator
```
cd /to/the/module/source/code/
make
insmod ./modulename.ko
```

### Test
to see the output `dmesg`
follow the instruction in the dmesg
to see module information `modinfo ./modulename.ko`


### Uninstall
```
rmmod modulename
make clean
```

for more information read the comments in the code
