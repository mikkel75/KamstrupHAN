# Kamstrup Omnipower HAN module with ESP8266

<img src="https://raw.githubusercontent.com/mikkel75/KamstrupHAN/main/20211109_093016.jpg" width="400"> <img src="https://raw.githubusercontent.com/mikkel75/KamstrupHAN/main/3d_model_v.1.2.PNG" width="400">
<img src="https://user-images.githubusercontent.com/22839537/136014923-615aa680-3982-4fa3-96f8-aa7382944311.PNG">

HAN module for Kamstrup Omnipower based on ESP8266

The design is done with EasyEDA and PCB produced by JLCPCB (https://jlcpcb.com/). 10 pcs 2 layer is ~4US$ !

Once you have the mounted PCB - the process is very easy

1) Connect a USB<>UART 3.3V dongle to your PC
2) Connect the UART RX, TX and GND to the HAN module
   - Remember to put ESP in prog mode using TPs on the PCB
4) Flash eg. this nice SW: https://github.com/gskjold/AmsToMqttBridge
   - You can find compiled .bin's under 'tags'
   - I use the ESPEasy flasher for Windows, but you could also use esptools
6) Configure AmsToMqtt to use Omnipower and GPIO 13, remember AES keys if used.
   - AmsToMqtt has nice Domoticz support as well as raw/JSON MQTT.
8) Enjoy!
