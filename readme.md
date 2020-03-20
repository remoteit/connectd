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

Please see [Using connectd](https://docs.remote.it/connectd-reference/connectd)
on our documentation site to learn how to use remote.it `connectd`.

Available Releases
------------------

If none of these run, let us know and we will help you build it for your
platform. Currently here are:

| Name                                 | Platform              | Architecture | Linking       | OS Version       | Notes                                                                             |
|--------------------------------------|-----------------------|--------------|---------------|------------------|-----------------------------------------------------------------------------------|
| `connectd.exe`                       | Microsoft Windows     | 32-bit       | VS static     |                  | PE32 executable (console) Intel 80386                                             |
| `connectd.exe`                       | Microsoft Windows     | 32-bit       | Migwin static |                  | PE32 executable (console) Intel 80386 (stripped to external PDB)                  |
| `connectd.x86_64-win.exe`            | Microsoft Windows     | 64-bit       | Migwin static |                  | PE32+ executable (console) x86-64 (stripped to external PDB)                      |
| `connectd.x86-osx`                   | i386                  | 32-bit       |               |                  | Mach-O i386 executable                                                            |
| `connectd.x86_64-osx`                | x86-64                | 64-bit       |               |                  | Mach-O 64-bit x86_64 executable                                                   |
| `connectd.arm-android`               | ARM                   | 32-bit       | dynamic       |                  | ELF LSB executable, nterpreter /system/bin/linker, EABI5 version 1 (SYSV)         |
| `connectd.arm-android_static`        | ARM                   | 32-bit       | static        |                  | ELF LSB executable, EABI5 version 1 (SYSV)                                        |
| `connectd.arm-gnueabi`               | ARM                   | 32-bit       | dynamic       | GNU/Linux 2.6.16 | , ELF LSB executable, interpreter /lib/ld-linux.so.3, EABI5 version 1 (SYSV)      |
| `connectd.arm-gnueabi_static`        | ARM                   | 32-bit       | static        | GNU/Linux 2.6.16 | ELF LSB executable, EABI5 version 1 (SYSV)                                        |
| `connectd.arm-linaro-pi`             | ARM                   | 32-bit       | dynamic       | GNU/Linux 2.6.26 | ELF LSB executable, interpreter /lib/ld-linux-armhf.so.3, EABI5 version 1 (SYSV)  |
| `connectd.arm-linaro-pi_static`      | ARM                   | 32-bit       | static        | GNU/Linux 2.6.26 | ELF LSB executable, EABI5 version 1 (SYSV)                                        |
| `connectd.arm-v5t_le`                | ARM                   | 32-bit       | dynamic       | GNU/Linux 2.4.17 | ELF LSB executable, interpreter /lib/ld-linux.so.3, EABI4 version 1 (SYSV)        |
| `connectd.arm-v5t_le_static`         | ARM                   | 32-bit       | static        | GNU/Linux 2.4.17 | ELF LSB executable, EABI4 version 1 (SYSV)                                        |
| `connectd.aarm64-ubuntu16.04`        | ARM aarch64           | 64-bit       | dynamic       | GNU/Linux 3.7.0  | ELF LSB executable, interpreter /lib/ld-linux-aarch64.so.1, version 1 (SYSV)      |
| `connectd.aarm64-ubuntu16.04_static` | ARM aarch64           | 64-bit       | static        | GNU/Linux 3.7.0  | ELF LSB executable, version 1 (SYSV)                                              |
| `connectd.mips-24kec`                | MIPS                  | 32-bit       | dynamic       |                  | ELF LSB executable, interpreter /lib/ld-uClibc.so.0, MIPS32 rel2 version 1 (SYSV) |
| `connectd.mips-24kec_static`         | MIPS                  | 32-bit       | static        |                  | ELF LSB executable, MIPS32 rel2 version 1 (SYSV)                                  |
| `connectd.mips-34kc`                 | MIPS                  | 32-bit       | dynamic       |                  | ELF LSB executable, interpreter /lib/ld-uClibc.so.0, MIPS32 rel2 version 1 (SYSV) |
| `connectd.mips-34kc_static`          | MIPS                  | 32-bit       | static        |                  | ELF LSB executable, MIPS32 rel2 version 1 (SYSV)                                  |
| `connectd.mipsel-bmc5354`            | MIPS                  | 32-bit       | dynamic       | GNU/Linux 2.2.15 | ELF LSB executable, interpreter /lib/ld.so.1, MIPS-I version 1 (SYSV)             |
| `connectd.mipsel-bmc5354_static`     | MIPS                  | 32-bit       | static        | GNU/Linux 2.2.15 | ELF LSB executable, MIPS-I version 1 (SYSV)                                       |
| `connectd.mipsel-gcc342`             | MIPS                  | 32-bit       | dynamic       |                  | ELF LSB executable, interpreter /lib/ld-uClibc.so.0, MIPS-II version 1 (SYSV)     |
| `connectd.mipsel-gcc342_static`      | MIPS                  | 32-bit       | static        |                  | ELF LSB executable, MIPS-II version 1 (SYSV)                                      |
| `connectd.mips-gcc-4.7.3`            | MIPS                  | 32-bit       | dynamic       |                  | ELF LSB executable, interpreter /lib/ld-uClibc.so.0, MIPS-I version 1 (SYSV)      |
| `connectd.mips-gcc-4.7.3_static`     | MIPS                  | 32-bit       | static        |                  | ELF LSB executable, MIPS-I version 1 (SYSV)                                       |
| `connectd.ppc-gnuspe`                | PowerPC or Cisco 4500 | 32-bit       | dynamic       | GNU/Linux 2.6.10 | ELF LSB executable, interpreter /lib/ld.so.1, version 1 (SYSV)                    |
| `connectd.ppc-gnuspe_static`         | PowerPC or Cisco 4500 | 32-bit       | static        | GNU/Linux 2.6.10 | ELF LSB executable, version 1 (SYSV)                                              |
| `connectd.x86_64-etch`               | x86-64                | 64-bit       | dynamic       | GNU/Linux 2.6.0  | ELF LSB executable, interpreter /lib64/ld-linux-x86-64.so.2, version 1 (SYSV)     |
| `connectd.x86_64-ubuntu16.04`        | x86-64                | 64-bit       | dynamic       | GNU/Linux 2.6.32 | ELF LSB executable, interpreter /lib64/ld-linux-x86-64.so.2, version 1 (SYSV)     |
| `connectd.x86_64-ubuntu16.04_static` | x86-64                | 64-bit       | static        | GNU/Linux 2.6.32 | ELF LSB executable, x86-64, version 1 (GNU/Linux)                                 |
| `connectd.x86-etch`                  | Intel 80386           | 32-bit       | dynamic       | GNU/Linux 2.4.1  | ELF LSB executable, interpreter /lib/ld-linux.so.2, version 1 (SYSV)              |
| `connectd.x86-linaro_uClibc`         | Intel 80386           | 32-bit       | dynamic       |                  | ELF LSB executable, interpreter /lib/ld-uClibc.so.0, version 1 (SYSV)             |
| `connectd.x86-linaro_uClibc_static`  | Intel 80386           | 32-bit       | static        |                  | ELF LSB executable, version 1 (SYSV)                                              |
| `connectd.x86-ubuntu16.04`           | Intel 80386           | 32-bit       | dynamic       | GNU/Linux 2.6.32 | ELF LSB executable, interpreter /lib/ld-linux.so.2, version 1 (SYSV)              |
| `connectd.x86-ubuntu16.04_static`    | Intel 80386           | 32-bit       | static        | GNU/Linux 2.6.32 | ELF LSB executable, version 1 (GNU/Linux)                                         |
