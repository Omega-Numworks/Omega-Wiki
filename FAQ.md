## `apps/rpn/Makefile`: No such file or directory

**Error**
```
Omega git:(omega-master) make PLATFORM=simulator
apps/Makefile:11: apps/rpn/Makefile: No such file or directory
make: *** No rules to make « apps/rpn/Makefile ». Stop.
```

**Fix**

You forgot the `--recursive` tag during clone. Execute the following command:
```
git submodule update --init --recursive
```

## No targets specified and no makefile found.  Stop.

**Error**
```
make: *** No targets specified and no makefile found.  Stop.
```

**Fix**
You forgot to cd to /Omega. Execute the following command:
```
cd /Omega
```

## Command not found
**Error**
```
/bin/sh:[differents things can be here]
```

**Fix**
You are missing at least one dependence follow the first step of [this guide](https://www.numworks.com/resources/engineering/software/build/)

## Acces denied
**Error**
```
Any acces denied error
```

**Fix**

You forgot to close a webpage or terminal which is connected to the calculator: close them

## Compilation is very slow
**Error**

The compilation is very slow 

**Fix**

If you have a powerfull enough computer you can modify the number in -j4 it defines the threads number

