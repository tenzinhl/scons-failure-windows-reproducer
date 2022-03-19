Output from running `scons` in this folder:

```
scons: Reading SConscript files ...
scons: done reading SConscript files.
scons: Building targets ...
gcc -o hello.o -c hello.c
The system cannot find the path specified.
scons: *** [hello.o] Error 1
scons: building terminated because of errors.
```

`hello.o` is created. (I'm pretty sure the object file is valid too)

**NOTE:** at one point (not with this exact setup) I was able
to get it so that it would "building terminated because of errors" but
it would *still successfully build* the last node it tried to build.

This meant you could call `scons` a few times to incrementally build
each step until it eventually succeeded (it wouldn't try to rebuild
the existing ones which is why this worked). And the final product
could be run!

My brain's kind of fried rn though so I'm not gonna try and even
think about how to repro that.
