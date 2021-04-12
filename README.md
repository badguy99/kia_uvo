I have baked a custom integration for EU Kia Uvo, this will be working for new account types. Thanks for your hard work [@wcomartin](https://github.com/wcomartin/kiauvo). This project was mostly inspired by his [home assistant integration](https://github.com/wcomartin/kia_uvo)

Warning ahead; this is pre-alpha phase, please do not expect something fully functional, I will improve the integration by time.

You can install this either manually copying files or using HACS. Configuration can be done on UI, you need to enter your username and password, (I know, translations are missing!). 

- it will only fetch values for the first car, I am not sure if there are people outside using Kia Uvo with multiple cars :)
- update - It will fetch the cached information every 30 minutes from Kia Servers.
- force update - It will ask your car for the latest data every 2 hours. 
- It will not force update between 10PM to 6AM. I am trying to be cautios here.

Supported entities;
- Air Conditioner Status, Defroster Status
- Car Battery Level (12v), EV Battery Level
- Tire Pressure Warnings (individual and all)
- Charge Status and Plugged In Status
- Low Fuel Light Status (for PHEV and IC)
- Doors, Trunk and Hood Open/Close Status
- Locking and Unlocking
- Engine Status
- Location (over GPS)
- Odometer, EV Range (for PHEV and EV), Fuel Range (for PHEV and IC), Total Range (for PHEV and EV)
- Last Update

Supported service;
- force_update: this will make a call to your vehicle to get its latest data, do not overuse this!
- update: get latest **cached** vehicle data

I have posted an example screenshot from my own car.

![Device Details](https://github.com/fuatakgun/kia_uvo/blob/master/Device%20Details.PNG?raw=true)
