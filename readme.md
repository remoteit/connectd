remote.it connectd
==================

>   Core remote.it connectivity tool

Install
-------

Download the correct version of `connectd` for your platform from the [releases
page](https://github.com/remoteit/connectd/releases).

### Deciding on the right distribution

If you don't know what version of `connectd` to use on your system and you are
on a Linux/Unix system, download and run the `bintester` to find the best daemon
for ARM and MIPS platforms:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
cd /tmp
sudo wget https://github.com/weaved/misc_bins_and_scripts/raw/master/connectd/bintester
sudo chmod +x bintester
./bintester <ARCHITECTURE>
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

...where `<ARCHITECTURE>` is either `arm` or `mips`.

Usage
-----

Please see [Using connectd](https://support.remote.it/hc/en-us/categories/360004321952-Information-for-developers)
on our documentation site to learn how to use remote.it `connectd`.

Available Releases
------------------

If none of these run, let us know and we will help you build it for your
platform. Currently here are:

| Name                                 | Platform              | Architecture | Linking | OS Version       | Notes                                                                             |
| ------------------------------------ | --------------------- | ------------ | ------- | ---------------- | --------------------------------------------------------------------------------- |
| `.exe`                       | Microsoft Windows     | 32-bit       |         |                  | PE32 executable (console) Intel 80386                                             |
| `.aarch64-openwrt`           | ARM aarch64           | 64-bit       |         |                  | ELF 64-bit LSB, ARM aarch64, version 1 (SYSV), dynamically linked, interpreter /lib/ld-musl-aarch64.so.1                                                            |
| `.aarch64-openwrt_static`    | ARM aarch64           | 64-bit       |         |                  | ELF 64-bit LSB, ARM aarch64, version 1 (SYSV), statically linked                                                            |
| `.x86-osx`                   | i386                  | 32-bit       |         |                  | Mach-O i386 executable                                                            |
| `.x86_64-osx`                | x86-64                | 64-bit       |         |                  | Mach-O 64-bit x86_64 executable                                                   |
| `.arm-android`               | ARM                   | 32-bit       | dynamic |                  | ELF LSB executable, nterpreter /system/bin/linker, EABI5 version 1 (SYSV)         |
| `.arm-android_static`        | ARM                   | 32-bit       | static  |                  | ELF LSB executable, EABI5 version 1 (SYSV)                                        |
| `.arm-gnueabi`               | ARM                   | 32-bit       | dynamic | GNU/Linux 2.6.16 | , ELF LSB executable, interpreter /lib/ld-linux.so.3, EABI5 version 1 (SYSV)      |
| `.arm-gnueabi_static`        | ARM                   | 32-bit       | static  | GNU/Linux 2.6.16 | ELF LSB executable, EABI5 version 1 (SYSV)                                        |
| `.arm-linaro-pi`             | ARM                   | 32-bit       | dynamic | interpreter /lib/ld-| ELF 32-bit LSB executable, ARM, EABI5 version 1 (SYSV)  |
| `c.arm-linaro-pi_static`      | ARM                   | 32-bit       | static  | GNU/Linux 2.6.26 | ELF LSB executable, EABI5 version 1 (SYSV)                                        |
| `.arm-linaro-uclib`             | ARM                   | 32-bit       | dynamic | GNU/Linux 2.6.26 | EABI5 version 1 (SYSV) /lib/ld-linux-armhf.so.3, EABI5 version 1 (SYSV)  |
| `.arm-v5t_le`                | ARM                   | 32-bit       | dynamic | GNU/Linux 2.4.17 | ELF LSB executable, interpreter /lib/ld-linux.so.3, EABI4 version 1 (SYSV)        |
| `.arm-v5t_le_static`         | ARM                   | 32-bit       | static  | GNU/Linux 2.4.17 | ELF LSB executable, EABI4 version 1 (SYSV)                                        |
| `.aarm64-ubuntu16.04`        | ARM aarch64           | 64-bit       | dynamic | GNU/Linux 3.7.0  | ELF LSB executable, interpreter /lib/ld-linux-aarch64.so.1, version 1 (SYSV)      |
| `.aarm64-ubuntu16.04_static` | ARM aarch64           | 64-bit       | static  | GNU/Linux 3.7.0  | ELF LSB executable, version 1 (SYSV)                                              |
| `.mips-24kec`                | MIPS                  | 32-bit       | dynamic |                  | ELF LSB executable, interpreter /lib/ld-uClibc.so.0, MIPS32 rel2 version 1 (SYSV) |
| `.mips-24kec_static`         | MIPS                  | 32-bit       | static  |                  | ELF LSB executable, MIPS32 rel2 version 1 (SYSV)                                  |
| `.mips-34kc`                 | MIPS                  | 32-bit       | dynamic |                  | ELF LSB executable, interpreter /lib/ld-uClibc.so.0, MIPS32 rel2 version 1 (SYSV) |
| `.mips-34kc_static`          | MIPS                  | 32-bit       | static  |                  | ELF LSB executable, MIPS32 rel2 version 1 (SYSV)                                  |
| `.mipsel-bmc5354`            | MIPS                  | 32-bit       | dynamic | GNU/Linux 2.2.15 | ELF LSB executable, interpreter /lib/ld.so.1, MIPS-I version 1 (SYSV)             |
| `.mipsel-bmc5354_static`     | MIPS                  | 32-bit       | static  | GNU/Linux 2.2.15 | ELF LSB executable, MIPS-I version 1 (SYSV)                                       |
| `.mipsel-gcc342`             | MIPS                  | 32-bit       | dynamic |                  | ELF LSB executable, interpreter /lib/ld-uClibc.so.0, MIPS-II version 1 (SYSV)     |
| `.mipsel-gcc342_static`      | MIPS                  | 32-bit       | static  |                  | ELF LSB executable, MIPS-II version 1 (SYSV)                                      |
| `.mips-gcc-4.7.3`            | MIPS                  | 32-bit       | dynamic |                  | ELF LSB executable, interpreter /lib/ld-uClibc.so.0, MIPS-I version 1 (SYSV)      |
| `.mips-gcc-4.7.3_static`     | MIPS                  | 32-bit       | static  |                  | ELF LSB executable, MIPS-I version 1 (SYSV)                                       |
| `.ppc-gnuspe`                | PowerPC or Cisco 4500 | 32-bit       | dynamic | GNU/Linux 2.6.10 | ELF LSB executable, interpreter /lib/ld.so.1, version 1 (SYSV)                    |
| `.ppc-gnuspe_static`         | PowerPC or Cisco 4500 | 32-bit       | static  | GNU/Linux 2.6.10 | ELF LSB executable, version 1 (SYSV)                                              |
| `.x86_64-etch`               | x86-64                | 64-bit       | dynamic | GNU/Linux 2.6.0  | ELF LSB executable, interpreter /lib64/ld-linux-x86-64.so.2, version 1 (SYSV)     |
| `.x86_64-ubuntu16.04`        | x86-64                | 64-bit       | dynamic | GNU/Linux 2.6.32 | ELF LSB executable, interpreter /lib64/ld-linux-x86-64.so.2, version 1 (SYSV)     |
| `.x86_64-ubuntu16.04_static` | x86-64                | 64-bit       | static  | GNU/Linux 2.6.32 | ELF LSB executable, x86-64, version 1 (GNU/Linux)                                 |
| `.x86-etch`                  | Intel 80386           | 32-bit       | dynamic | GNU/Linux 2.4.1  | ELF LSB executable, interpreter /lib/ld-linux.so.2, version 1 (SYSV)              |
| `.x86-linaro_uClibc`         | Intel 80386           | 32-bit       | dynamic |                  | ELF LSB executable, interpreter /lib/ld-uClibc.so.0, version 1 (SYSV)             |
| `.x86-linaro_uClibc_static`  | Intel 80386           | 32-bit       | static  |                  | ELF LSB executable, version 1 (SYSV)                                              |
| `.x86-ubuntu16.04`           | Intel 80386           | 32-bit       | dynamic | GNU/Linux 2.6.32 | ELF LSB executable, interpreter /lib/ld-linux.so.2, version 1 (SYSV)              |
| `.x86-ubuntu16.04_static`    | Intel 80386           | 32-bit       | static  | GNU/Linux 2.6.32 | ELF LSB executable, version 1 (GNU/Linux)                                         |
| `android.tgz`                        | multi                 | multi        | dynamic       | Android          | For Android Apps                                              |
