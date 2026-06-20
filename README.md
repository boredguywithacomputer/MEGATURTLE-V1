  # MEGATURTLE-V1
An ESP32-S3 based custom drone flight controller that is a part of a bigger project. This is not the entire project, but is the only part that needs funding. 

<a href='https://epicturtle.web.app/demoflightcontroller/'>Here's a link to a demo</a>

It features
- 4 connectors for each individual ESC of my quadcopter
  -  One ESC will supply 5v for the flight controller
- A voltage divider setup that enables measurement of the LiPo battery's voltage and capacity
- An ESP32-S3 Wroom-1 microcontroller
- An IMU consisting of Bosch's BMI270 + BMM150, and an BMP388 Barometer
- Sockets to mount an NRF24L01 module

Note:
DRC says the courtyard two header pins overlap with those of the ESP32's antenna, but I ignored it since I won't need wireless connectivity. 

# Schematic

<img width="1231" height="837" alt="image" src="https://github.com/user-attachments/assets/370dc759-532c-4d35-b968-9cd067dcea00" />


# Board
<img width="807" height="809" alt="image" src="https://github.com/user-attachments/assets/7df504fb-e048-4566-a350-dfd11ed9b367" />
<br>
<img width="807" height="809" alt="image" src="https://github.com/user-attachments/assets/680bc4a4-d9a7-41ab-87a8-83ccb70f230c" />
<img width="508" height="477" alt="image" src="https://github.com/user-attachments/assets/242d1140-f8c8-4fe3-996c-7235d743b7bd" />
