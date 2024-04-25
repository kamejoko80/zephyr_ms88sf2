# zephyr_ms88sf2
Zephyr OS on MS88SF2 IoT board

# Setting up build environment

```
$ mkdir Workspace
$ cd Workspace
$ pip3 install west
$ west init -m git@github.com:kamejoko80/zephyr_ms88sf2.git --mr main
$ west update
$ pip3 install -r zephyr/scripts/requirements.txt
$ pip3 install -r bootloader/mcuboot/scripts/requirements.txt
```
# Install cmake new version:

```
$ sudo apt-get remove cmake
$ mkdir download
$ cd download
$ wget https://cmake.org/files/v3.29/cmake-3.29.1.tar.gz
$ tar -xf cmake-3.29.1.tar.gz
$ cd cmake-3.29.1
$ ./configure
$ make -j2
$ cd bin
$ export PATH=$PATH:$PWD
```
# Install SDK toolchains:

```
$ cd download
$ wget https://github.com/zephyrproject-rtos/sdk-ng/releases/download/v0.16.5-1/zephyr-sdk-0.16.5-1_linux-x86_64.tar.xz
$ tar -xf zephyr-sdk-0.16.5-1_linux-x86_64.tar.xz
$ cd zephyr-sdk-0.16.5-1
$ ./setup.sh
```
