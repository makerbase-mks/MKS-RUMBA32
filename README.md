# MKS RUMBA32
## Feature
 - CPU is STM32F446VET6,180MHZ...
 - MKS RUMBA32 hardware change base on Aus3d rumba32;
 - Support connect MKS TFT by AUX-1...
 - Support TMC SPI mode interface...
 - Support MKS TMC2208/2209 uart mode and TMC2130 spi mode(Marlin firmware need fix...)
 - Support platformio build and upload firmware online...
 
## How to build and upload marlin2.0 firmware for MKS RUMBA32
MKS RUMBA32 build and upload marlin2.0 can use platformio, how to do it? Please see the following tutorial.

### MKS RUMBA32 bootloader drive install
 - USB connect MKS RUMBA32, press and hold the "BOOT" button, then press the "RESET" light strip for more than 1S, release "RESET", and then release "BOOT". The motherboard enters DFU mode.
 ![1_connect_board](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/1_connect_board.png "1_connect_board")
 - We need to show STM32 BOOTLOADER installation failed
 ![2_stm32boorloader_fail](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/2_stm32boorloader_fail.png "2_stm32boorloader_fail")
 - Open Zadig.exe, set and install drive
 ![3_set_zadig_install](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/3_set_zadig_install.png "3_set_zadig_install")
 - Install drive ok
 ![4_install_ok_1](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/4_install_ok_1.png "4_install_ok_1")
 ![4_install_ok_2](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/4_install_ok_2.png "4_install_ok_2")
 
### Build and upload marlin2.0 firmware
 - Open marlin2.0 project(need download mks github rumba32 path marlin firmware)
 ![5_open_project](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/5_open_project.png "5_open_project")
 - Platformio.ini set as mks_rumba32 and configuration.h set board 
 ![6_set_mks_rumba32](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/6_set_mks_rumba32.png "6_set_mks_rumba32")
 ![6_set_mks_rumba32_board](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/6_set_mks_rumba32_board.png "6_set_mks_rumba32_board")
 - Build and upload marlin2.0 firmware
 First, upload firmware, MKS RUMBA32 board need enter DFU mode. USB connect MKS RUMBA32, press and hold the "BOOT" button, then press the "RESET" light strip for more than 1S, release "RESET", and then release "BOOT".
 ![4_install_ok_2](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/4_install_ok_2.png "4_install_ok_2")
 Second, upload firmware
 [7_build_upload](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/7_build_upload.png "7_build_upload")

### MKS RUMBA32 after upload marlin2.0 firmware
 - Connect MKS MINI12864 V2.1
 [8_test_ok](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/8_test_ok.png "8_test_ok")
 
## How to connect pronterface by usb
 - When after upload firmware, we look like this
 [9_usb_not_com](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/9_usb_not_com.png "9_usb_not_com")
 - We need update COM drive and use SSTM32 virtual serial port
 [10_install_stm32_drive](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/10_install_stm32_drive.png "10_install_stm32_drive")
 - After installing the STM32 virtual serial port, we need to manually update the COM
 [11_updatecom1](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/11_updatecom1.png "11_updatecom1")
 [11_updatecom2](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/11_updatecom2.png "11_updatecom2")
 [11_updatecom3](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/11_updatecom3.png "11_updatecom3")
 [11_updatecom4](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/11_updatecom4.png "11_updatecom4")
 [11_updatecom5](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/11_updatecom5.png "11_updatecom5")
 - Connet pronterface test
 [12_connet_pc_ok](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/12_connet_pc_ok.png "12_connet_pc_ok")
 
## How to update marlin2.0 firmware.bin file
 - Copy firmware.bin file to update firmware bin file path
 [13_copy_firmware_bin](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/13_copy_firmware_bin.png "13_copy_firmware_bin")
 - Run Upload.bat(MKS RUMBA32 need enter DFU mode)
 [14_update_firmware_bin_flie](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/14_update_firmware_bin_flie.png "14_update_firmware_bin_flie")

## How to buy the MKS RUMBA32
 - Link：https://www.aliexpress.com/item/4000717327779.html?spm=2114.12010612.8148356.19.86d51141BPaqTo
 [MKS_RUMBA32](https://github.com/makerbase-mks/MKS-RUMBA32/blob/master/Picture/MKS_RUMBA32.png "MKS_RUMBA32")

