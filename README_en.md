# FT232HL-to-JTAG Conversion Board

[日本語版](README.md)

This board converts the [FT232HL High-Speed USB Serial Converter Module](https://akizukidenshi.com/catalog/g/g106503/) from Akizuki Denshi for JTAG use.

It is mainly intended for use with my [USB 3.0 board for Tang Primer25K](https://github.com/ryuz/rtcl-tp25k-usb3-pcb).

![PCB image](images/pcb_image.png)

You no longer need to connect each wire one by one, which makes plugging and unplugging much easier.

![before_after](images/before_after.png)

## How to Use

For better usability during operation, silkscreen is also printed on the solder side. When soldering connectors, be careful not to confuse the front and back sides.

The side with reference labels such as J1/J2/J3 is the component side.

On the FT232HL High-Speed USB Serial Converter Module, short only JP3, and **always leave JP4 open**.

JP4 supplies I/O voltage, but this board is designed to receive voltage from the target board. If JP4 is connected, 3.3 V will also be supplied from the FT232HL side, which can cause a power rail conflict and may **damage the board**.

## Disclaimer

This design data is intended for research and development prototypes and experimental use. Please note that the author will not compensate for any damages arising from its use.

## License

This design data is provided under the [Creative Commons Attribution-NonCommercial 4.0 International License](https://creativecommons.org/licenses/by-nc/4.0/).

You may freely use it for hobby, research, and development purposes as long as you do not sell or distribute boards manufactured from this design without permission.

If you would like to manufacture and sell this board commercially, please contact the author separately to discuss a licensing agreement. You can get in touch via the [contact form](https://rtc-lab.com/contact/).

## Author

Ryuji Fuchikami  
[Real-Time Computing Lab.](https://rtc-lab.com/)
