Recursive Fibonacci function defined in various languages:
==========================================================

Comparing various langs for fun. Should not be considered as true benchmarks of any kind.
Timmings on 2-core Intel(R) Core(TM) i7-5600U CPU @ 2.60GHz running Ubuntu 14.04


[C](https://gcc.gnu.org/)
==

To Compile:
-----------

``````
$ gcc -std=c99 fibo.c -o fibo

$ ls -l fibo
-rwxrwxr-x 1 shashank shashank 8594 Feb  4 20:29 fibo
``````

Dependencies:
-------------

``````
$ ldd ./fibo
  linux-vdso.so.1 =>  (0x00007ffef8e55000)
  libc.so.6 => /lib/x86_64-linux-gnu/libc.so.6 (0x00007f4fe1545000)
  /lib64/ld-linux-x86-64.so.2 (0x000055be39a12000)
``````

Runtime:
--------

``````
$ time ./fibo
2178309

real  0m0.128s
user  0m0.080s
sys   0m0.016s
``````


***

[Lua](https://www.lua.org/)
===

``````
$ time lua fibo.lua
2178309

real  0m0.554s
user  0m0.368s
sys   0m0.092s

$ time luajit fibo.lua
2178309

real  0m0.073s
user  0m0.036s
sys   0m0.008s
``````


***

[mRuby](http://mruby.org/)
=====


***

[Crystal](http://crystal-lang.org/)
=======

***

[Ruby](https://www.ruby-lang.org/)
====

***

[Perl](https://www.perl.org/)
====

***

[Javascript](https://www.javascript.com/)
==========

***

[Python](https://www.python.org/)
======

***

[Haskell](https://www.haskell.org/ghc/)
=======

To Compile:
-----------

``````
$ ghc -o fibo fibo.hs

$ ls -l fibo
-rwxrwxr-x 1 shashank shashank 1104363 Feb  4 20:44 fibo
``````

Dependencies:
-------------

``````
$ ldd fibo
  linux-vdso.so.1 =>  (0x00007ffd3b790000)
  libgmp.so.10 => /usr/lib/x86_64-linux-gnu/libgmp.so.10 (0x00007f1e67e47000)
  libffi.so.6 => /usr/lib/x86_64-linux-gnu/libffi.so.6 (0x00007f1e67c3f000)
  libm.so.6 => /lib/x86_64-linux-gnu/libm.so.6 (0x00007f1e67938000)
  librt.so.1 => /lib/x86_64-linux-gnu/librt.so.1 (0x00007f1e67730000)
  libdl.so.2 => /lib/x86_64-linux-gnu/libdl.so.2 (0x00007f1e6752c000)
  libc.so.6 => /lib/x86_64-linux-gnu/libc.so.6 (0x00007f1e67166000)
  libpthread.so.0 => /lib/x86_64-linux-gnu/libpthread.so.0 (0x00007f1e66f48000)
  /lib64/ld-linux-x86-64.so.2 (0x0000563647a27000)
``````

Runtime:
--------
``````
$ time ./fibo
2178309

real  0m1.108s
user  0m1.012s
sys   0m0.048s
``````

***


[Elixir](http://www.elixir-lang.org/)
======

***

[Rust](https://www.rust-lang.org)
====

***

[Go](https://golang.org)
===

***

[Bash](https://www.gnu.org/software/bash/)
====


***

