# Lunarbie

![Lunarbie](Images/Lunarbie_PCB_bare.PNG)
The nighty companion of Starbie! Lunarbie is a tiny keychain sized board that acts like a little pet for your everyday carry.It is the counterpart to Starbie a starter project of the Hackclub Half-Life program

Heavily inspired by this Repo: [have a look](https://github.com/SharKingStudios/Starbie/tree/main)

# What is this

Lunarbie is a project, made for the [Half life](https://halflife.hackclub.com) by Hackclub programm. It is an alternation by earlier mentioned beginner project Starbie. The project itself is a tiny keychain sized board that acts like a pokemon styled pet. 

The Board features a Microcontroller, display, motion sensor, and environmental sensor in a compact PCB design. It is USB powered and easy to build. Its also moon shaped !

# Project status

The project is finished but it is still possible that some additions to this repo will be made, like CAD files or more features for the Lunarbie.

# Detailed description

Lunarbie is able to interact with its holder passively with its environmental and motion sensors or via the buttons on it. It can interact with the holder by changing its built in display. 
(Additionally it is able to detect another Lunarbie (or Starbie) when holding them at each other, similar to apples airdrop feature.)

# Motivation

The main motivation is of course the Half Life (LINK) program by hackclub. It was designed in week one of the project where the task was to create a custom PCB. Other than that, I really wanted to design a PCB for a long time now and it definitely won’t be my last one. It was really fun to design it and challenge me with a fun and beginnerfriendly project that could maybe even be continued.

# Project journaling

Via the [Half life](https://halflife.hackclub.com) by Hackclub programm, several Journal entries have been made either in timelaps form or as written entry to track the project. 

# Assembly

![Lunarbie](Images/Render.PNG)
The assembly should be quite beginnerfriendly. The board itself has not many part and is partly prefabricated. All remaining components are easy to be soldered by hand.

# Schematic and components

![Lunarbie](Images/Schematic.PNG)
The board is powered by the XIAO_ESP32C3. It provides the power and data connector with an onboard USB-receptacle. The board also features a MPU6050 motion sensor and an DHT11 environmental sensor. Furthermore it has an Display to broadcast emotions and expressions of the pet. For navigation of the Display and its features, there are two buttons on the board.

# PCB

![Lunarbie](Images/Routing.PNG)
The PCB is a simple 2 layer PCB with another silkscreen layer for cosmetic purposes. The board also has a GND pour and features routing on the front and backside.

closeup
![Lunarbie](Images/Routing_closeup.PNG)

# Firmware

The firmware is written in the ArduinoIDE and is contained in one singe .ino file. It has some additional features but mainly comes from the starbie repo mentioned above. The firmware can be easily flashed onto the ESP as long as the board has been downloaded in the IDE.

# BOM
The BOM can be viewed in the [BOM.csv](BOM.csv) file 

embedded too: 
Lunarbie – bill of materials
				
| Part | Qty | Unit | Total | Vendor |
| --- | --- | --- | --- |
| XIAO ESP32 C3 | 1 | Aliexpress | $11.33 | [ALIEXPRESS](https://www.aliexpress.com/item/1005007084388623.html?spm=a2g0o.cart.0.0.4a4838daq48qnZ&mp=1&pdp_npi=6%40dis%21USD%21USD%2011.36%21USD%2011.36%21%21USD%2011.36%21%21%21%40213297f617927060235196646e0d7e%2112000056349597200%21ct%21DE%21-1%21%211%210%21) |
| 0.96 OLED | 1 | Aliexpress | $2.57 | [ALIEXPRESS](https://www.aliexpress.com/item/1005009170035050.html?spm=a2g0o.cart.0.0.4a4838daq48qnZ&mp=1&pdp_npi=6%40dis%21USD%21USD%202.57%21USD%202.57%21%21USD%202.57%21%21%21%402127805117927049331983887e0e49%2112000048183387215%21ct%21DE%21-1%21%211%210%21) |
| MPU6050 | 1 | Aliexpress |  $3.61 | [ALIEXPRESS](https://www.aliexpress.com/item/32869974009.html?spm=a2g0o.cart.0.0.4a4838daq48qnZ&mp=1&pdp_npi=6%40dis%21USD%21USD%203.61%21USD%203.61%21%21USD%203.61%21%21%21%402127805117927049331983887e0e49%2165507493207%21ct%21DE%21-1%21%211%210%21) |
| DHT11 | 1 | Aliexpress | $2.05 | [ALIEXPRESS](https://www.aliexpress.com/item/1005008818897051.html?spm=a2g0o.cart.0.0.4a4838daq48qnZ&mp=1&pdp_npi=6%40dis%21USD%21USD%201.50%21USD%201.50%21%21USD%201.50%21%21%21%402127805117927062540226303e0e49%2112000046802736833%21ct%21DE%21-1%21%211%210%21) |
| MX Switches | 1 | Aliexpress | $3.60 | [ALIEXPRESS](https://www.aliexpress.com/item/1005006161274872.html?spm=a2g0o.cart.0.0.4a4838daq48qnZ&mp=1&pdp_npi=6%40dis%21USD%21USD%204.27%21USD%204.27%21%21USD%204.27%21%21%21%40213297f617927060235196646e0d7e%2112000036051057268%21ct%21DE%21-1%21%211%210%21&pdp_ext_f=%7B%22cart2PdpParams%22%3A%7B%22pdpBusinessMode%22%3A%22retail%22%7D%7D) |
| Keycaps | 2 | Aliexpress | $4.27 | [ALIEXPRESS](https://www.aliexpress.com/item/1005007482124353.html?spm=a2g0o.cart.0.0.4a4838daq48qnZ&mp=1&pdp_npi=6%40dis%21USD%21USD%201.80%21USD%201.80%21%21USD%201.80%21%21%21%40213297f617927060235196646e0d7e%2112000040968628728%21ct%21DE%21-1%21%212%210%21) |
| 10k Resistor | 1 | Aliexpress | $1.50 | [ALIEXPRESS](https://www.aliexpress.com/item/1005004698981340.html?spm=a2g0o.cart.0.0.4a4838daq48qnZ&mp=1&pdp_npi=6%40dis%21USD%21USD%202.05%21USD%202.05%21%21USD%202.05%21%21%21%402127805117927049331983887e0e49%2112000030143050818%21ct%21DE%21-1%21%211%210%21) |
| Total = $28.96 | Shipping = Free |
