# mmc

 
Project Title:save data with Real time clock in SD Card .
Name: Mostafa Kahlil Ahmed.
Email:Mostafa.elsherif1995@gamail.com.


Hardware:
MCU-----------Atmega32         Sensor---------------DHT22
RTC-------------DS1307       Memory: Micro SD based on Fat32
Other: RGB LED, Resistors, Buttons, crystals, and battery.
Software:
Atmel Studio----------for coding Atmega32.
Proteuse8 professional for simulation all project.
WinImage---------------for virtual SD.

Main Output:
This project used to read data from sensor (temperature and humidity) and save data with Real time clock in SD Card.
 Image:
 
Project description:
Project working in two in two mode:
Firstly (Interface Mode):
-When switch Button (PinA4) be ON 
It give user selection in serial transfer to deal with all data like getting data , update time or date ,create file ,Delete file , and read file .
-this mode is very important to update date or time of RTC or read all file and data without use SD-Card out of Circuit. 
Secondly (Working Mode):
-When switch Button (PinA4) be OFF.
-MCU will Read data automatic and save it with file 
Every 5 minute (less for test) the will take name of “MOST” + day in number and month in number like 
In 03/08/2021 the data will save in file “MOST0308.CSV”.
-the MCU will create file for the day date of reading in excel sheet and append all date of day in same file.
Error and led (RGB led):
-If MCU in Interface Mode it will give Blue color.
-If MCU in Working Mode it will give Green color.
-If ERROR occur it will give red color and Stop working.
Finally:
-this project can worked with any type of Controller LIKE Microcontroller depended on arm cortex m4.






Appendix:
Clock Atmega32: External clock =8000000 Hz.
Baud rate Serial interface =1000000 bit/s.
Clock of I2C:100 KHz----bit rate=18.
SPI: High speed =4000000Hz.











