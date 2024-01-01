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

## Board defines

Besides the normal PlatformIO defines, there are the defines below that allow to make software for all these boards using only one source.
This is used by the [esp32-smartdisplay](https://github.com/rzeldent/esp32-smartdisplay) project to have one abstraction for these boards.

The table below provides some explanation of the variable names. These definitions might still be incomplete.

| Define                              | Explanation                                                     |
|---                                  |---                                                              |
| ESP32_wwhhS0ddN/R/C                 | The board name, e.g. 2423S012C                                  |
|                                     |                                                                 |
| BOARD_HAS_PSRAM                     | The boards has PSRAM                                            |
|                                     |                                                                 |
| BUTTON_BOOT                    | GPIO of the BOOT pushbutton                                     |
|                                     |                                                                 |
| LCD_USES_ST7789                     | LCD uses the ST7789 display driver                              |
| LCD_USES_GC9A01                     | LCD uses the GC9A01 display driver                              |
| LCD_USES_ILI9341                    | LCD uses the ILI9341 display driver                             |
| LCD_USES_DIRECT_IO                  | LCD uses direct IO with the display                             |
|                                     |                                                                 |
| LCD_WIDTH                           | The width of the LCD panel in pixels                            |
| LCD_HEIGHT                          | The height of the LCD panel in pixels                           |
| BCKL                                | GPIO of the backlight                                           |
| type_SPI_HOST                       | The SPI host to use for the LCD driver                          |
| type_SPI_MOSI                       | SPI                                                             |
| type_SPI_MISO                       | SPI                                                             |
| type_SPI_SCLK                       | SPI                                                             |
| type_CS                             |                                                                 |
| type_DC                             |                                                                 |
| type_RST                            |                                                                 |
|                                     |                                                                 |
| IO_HSYNC_PULSE_WIDTH                | Direct IO                                                       |
| IO_HSYNC_BACK_PORCH                 | Direct IO                                                       |
| IO_HSYNC_FRONT_PORCH                | Direct IO                                                       |
| IO_VSYNC_PULSE_WIDTH                | Direct IO                                                       |
| IO_VSYNC_BACK_PORCH                 | Direct IO                                                       |
| IO_VSYNC_FRONT_PORCH                | Direct IO                                                       |
| IO_HSYNC                            | Direct IO                                                       |
| IO_VSYNC                            | Direct IO                                                       |
| IO_DE                               | Direct IO                                                       |
| IO_PCLK                             | Direct IO                                                       |
| IO_R0                               | Direct IO                                                       |
| IO_R1                               | Direct IO                                                       |
| IO_R2                               | Direct IO                                                       |
| IO_R3                               | Direct IO                                                       |
| IO_R4                               | Direct IO                                                       |
| IO_G0                               | Direct IO                                                       |
| IO_G1                               | Direct IO                                                       |
| IO_G2                               | Direct IO                                                       |
| IO_G3                               | Direct IO                                                       |
| IO_G4                               | Direct IO                                                       |
| IO_G5                               | Direct IO                                                       |
| IO_B0                               | Direct IO                                                       |
| IO_B1                               | Direct IO                                                       |
| IO_B2                               | Direct IO                                                       |
| IO_B3                               | Direct IO                                                       |
| IO_B4                               | Direct IO                                                       |
|                                     |                                                                 |
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
| type_I2C_HOST                       | The I2C host to use for the touch controller                    |
| type_I2C_SDA                        | I2C                                                             |
| type_I2C_SCL                        | I2C                                                             |
| type_RST                            | I2C                                                             |
| type_INT                            | I2C                                                             |
|                                     |                                                                 |
| type_SPI_HOST                       | SPI                                                             |
| type_SPI_MOSI                       | SPI                                                             |
| type_SPI_MISO                       | SPI                                                             |
| type_SPI_SCLK                       | SPI                                                             |
| type_CS                             |                                                                 |
| type_DC                             |                                                                 |
| type_RST                            |                                                                 |
| type_INT                            |                                                                 |
|                                     |                                                                 |
| TOUCH_SWAP_X                        | Swap the touch horizontally                                     |
| TOUCH_SWAP_Y                        | Swap the touch vertically                                       |
|                                     |                                                                 |
| BOARD_HAS_TF                        | The board has a TF slot                                         |
| TF_CS                               | GPIO of the CS of the TF slot                                   |
| TF_SPI_MOSI                         | GPIO of the MOSI of the TF slot                                 |
| TF_SPI_SCLK                         | GPIO of the SCLK of the TF slot                                 |
| TF_SPI_MISO                         | GPIO of the MISO of the TF slot                                 |
|                                     |                                                                 |
| BOARD_HAS_RGB_LED                   | The board has an RGB led                                        |
| RGB_LED_R                           | GPIO of the red LED                                             |
| RGB_LED_G                           | GPIO of the green LED                                           |
| RGB_LED_B                           | GPIO of the blue LED                                            |
|                                     |                                                                 |
| BOARD_HAS_CDS                       | The board has a CdS resistive light resistor                    |
| CDS                                 | Analogue GPIO input of the CdS sensor                           |
|                                     |                                                                 |
| BOARD_HAS_SPEAK                     | The board has an onboard amplifier for a speaker                |
| SPEAK                               | GPIO of the speaker                                             |
|                                     |                                                                 |
| BOARD_HAS_RELAYS                    | The board has replays                                           |
| RELAY_BASE                          | The GPIO of the first relay                                     |






## PSRAM

At boot the ESP32 has approx 315Kb usable memory (from the 520Kb present). Displays with a controller do not have an internal frame buffer to save the state of the display. However, if the display is using the direct 16bits parallel connection, there is no controller and the contents of the RAM is copied to the display at a fast rate. This buffer is allocated from the memory of the ESP32.

If using the normal SRAM, this would (for the ESP32_4827S043 with a 480x270 pixels) snoop away 480x270x2 = 261120 bytes, leaving only 54140 bytes for the application. This can be done and works.
However, the other boards with a resolution of 800x480, 800x480x2 = 768000 bytes are required. This is more than the available RAM.

This is the reason for boards with a direct 16bits parallel connection 8Mb of PSRAM is added and should be used to store this buffer.

The standard definition of the ```esp32-s3-devkitc-1.json``` does not have any configuration for the increases flash size and PSRAM. This is corrected in the board definitions.

## Controlling the RGB led

>[!NOTE]
>Not all boards have a LED. Refer to the [supported boards](#supported-boards) to see if this is available.

If the board has an RGB led, the define ```BOARD_HAS_RGB_LED``` is defined.
Additionally, the following defines are present for the definition of the GPIO pins:

- RGB_LED_R
- RGB_LED_G
- RGB_LED_B

Before using the RGB LEDs, the GPIOs must be defined as output. This is already done in the [smartdisplay_init()](#void-smartdisplay_init) function.

```c++
  pinmode(RGB_LED_R, OUTPUT);
  pinmode(RGB_LED_G, OUTPUT);
  pinmode(RGB_LED_B, OUTPUT);
```

The LEDs are connected between the GPIO pin and the 3.3V. So the LED will light up if the GPIO is set to LOW (inverted).

For example: set the RGB led to red is done by the following code:

```c++
  digitalWrite(RGB_LED_R, false);
  digitalWrite(RGB_LED_G, true);
  digitalWrite(RGB_LED_B, true);
```

To have more colors than the 8 RGB combinations, PWM can be used to mix the colors.
To do this, attach a PWM channel to each GPIO pin to modulate the intensity.

>[!WARNING]
>The number of PWM channels is limited and some channels are reserved for some functions
>e.g. channel 0 is used by the tone() function but can be used if this function is not called.

Example:
Set PWM channel 0 to 5000Hz with a resolution of 8 bits (256 levels) and attach it to the red LED.
Next, set the level to 25%. This is 192 (256 - 25%) because of the inverted output.

>[!CAUTION]
>The functions for using PWM will change in the upcoming release of the IDF and will break the usage of the PWM functions!

ESP_ARDUINO_VERSION_MAJOR < 3:

```c++
  ledcSetup(0, 5000, 8);
  ledcAttachPin(RGB_LED_R, 0);
  ledcWrite(0, 192);
```

ESP_ARDUINO_VERSION_MAJOR >= 3

```c++
  ledcAttach(RGB_LED_R, 0, 8);
  ledcWrite(RGB_LED_R, 192);
```

## Reading the CdS (light sensor)

>[!NOTE]
>Not all boards have a light sensor. Refer to the [supported boards](#supported-boards) to see if this is available.

If the board has a CdS photo resistor (Cadmium Sulfide, CdS), the define ```BOARD_HAS_CDS``` is defined. It is attached to the analogue input of the ESP32 with two resistors between the GND and the VCC. When the CDS is covered, it's resistance is in the order of mega&Omega; but in bright light can drop to a few 1k&Omega;.

To use the sensor, the define ```CDS``` indicates the analogue port to read.
Setting the port to input and the attenuation is already done in the [smartdisplay_init()](#void-smartdisplay_init) function.

```c++
  analogSetAttenuation(ADC_0db); // 0dB(1.0x) 0~800mV
  pinMode(CDS, INPUT);
```

Next, read the value using:

```c++
  auto value = analogReadMilliVolts(CDS);
```

See the [GT36516](assets/datasheets/GT36516.pdf) specs:

- Dark = 0.3M&Omega;
- Light 5k&Omega;

Theory: The voltage is between 1.28V (dark) and 16mV (light).
The ESP32 has a threshold of ~15mV so below 15mV the value is 0.

## Controlling the speaker

>[!NOTE]
>Not all boards have a LED. Refer to the Refer to the [supported boards](#supported-boards) to see if this is available.

An 8&Omega; speaker can be connected to the output marked SPEAK. This is a 1.25 JST connector.
Setting the speaker GPIO to output is already done in the [smartdisplay_init()](#void-smartdisplay_init) function.

```c++
pinmode(SPEAK, OUTPUT)
```

Beeps can be generated by generating a PWM signal on the SPEAK or using the tone function:

```c++
// Uses PWM Channel 0
tone(SPEAK, frequency, duration);
```

To produce "real" audio connect the internal 8 bits D2A converter in the ESP32. Because the speaker is connected to GPIO26, this is the DAC2 (Left Channel).

>[!TIP]
>Make sure the I2S connection is only to the LEFT channel. GPIO25, the right channel, is connected on some boards to the GT911 touch controller and creates strange results.

The audio is a bit distorted. [HexeguitarDIY](https://github.com/hexeguitar/ESP32_LCD_PIO) has a fix for that by changing the resistor values to prevent distortion.
[![HexeguitarDIY Audio mod](https://img.youtube.com/vi/6JCLHIXXVus/0.jpg)](https://www.youtube.com/watch?v=6JCLHIXXVus)

## Appendix: Board details

### ESP32_1732S019 N/C

- USB-C

### ESP32-2424S012 N/C

- USB-C
- I2C: 1 x SH1.0 4p
- Battery interface: JST1.25 2p

![ESP32-2424S012 front](assets/images/esp32-2424S012-front.png)
![ESP32-2424S012 back](assets/images/esp32-2424S012-back.png)

### ESP32-2432S024 N/R/C

- Micro USB
- I2C: 2 x JST1.25 4p
- Power + Serial: JST1.25 4p
- Speaker: JST1.25 2p

![ESP32-2432S024 front](assets/images/esp32-2432S024-front.png)

### ESP32-2432S028 R

- Micro USB
- I2C: 2 x JST1.25 4p
- Power + Serial: JST1.25 4p
- Speaker: JST1.25 2p

![ESP32-2432S028R back](assets/images/esp32-2432S028R-back.png)

### ESP32-3248S035

- Micro USB
- I2C: 2 x JST1.25 4p
- Power + Serial: JST1.25 4p
- Speaker: JST1.25 2p

![ESP32-3248S035 front](assets/images/esp32-3248S035-front.png)
![ESP32-3248S035 back](assets/images/esp32-3248S035-back.png)

### ESP32-4827S043

- USB-C
- I2C: JST1.25 4p
- Power + Serial: JST1.25 4p

![ESP32-4827S043 front](assets/images/esp32-4827S043-front.png)
![ESP32-4827S043 back](assets/images/esp32-4827S043-back.png)

### ESP32-8048S050

- USB-C
- I2C: JST1.25 4p
- Power + Serial: JST1.25 4p

![ESP32-8048S050 front](assets/images/esp32-8048S050-front.png)
![ESP32-8048S050 back](assets/images/esp32-8048S050-back.png)

### ESP32-8048S070

- USB-C
- I2C: JST1.25 4p
- Power + Serial: JST1.25 4p

![ESP32-8048S070 front](assets/images/esp32-8048S070-front.png)
![ESP32-8048S070 back](assets/images/esp32-8048S070-back.png)