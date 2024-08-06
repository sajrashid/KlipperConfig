
# Klipper Command to flash via DFU

After the sd-card has been imaged

> [!CAUTION]
> Get the Device ID

`ssh biqu@x.x.x.x`

From an ssh terminal on the host machine

`ls /dev/serial/by-id/*`

Copy the device id and replace after the **=** sign

> [!IMPORTANT]
> Do not leave a space after the =

`make serialflash FLASH_DEVICE=/dev/serial/by-id/usb-Klipper_stm32h723xx_2D003F001751313434373135-if00****`
