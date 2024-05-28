sudo service klipper stop

make flash FLASH_DEVICE=/dev/serial/by-id/usb-1a86_USB2.0-Serial-if00-port0


## CB1 (HOST)
- Linux process
```zsh
make clean menuconfig  #select `Linux process`
sudo service klipper stop
make flash
sudo service klipper start
```

## M5P (MCU)
![alt text](menuconfig.png)
```zsh
make clean menuconfig
sudo service klipper stop
make flash FLASH_DEVICE=/dev/serial/by-id/usb-Klipper_stm32g0b1xx_440047000B504B5735313920-if00
sudo service klipper start
```
