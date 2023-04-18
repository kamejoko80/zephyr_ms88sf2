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
