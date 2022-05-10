# OpenCR Turtlebot 3 ROS2 Core

### OpenCR Firmware for Turtlebot 3 updated for Dynamixel XC430-W150T

## Create Firmware:
```bash
# make script executable
pi@raspberry:~$ chmod 755 ./opencr_ld_shell_arm

# to create the firmware use the following command [ARM BOARD]
# opencr_ld_shell_arm make [SOURCE_BIN] [OUTPUT] [VERSION]
pi@raspberry:~$ opencr_ld_shell_x86 make turtlebot3_core.ino.OpenCR.bin burger 1.0.0
```

## Flash Firmware:
```bash
# make script executable
pi@raspberry:~$ chmod 755 ./update.sh

# to flash the firmware use the following command
# ./update.sh [PORT] [BINARY]
pi@raspberry:~$ ./update.sh /dev/ttyACM0 burger.opencr
```
