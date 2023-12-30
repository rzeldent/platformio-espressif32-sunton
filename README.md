# Sunton CYD (Cheap Yellow Display) PlatformIo Board definitions
# Sunton CYD (Cheap Yellow Display) PlatformIo Board definitions

## This repo contains definitions for the CPU and board information about the hardware

The json files are to be used with PlatformIo and contain defines that specify the location and type of the hardware.
When this repository is used as a git submodule in the directory ```<project>/boards``` This will be detected automatically.

## Supported boards

| Type              | USB       | CPU                       | Flash | PSRAM | Cores/Speed | Display                                 | Size        | Display interface | Display controller                       | Touch interface    | Touch controller                          | Audio                                     | Flash                                          | LED  | CdS                                       | Relay  | Link                                                                  |
|---                |---        |---                        |---    |---    |--           |---                                      |--           |---                |---                                       |---                 |---                                        |---                                        |---                                             |---   |---                                        |---     |---                                                                    |
| ESP32_1732S019N   | micro USB | ESP32-S3-WROOM-1-MCN16R8  | 16Mb  | 8Mb   | 2 x 240Mhz  | 170x320                                 | 1.9"        | SPI               | [ST7796](assets/datasheets/ST7796.pdf)   |                    |                                           |                                           |                                                |      |                                           |        | [Ali Express](https://www.aliexpress.com/item/1005005059421229.html)  |
| ESP32_1732S019C   | micro USB | ESP32-S3-WROOM-1-MCN16R8  | 16Mb  | 8Mb   | 2 x 240Mhz  | 170x320                                 | 1.9"        | SPI               | [ST7796](assets/datasheets/ST7796.pdf)   | I2C                | [GT911](assets/datasheets//GT911.pdf)     |                                           |                                                |      |                                           |        | [Ali Express](https://www.aliexpress.com/item/1005005059421229.html)  |
| ESP32-2424S012N   | USB-C     | ESP32-C3-MINI-1U-XXN4     | 4Mb   |       | 1 x 160Mhz  | 240x240                                 | 1.2" round  | SPI               | [GC9A01A](assets/datasheets/GC9A01A.pdf) |                    |                                           |                                           |                                                |      |                                           |        | [Ali Express](https://www.aliexpress.com/item/1005005453515690.html)  |
| ESP32-2424S012C   | USB-C     | ESP32-C3-MINI-1U-XXN4     | 4Mb   |       | 1 x 160Mhz  | 240x240                                 | 1.2" round  | SPI               | [GC9A01A](assets/datasheets/GC9A01A.pdf) | I2C                | [CST816S](assets/datasheets/CST816S.pdf)  |                                           |                                                |      |                                           |        | [Ali Express](https://www.aliexpress.com/item/1005005453515690.html)  |
| ESP32-2432S024N   | micro USB | ESP32-WROOM-32            | 4Mb   |       | 2 x 240Mhz  | [240x320](assets/lcd/JC2432A024N.pdf)   | 2.4"        | SPI               | [ILI9341](assets/datasheets/ILI9341.pdf) |                    |                                           | [FM8002A](assets/datasheets/FM8002A.pdf)  | [W25Q32JV](assets/datasheets/25Q32JVSSIQ.pdf)  | RGB  | [GT36516](assets/datasheets//GT36516.pdf) |        | [Ali Express](https://www.aliexpress.com/item/1005005865107357.html)  |
| ESP32-2432S024R   | micro USB | ESP32-WROOM-32            | 4Mb   |       | 2 x 240Mhz  | [240x320](assets/lcd/JC2432A024N.pdf)   | 2.4"        | SPI               | [ILI9341](assets/datasheets/ILI9341.pdf) | SPI                | [XPT2046](assets/datasheets/XPT2046.pdf)  | [FM8002A](assets/datasheets/FM8002A.pdf)  | [W25Q32JV](assets/datasheets/25Q32JVSSIQ.pdf)  | RGB  | [GT36516](assets/datasheets//GT36516.pdf) |        | [Ali Express](https://www.aliexpress.com/item/1005005865107357.html)  |
| ESP32-2432S024C   | micro USB | ESP32-WROOM-32            | 4Mb   |       | 2 x 240Mhz  | [240x320](assets/lcd/JC2432A024N.pdf)   | 2.4"        | SPI               | [ILI9341](assets/datasheets/ILI9341.pdf) | I2C                | [CST816S](assets/datasheets/CST816S.pdf)  | [FM8002A](assets/datasheets/FM8002A.pdf)  | [W25Q32JV](assets/datasheets/25Q32JVSSIQ.pdf)  | RGB  | [GT36516](assets/datasheets//GT36516.pdf) |        | [Ali Express](https://www.aliexpress.com/item/1005005865107357.html)  |
| ESP32-2432S028R   | micro USB | ESP32-WROOM-32            | 4Mb   |       | 2 x 240Mhz  | [240x320](assets/lcd/JC2432A028N.pdf)   | 2.8"        | SPI               | [ILI9341](assets/datasheets/ILI9341.pdf) | SPI                | [XPT2046](assets/datasheets/XPT2046.pdf)  | [FM8002A](assets/datasheets/FM8002A.pdf)  | [W25Q32JV](assets/datasheets/25Q32JVSSIQ.pdf)  | RGB  | [GT36516](assets/datasheets//GT36516.pdf) |        | [Ali Express](https://www.aliexpress.com/item/1005004502250619.html)  |
| ESP32-2432S028Rv2 | USB-C     | ESP32-WROOM-32            | 4Mb   |       | 2 x 240Mhz  | [240x320](assets/lcd/JC2432B028N.pdf)   | 2.8"        | SPI               | [ILI9341](assets/datasheets/ILI9341.pdf) | SPI                | [XPT2046](assets/datasheets/XPT2046.pdf)  | [FM8002A](assets/datasheets/FM8002A.pdf)  | [W25Q32JV](assets/datasheets/25Q32JVSSIQ.pdf)  | RGB  | [GT36516](assets/datasheets//GT36516.pdf) |        | [Ali Express](https://www.aliexpress.com/item/1005004502250619.html)  |
| ESP32-2432S032N   | micro USB | ESP32-WROOM-32            | 4Mb   |       | 2 x 240Mhz  | 240x320                                 | 3.2"        | SPI               | [ST7796](assets/datasheets/ST7796.pdf)   |                    |                                           | [FM8002A](assets/datasheets/FM8002A.pdf)  | [W25Q32JV](assets/datasheets/25Q32JVSSIQ.pdf)  | RGB  | [GT36516](assets/datasheets//GT36516.pdf) |        | [Ali Express](https://www.aliexpress.com/item/1005006224494145.html)  |
| ESP32-2432S032R   | micro USB | ESP32-WROOM-32            | 4Mb   |       | 2 x 240Mhz  | 240x320                                 | 3.2"        | SPI               | [ST7796](assets/datasheets/ST7796.pdf)   | SPI                | [XPT2046](assets/datasheets/XPT2046.pdf)  | [FM8002A](assets/datasheets/FM8002A.pdf)  | [W25Q32JV](assets/datasheets/25Q32JVSSIQ.pdf)  | RGB  | [GT36516](assets/datasheets//GT36516.pdf) |        | [Ali Express](https://www.aliexpress.com/item/1005006224494145.html)  |
| ESP32-2432S032C   | micro USB | ESP32-WROOM-32            | 4Mb   |       | 2 x 240Mhz  | 240x320                                 | 3.2"        | SPI               | [ST7796](assets/datasheets/ST7796.pdf)   | I2C                | [GT911](assets/datasheets//GT911.pdf)     | [FM8002A](assets/datasheets/FM8002A.pdf)  | [W25Q32JV](assets/datasheets/25Q32JVSSIQ.pdf)  | RGB  | [GT36516](assets/datasheets//GT36516.pdf) |        | [Ali Express](https://www.aliexpress.com/item/1005006224494145.html)  |
| ESP32-3248S035R   | micro USB | ESP32-WROOM-32            | 4Mb   |       | 2 x 240Mhz  | 320x480                                 | 3.5"        | SPI               | [ST7796](assets/datasheets/ST7796.pdf)   | SPI                | [XPT2046](assets/datasheets/XPT2046.pdf)  | [FM8002A](assets/datasheets/FM8002A.pdf)  | [W25Q32JV](assets/datasheets/25Q32JVSSIQ.pdf)  | RGB  | [GT36516](assets/datasheets//GT36516.pdf) |        | [Ali Express](https://www.aliexpress.com/item/1005004632953455.html)  |
| ESP32-3248S035C   | micro USB | ESP32-WROOM-32            | 4Mb   |       | 2 x 240Mhz  | 320x480                                 | 3.5"        | SPI               | [ST7796](assets/datasheets/ST7796.pdf)   | I2C                | [GT911](assets/datasheets//GT911.pdf)     | [FM8002A](assets/datasheets/FM8002A.pdf)  | [W25Q32JV](assets/datasheets/25Q32JVSSIQ.pdf)  | RGB  | [GT36516](assets/datasheets//GT36516.pdf) |        | [Ali Express](https://www.aliexpress.com/item/1005004632953455.html)  |
| ESP32-4827S043R   | USB-C     | ESP32-S3-WROOM-1-MCN16R8  | 16Mb  | 8Mb   | 2 x 240Mhz  | [480x272](assets/lcd/JC4827B043N.pdf)   | 4.3"        | Direct            | [ST7701](assets/datasheets/ST7701S.pdf)  | SPI                | [XPT2046](assets/datasheets/XPT2046.pdf)  |                                           |                                                |      |                                           |        | [Ali Express](https://www.aliexpress.com/item/1005004788147691.html)  |
| ESP32-4827S043C   | USB-C     | ESP32-S3-WROOM-1-MCN16R8  | 16Mb  | 8Mb   | 2 x 240Mhz  | [480x272](assets/lcd/JC4827B043N.pdf)   | 4.3"        | Direct            | [ST7701](assets/datasheets/ST7701S.pdf)  | I2C                | [GT911](assets/datasheets//GT911.pdf)     |                                           |                                                |      |                                           |        | [Ali Express](https://www.aliexpress.com/item/1005004788147691.html)  |
| ESP32-8048S043N   | USB-C     | ESP32-S3-WROOM-1-MCN16R8  | 16Mb  | 8Mb   | 2 x 240Mhz  | 800x480                                 | 4.3"        | Direct            | [ST7701](assets/datasheets/ST7701S.pdf)  |                    |                                           |                                           |                                                |      |                                           |        | [Ali Express](https://www.aliexpress.com/item/1005006110360174.html)  |
| ESP32-8048S043R   | USB-C     | ESP32-S3-WROOM-1-MCN16R8  | 16Mb  | 8Mb   | 2 x 240Mhz  | 800x480                                 | 4.3"        | Direct            | [ST7701](assets/datasheets/ST7701S.pdf)  | SPI                | [XPT2046](assets/datasheets/XPT2046.pdf)  |                                           |                                                |      |                                           |        | [Ali Express](https://www.aliexpress.com/item/1005006110360174.html)  |
| ESP32-8048S043C   | USB-C     | ESP32-S3-WROOM-1-MCN16R8  | 16Mb  | 8Mb   | 2 x 240Mhz  | 800x480                                 | 4.3"        | Direct            | [ST7701](assets/datasheets/ST7701S.pdf)  | I2C                | [GT911](assets/datasheets//GT911.pdf)     |                                           |                                                |      |                                           |        | [Ali Express](https://www.aliexpress.com/item/1005006110360174.html)  |
| ESP32-8048S050N   | USB-C     | ESP32-S3-WROOM-1-MCN16R8  | 16Mb  | 8Mb   | 2 x 240Mhz  | 800x480                                 | 5.0"        | Direct            | [ST7701](assets/datasheets/ST7701S.pdf)  |                    |                                           |                                           |                                                |      |                                           |        | [Ali Express](https://www.aliexpress.com/item/1005005938915207.html)  |
| ESP32-8048S050C   | USB-C     | ESP32-S3-WROOM-1-MCN16R8  | 16Mb  | 8Mb   | 2 x 240Mhz  | 800x480                                 | 5.0"        | Direct            | [ST7701](assets/datasheets/ST7701S.pdf)  | I2C                | [GT911](assets/datasheets//GT911.pdf)     |                                           |                                                |      |                                           |        | [Ali Express](https://www.aliexpress.com/item/1005005938915207.html)  |
| ESP32-8048S050R   | USB-C     | ESP32-S3-WROOM-1-MCN16R8  | 16Mb  | 8Mb   | 2 x 240Mhz  | 800x480                                 | 5.0"        | Direct            | [ST7701](assets/datasheets/ST7701S.pdf)  | SPI                | [XPT2046](assets/datasheets/XPT2046.pdf)  |                                           |                                                |      |                                           |        | [Ali Express](https://www.aliexpress.com/item/1005005938915207.html)  |
| ESP32-8048S070N   | USB-C     | ESP32-S3-WROOM-1-MCN16R8  | 16Mb  | 8Mb   | 2 x 240Mhz  | [800x480](assets/lcd/JC8048B070N.pdf)   | 7.0"        | Direct            | [ST7701](assets/datasheets/ST7701S.pdf)  |                    |                                           |                                           |                                                |      |                                           |        | [Ali Express](https://www.aliexpress.com/item/1005005928865239.html)  |
| ESP32-8048S070C   | USB-C     | ESP32-S3-WROOM-1-MCN16R8  | 16Mb  | 8Mb   | 2 x 240Mhz  | [800x480](assets/lcd/JC8048B070N.pdf)   | 7.0"        | Direct            | [ST7701](assets/datasheets/ST7701S.pdf)  | I2C                | [GT911](assets/datasheets//GT911.pdf)     |                                           |                                                |      |                                           |        | [Ali Express](https://www.aliexpress.com/item/1005005928865239.html)  |
| ESP32-4848S040C   | micro USB | ESP32-S3-WROOM-1-MCN16R8  | 16Mb  | 8Mb   | 2 x 240Mhz  | 240x240                                 | 4.0"        | Direct            | [ST7701](assets/datasheets/ST7701S.pdf)  | I2C                | [GT911](assets/datasheets//GT911.pdf)     | [NS4168](assets/datasheets/NS4168.pdf)    |                                                | yes  |                                           | 1-3    | [Ali Express](https://www.aliexpress.com/item/1005006320253803.html)  |

