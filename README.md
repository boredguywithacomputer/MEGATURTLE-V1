  # MEGATURTLE-V1
An ESP32-S3 based custom drone flight controller that is a part of a bigger project. This is not the entire project, but is the only part that needs funding. 

<a href='https://epicturtle.web.app/demoflightcontroller/'>Here's a link to a demo</a><br>
<a href='https://epicturtle.web.app/schemm.pdf'>PDF version of schematic</a>


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
<img width="1329" height="892" alt="image" src="https://github.com/user-attachments/assets/21705afb-79d2-404a-adfe-e3caec5f1668" />


# Board
<img width="807" height="809" alt="image" src="https://github.com/user-attachments/assets/7df504fb-e048-4566-a350-dfd11ed9b367" />
<br>
<img width="807" height="809" alt="image" src="https://github.com/user-attachments/assets/680bc4a4-d9a7-41ab-87a8-83ccb70f230c" />
<img width="508" height="477" alt="image" src="https://github.com/user-attachments/assets/242d1140-f8c8-4fe3-996c-7235d743b7bd" />

# Bill Of Materials
|Component                  |Total Price ($)|Part #                                                           |Link                                                                     |Qty|JLCPCB Part #|
|---------------------------|---------------|-----------------------------------------------------------------|-------------------------------------------------------------------------|---|-------------|
|22uF                       |0.472          |CL10A226MQ8NRNC                                                  |https://jlcpcb.com/partdetail/60514-CL10A226MQ8NRNC/C59461               |20 |C59461       |
|1uF                        |0.284          |CL05A105KA5NQNC                                                  |https://jlcpcb.com/partdetail/53938-CL05A105KA5NQNC/C52923               |20 |C52923       |
|10uF                       |0.524          |CL10A106KP8NNNC                                                  |https://jlcpcb.com/partdetail/20411-CL10A106KP8NNNC/C19702               |20 |C19702       |
|0.1uF                      |0.0868         |CL05B104KO5NNNC                                                  |https://jlcpcb.com/partdetail/1877-CL05B104KO5NNNC/C1525                 |28 |C1525        |
|LED                        |0.144          |KT-0603R                                                         |https://jlcpcb.com/partdetail/Hubei_KENTOElec-KT0603R/C2286              |20 |C2286        |
|BMP388                     |4.7298         |BMP388                                                           |https://jlcpcb.com/partdetail/BoschSensortec-BMP388/C779278              |2  |C779278      |
|BMI270                     |6.501          |BMI270                                                           |https://jlcpcb.com/partdetail/BoschSensortec-BMI270/C2836813             |2  |C2836813     |
|USB_C_Receptacle_USB2.0_14P|0.3686         |TYPE-C-31-M-12                                                   |https://jlcpcb.com/partdetail/Korean_HropartsElec-TYPE_C_31_M12/C165948  |2  |C165948      |
|Conn_01x03_Pin             |7.0924         |TSM-103-01-L-SV                                                  |https://jlcpcb.com/partdetail/Samtec-TSM_103_01_LSV/C6886650             |14 |C6886650     |
|Conn_01x03_Pin             |               |                                                                 |                                                                         |   |             |
|NRF24L01                   |0.3618         |PM254-2-04-S-8.5                                                 |https://jlcpcb.com/partdetail/HCTL-PM254_2_04_S_85/C3975149              |2  |C3975149     |
|10K                        |0.024          |0402WGF1002TCE                                                   |https://jlcpcb.com/partdetail/26487-0402WGF1002TCE/C25744                |20 |C25744       |
|100K                       |0.022          |0402WGF1003TCE                                                   |https://jlcpcb.com/partdetail/26484-0402WGF1003TCE/C25741                |20 |C25741       |
|5.1K                       |0.018          |0402WGF5101TCE                                                   |https://jlcpcb.com/partdetail/26648-0402WGF5101TCE/C25905                |20 |C25905       |
|33K                        |0.016          |0402WGF3302TCE                                                   |https://jlcpcb.com/partdetail/26522-0402WGF3302TCE/C25779                |20 |C25779       |
|1K                         |0.022          |0402WGF1001TCE                                                   |https://jlcpcb.com/partdetail/12256-0402WGF1001TCE/C11702                |20 |C11702       |
|SW_Push                    |0.4416         |TS-1088-AR02016                                                  |https://jlcpcb.com/partdetail/XUNPU-TS_1088AR02016/C720477               |8  |C720477      |
|ESP32-S3-WROOM-1           |9.6078         |ESP32-S3-WROOM-1-N8                                              |https://jlcpcb.com/partdetail/3198296-ESP32_S3_WROOM_1N8/C2913198        |2  |C2913198     |
|AMS1117                    |0.3944         |AMS1117-3.3                                                      |https://jlcpcb.com/partdetail/Advanced_MonolithicSystems-AMS1117_33/C6186|2  |C6186        |
|BMM150                     |3.1424         |BMM150                                                           |https://jlcpcb.com/partdetail/BoschSensortec-BMM150/C171681              |2  |C171681      |
|PCB Price                  |7              |                                                                 |                                                                         |   |             |
|Standard PCBA Setup        |25.56          |*board must be standard pcba because of some components I'm using|                                                                         |   |             |
|Stencil                    |8.21           |                                                                 |                                                                         |   |             |
|Total                      |75.0226        |                                                                 |                                                                         |   |             |
