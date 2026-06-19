  # MEGATURTLE-V1
An ESP32-S3 based custom drone flight controller that is a part of a bigger project. This is not the entire project, but is the only part that needs funding. 

<a href='https://epicturtle.web.app/fc/'>Here's a link to a demo</a>

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
<img width="909" height="840" alt="image" src="https://github.com/user-attachments/assets/2ef6d172-c325-4605-87c5-f8080c4f36b3" />
<br>
<img width="713" height="722" alt="image" src="https://github.com/user-attachments/assets/e8057072-8888-4cde-b9ab-2839fc4da7e9" />
<img width="505" height="451" alt="image" src="https://github.com/user-attachments/assets/f45b4877-69fb-4ce9-8885-00afc8e449be" />
