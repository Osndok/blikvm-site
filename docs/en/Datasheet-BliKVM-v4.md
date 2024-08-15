# BliKVM v4 Allwinner (H616/H313 SOC)

 ![Main](assets/images/v4/Datasheet-BliKVM-v4.assets/Main.png){width="400"}

BliKVM is a production-ready, plug and play KVM-over-IP device that offers professional users a convenient solution **for remote server or workstation management**. It is based on Linux and fully open source. With BliKVM, you can easily **power on/off, restart your computer, configure UEFI/BIOS settings, and perform OS reinstallation using an emulated Mass Storage Device**. BliKVM simulates a keyboard, mouse, and monitor, all accessible through a web browser, ensuring a seamless user experience. **Its hardware-level access guarantees independence from specific remote ports, protocols, or services**, making it a highly flexible and reliable remote management solution for professionals!

## **Connectivity Diagram**

![Interface-Layout-Diagram](assets/images/v4/Datasheet-BliKVM-v4.assets/Interface-Layout-Diagram.png)

| 1 | USB 2.0 port             | 10   | Antenna interface             |
| ----- | ------------------------------- | ---- | ----------------------------- |
| 2     | Power Input 5V 3A & UART        | 11   | RJ45 100M Ethernet port & PoE |
| 3     | RJ45 ATX control port           | 12   | Display 1.33 inch LCD         |
| 4     | HDMI video loop through port | 13   | Power LED (red)             |
| 5     | USB-PC port                     | 14   | User defined button SW1       |
| 6     | Power Input 12V 2A 5.5*2.1mm    | 15   | ACT LED (green) |
| 7     | HDMI video input port           | 16 | Display ON/OFF button         |
| 8     | HDMI input status LED (green)  | 17   | Micro SD card slot            |
| 9     | HDMI output status LED (yellow) |      |                               |

## **Specifications**

![Topology-Diagram](assets/images/v4/Datasheet-BliKVM-v4.assets/Topology-Diagram.png)

| Parameter name              | Characteristics                                              |
| --------------------------- | ------------------------------------------------------------ |
| **Power**                   |                                                              |
| 5V 3A                       | 5V port, USB-PC port                                         |
| 12V 2A                      | 12V port                                                     |
| PoE                         | Power over Ethernet (IEEE802.3af compliant)  48V DC          |
|                             |                                                              |
| **Connectivity/Interfaces** |                                                              |
| HDMI-IN                     | HDMI video input port                                        |
| HDMI-OUT                    | HDMI video loop through port                                 |
| USB-PC                      | Keyboard, mouse, mass storage, and other external device emulation) |
| ATX                         | Turn on/off or restart the controlled computer               |
| WiFi & Bluetooth            | IEEE802.11 b/g/n + BLE4.2                                    |
| Micro SD card slot          | Persistent storage for OS and your data                      |
| 5V port                     | 5V 3A power or serial console management port                |
|                             |                                                              |
| **Displays and indicators** |                                                              |
| LED indicators              | Power LED, ACT LED, HDMI input status LED (green)， HDMI output status LED (yellow) |
| LCD display                 | LCD 240x240 1.33 inch                                        |
| User defined button         | SW1                                                          |
| Buzzer                      | Find me                                                      |
|                             |                                                              |
| **Video**                   |                                                              |
| Supported resolutions       | Up to 4k@30Hz                                                |
| Video compression methods   | MJPEG                                                        |
|                             |                                                              |
| **Core**                    |                                                              |
| Chip                        | ALLWINNER H616/H313                                               |
| RAM                         | 1GB                                                          |
|                             |                                                              |
| **Power consumption**       | Up to 15W                                                    |
|                             |                                                              |
| **Environmental**           |                                                              |
| Operating temperature       | 0°C to 70°C                                                  |
| Storage temperature         | -20°C to 60°C                                                |
|                             |                                                              |
| **Dimensions and weight**   |                                                              |
| Size                        | 100 (L) x 134 (W) x 44.4 (H) mm                              |
| Weight                      | 0.45 kg                                                      |

!!! info "BLIKVM CM4 version OLED display"
    The product comes standard with a monochrome OLED display with a resolution of 128x64, and the chip is SSD1306.  
    The user connects the display to the product with the wiring of the display.

    ![Image title](assets/images/oled/BLIKVM-CM4-oled.png){width="300"}

    The module is connected to CM4 through the I^2^C interface. The wiring definition is shown in the following table. 
    This is a library for the monochrome OLEDs based on [SSD1306 drivers.](https://github.com/adafruit/Adafruit_SSD1306)

    | Display(SSD1306) | CM4               |
    | ---------------- | ----------------- |
    | GND              | GND               |
    | VCC              | 3.3V              |
    | SCL              | GPIO3(SCL1,I^2^C) |
    | SDA              | GPIO2(SDA1,I^2^C) |

## **Dimensions Schematic Diagram**

![Dimensions](assets/images/v4/Datasheet-BliKVM-v4.assets/Dimensions.png){width="400"}
