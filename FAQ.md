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
git pull --recurse-submodules
```