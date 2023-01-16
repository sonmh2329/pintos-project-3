# pintos-project-3

Implemented functionality for Virtual Memory into the Pintos Operating System.

References:[https://github.com/salamentic/pintos-project-3/commits/master/src](https://github.com/salamentic/pintos-project-3/commits/master/src)

## Step modifi

Clone project:


```bash
git clone git@github.com:salamentic/pintos-project-3.git
```

### Step 1:

- Mo file `utils/pintos-gdb`, thay GDBMACROS = _<full duong dan den /src/misc/gdb-macros>_

- Mo `utils/Makfile` sua `LOADLIBES` thanh `LDLIBS`

Mo terminal thu muc `/src/utils`, go `make`

### Step 2:

- Sua trong file `/src/vm/Make.vars`

_Line 7_: sua `bochs` thanh `qemu` 

Mo termianl thu muc `/src/vm`. Go `make`

### Step 3:

Sua file `/utils/pintos`

- Line 103: Sua `bochs` thanh `qemu`
- Line 257: Sua `kernel.bin` thanh full path den kernel.bin (...src/vm/build/kernel.bin)
- Line 621: Sua `qemu-system-i386` thanh `qemu-system-x86_64`

### Step 4:

Sua file `utils/Pintos.pm`

- Line 362: Sua `loader.bin` thanh full path den loader.bin (...src/vm/build/loader.bin)

### Step 5:

- Sua file `.bashrc` tai folder `/home`, them dong sau:

`export PATH=/home/.../pintos/src/utils:$PATH`

Xem chi tiet commit de lam theo [tai day](https://github.com/sonmh2329/pintos-project-3/commit/7a78c4c9d9ee911edc81a6683dd539d54f4ef693)

### Step 6:

Go `make check` tai `src/vm`