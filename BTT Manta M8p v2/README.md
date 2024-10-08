# Klipper Configuration for Manta M8P v2.0

> [!Warning]
> This is a custom conversion for a **WiBox 3** from a dual z cartesian to a triple Z coreXY similar to a Voron Trident

- Phase 1 will convert the electronics to a Manta M8P - In Test
- Phase 2 is to add the additional Z axis & ToolHead - Not Started
- Phase 3 is to change the x/y axis to coreXY- Not Started
- Phase 4 is to add additional x and/or y axis to Quad coreXY- Not Started
- 

Firmware MCU selection STM32H723 with a "128KiB bootloader" "25 MHz &crystal"

## Klipper Command to flash via DFU

After the sd-card has been imaged

> [!CAUTION]
> Get the Device ID

`ssh biqu@x.x.x.x`

From an ssh terminal on the host machine

`ls /dev/serial/by-id/*`

Copy the device id and replace after the **=** sign

> [!IMPORTANT]
> Do not leave a space after the =

`make serialflash FLASH_DEVICE=/dev/serial/by-id/usb-Klipper_stm32h723xx_2D003F001751313434373135-if00

****`
