# proot-static
Static builded of Termux's version proot. Only armhf binary files, but also works on arm64

## Usage example
0) proot-static can be used to run 32 bit proot systems on 64 bit environments without installing 32 bit packages, and switching environment (Not tested yet, only in theory!).
1) also proot-static does not require any dependency on the system, accordingly can be started without any dependencies (talloc, libc) (Only in Android, of course)

## Usage
```
$ git clone https://github.com/ZhymabekRoman/proot-static
$ cd proot-static/
$ ./proot_static --help
```
