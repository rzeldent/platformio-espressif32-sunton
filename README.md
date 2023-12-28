# Sunton CYD (Cheap Yellow Display) Board definitions

## This repo contains the definitions for the CPU and board information about the hardware available and how connected

Besides the normal PlatformIO defines, there are the defines below.

The table below provides some explanation of the variable names. These definitions might still be incomplete.

| Define                              | Explanation                                                     |
|---                                  |---                                                              |
| ESP32_wwhhS0ddN/R/CxR               | The board name, e.g. 2423S012C                                  |
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
| NUM_RELAY                           | The number of relays present on the board                       |
| RELAY_BASE_GPIO                     | The GPIO of the first relay (next is one higher)                |