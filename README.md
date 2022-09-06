# proot-static
A static compiled version of proot from Termux. Only armhf binary files, but also works on arm64

## Usage example
proot-static can be used to run 32 bit proot systems on 64 bit environments without installing 32 bit packages, and switching environment (for example, to run box86/box64). Also proot-static does not require any dependency on the system, accordingly can be started without any dependencies (talloc and etc) (only in Android, of course).

## Usage
```
$ git clone https://github.com/ZhymabekRoman/proot-static
$ cd proot-static/
$ ./proot_static --help
```
Or you can overwrite the PATH value to use proot-static, instead of the usual proot:
```
$ git clone https://github.com/ZhymabekRoman/proot-static
$ cd proot-static/
$ export PATH=`pwd`/bin:$PATH
$ export PROOT_LOADER=`pwd`/bin/loader
```

## Compile
Clone `termux-packages` repository and apply patch `patches/proot_static_compile.patch`. For compilation I used GitHub Action (CI).
