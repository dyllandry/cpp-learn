# trying to figure out how to compile c++

g++, gcc, clang, they are all "drivers" that analyze input arguments to figure out what other things to use to compile your c++ code.

g++ for c++, gcc for c, but g++ is just gcc with flags to compile c++.

On mac, calling g++/gcc actually calls clang, their driver for compiling c.

clang++ vs clang, clang++ will link against c++ and c standard library, where clang just links to c standard library.

I'm gonna use g++, becuase then hopefully these examples will work if I ever swap from my mac to my linux computer.

I included a shell script named `compile.sh` that will compile this c++ program. I leads with a `#!/usr/bin/env bash` command. The system will then use the `env` command to find the first `bash` binary on the system's `PATH` variable and run the remaining of the `compile.sh` program using `bash`.

- [Wikipedia Shebang](https://en.wikipedia.org/wiki/Shebang_(Unix)#:~:text=In%20computing%2C%20a%20shebang%20is,bang%2C%20or%20hash%2Dpling.)
- [What is the preferred Bash shebang ("#!")?](https://stackoverflow.com/a/10383546/7933478)

