# Serial-over-USB connection

The BliKVM device can be accessed through the serial port terminal.

!!! info "1. For hardware connection, you should use the USB to TTL module to connect the USB of the computer to the uart of BliKVM. If you are using the Hat version, please connect the serial ports GPIO14 and GPIO15. If you are using the PCIe version, connect the **GTR** pin marked by the PCB"
    ![rasp4b](assets/images/serial/rasp4b.png){width="300"}

!!! info "2. Install terminal login tools on the computer. For example, Putty for Windows"
    ![putty](assets/images/serial/putty.png){width="100"}

!!! info "3. Use the Putty instructions. Enter the correct COM port. The default baud rate is `115200`. Select serial as the connection method, and then click Open（Use PiKVM firmware as an example"
    ![putty_conf](assets/images/serial/putty_conf.png){width="300"}
    ![putty_ter01](assets/images/serial/putty_ter01.png){width="300"}
    ![putty_ter02](assets/images/serial/putty_ter02.png){width="300"}

!!! warning "If your computer cannot correctly recognize the USB to TTL module, please follow the steps below to install the driver for your computer"
    1. Connect the USB-A connector to your admin host (in this example, it's on a Windows host). As a result, Device Manager will show a new USB Serial device in Other Devices.
    ![drive-usb-serial](assets/images/serial/drive-usb-serial.png){width="300"}
    2. Download and extract/run drivers. In this example, I downloaded and extracted the ZIP file.
    https://learn.sparkfun.com/tutorials/how-to-install-ch340-drivers/all
    3. Update driver for the new USB Serial device, point it to where you extracted the files, and click Next then Close.  
    ![update-ch430-01](assets/images/serial/update-ch430-01.png){width="300"}
    ![update-ch430-02](assets/images/serial/update-ch430-02.png){width="300"}
    4. If done right, the new USB serial device should now show up under Ports as USB-SERIAL CH340 (COMX).
    ![drive-ch430](assets/images/serial/drive-ch430.png){width="300"}
