ssd1306-control-panel
============
http://elegantcircuits.com/2014/08/25/ssd1306-control-panel/

An example of an "instrument display" using SSD1306 OLED with an AVR microcontroller. Potentiometer captures user "input" (any type of setting) and displays on OLED

Runs on Atmega328P AVR Microcontroller at 8MHz (CLKDIV 8 fuse disabled for quicker refresh)

CLK = 8MHZ
avrdude -p atmega328p -P /dev/ttyUSB0 -c avrisp -b 19200 -B 1 -U lfuse:w:0xe2:m -U hfuse:w:0xd9:m -U efuse:w:0xff:m 

Enable CKDIV8 fuse
avrdude -p atmega328p -P /dev/ttyUSB0 -c avrisp -b 19200 -B 1 -U lfuse:w:0x62:m -U hfuse:w:0xd9:m -U efuse:w:0xff:m 