>[!IMPORTANT]
>The additional flash chip (W25Q32JV) is not always mounted on the board.

Besides the normal PlatformIO defines, there are the defines below.

The table below provides some explanation of the variable names. These definitions might still be incomplete.

| Define                              | Explanation                                                     |
|---                                  |---                                                              |
| ESP32_wwhhS0ddN/R/C                 | The board name, e.g. 2423S012C                                  |
|                                     |                                                                 |
| BOARD_HAS_PSRAM                     | The boards has PSRAM                                            |
|                                     |                                                                 |
| BUTTON_BOOT_GPIO                    | GPIO of the BOOT pushbutton                                     |
|                                     |                                                                 |
| LCD_USES_ST7789                     | LCD uses the ST7789 display driver                              |
| LCD_USES_GC9A01                     | LCD uses the GC9A01 display driver                              |
| LCD_USES_ILI9341                    | LCD uses the ILI9341 display driver                             |
| LCD_USES_DIRECT_IO                  | LCD uses direct IO with the display                             |
|                                     |                                                                 |
| LCD_WIDTH                           | The width of the LCD panel in pixels                            |
| LCD_HEIGHT                          | The height of the LCD panel in pixels                           |
| LCD_BCKL_GPIO                       | GPIO of the backlight                                           |
| LCD_SPI_HOST                        | The SPI host to use for the LCD driver                          |
| LCD_SPI_BUS_CONFIG                  | The LCD SPI BUS configuration                                   |
| LCD_IO_SPI_CONFIG                   | The LCD IO SPI configuration                                    |
| LCD_PANEL_DEV_CONFIG                | The LCD panel device configuration                              |
| LCD_RGB_PANEL_CONFIG                | The LCD panel settings for LV_COLOR_16_SWAP = 0                 |
| LCD_RGB_PANEL_CONFIG_COLOR_16_SWAP  | The LCD panel settings for LV_COLOR_16_SWAP = 1                 |
| LCD_SWAP_XY                         | Swap the X and Y axes for the panel                             |
| LCD_MIRROR_X                        | Mirror the panel horizontally                                   |
| LCD_MIRROR_Y                        | Mirror the panel vertically                                     |
| LCD_GAP_X                           | The horizontal gap in pixels before the panel                   |
| LCD_GAP_Y                           | The vertical gap in pixels before the panel                     |
|                                     |                                                                 |
| BOARD_HAS_TOUCH                     | The panel has a touch interface                                 |
| TOUCH_USES_GT911                    | Touch uses the GT911 capacitive touch controller                |
| TOUCH_USES_CST816S                  | Touch uses the CST816S capacitive touch controller              |
| TOUCH_USES_XPT2046                  | Touch uses the XPT2046 resistive  touch controller              |
|                                     |                                                                 |
| TOUCH_I2C_HOST                      | The I2C host to use for the touch controller                    |
| TOUCH_I2C_CONFIG                    | The touch I2C configuration                                     |
| TOUCH_IO_I2C_CONFIG                 | The touch IO I2C configuration                                  |
| TOUCH_DEV_CONFIG                    | The touch device configuration                                  |
| TOUCH_SWAP_X                        | Swap the touch horizontally                                     |
| TOUCH_SWAP_Y                        | Swap the touch vertically                                       |
|                                     |                                                                 |
| BOARD_HAS_TF                        | The board has a TF slot                                         |
| TF_CS_GPIO                          | GPIO of the CS of the TF slot                                   |
| TF_MOSI_GPIO                        | GPIO of the MOSI of the TF slot                                 |
| TF_SCLK_GPIO                        | GPIO of the SCLK of the TF slot                                 |
| TF_MISO_GPIO                        | GPIO of the MISO of the TF slot                                 |
|                                     |                                                                 |
| BOARD_HAS_RGB_LED                   | The board has an RGB led                                        |
| LED_R_GPIO                          | GPIO of the red LED                                             |
| LED_G_GPIO                          | GPIO of the green LED                                           |
| LED_B_GPIO                          | GPIO of the blue LED                                            |
|                                     |                                                                 |
| BOARD_HAS_CDS                       | The board has a CdS resistive light resistor                      |
| CDS_GPIO                            | Analogue GPIO input of the CdS sensor                           |
|                                     |                                                                 |
| BOARD_HAS_SPEAK_GPIO                | The board has an onboard amplifier for a speaker                |
| SPEAK_GPIO                          | GPIO of the speaker                                             |
|                                     |                                                                 |
| BOARD_HAS_RELAYS                    | The board has replays                                           |
| RELAY_BASE_GPIO                     | The GPIO of the first relay (next is one higher)                |