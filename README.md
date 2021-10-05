![Board rev. 1.1](https://raw.githubusercontent.com/mikkel75/KamstrupHAN/main/3d_model.PNG)

# Kamstrup Omnipower HAN module with ESP8266

HAN module for Kamstrup Omnipower based on ESP8266

The design is done with EasyEDA and PCB produced by JLCPCB (https://jlcpcb.com/). 10 pcs 2 layer is ~4US$ !

Once you have the mounted PCB - the process is very easy

1) Connect a USB<>UART 3.3V dongle to your PC
2) Connect the UART RX, TX and GND to the HAN module (remember to put ESP in prog mode using TPs on the PCB)
3) Flash eg. this nice SW: https://github.com/gskjold/AmsToMqttBridge
3.1) You can find compiled .bin's under 'tags'
3.2) I use the ESPEasy flasher for Windows, but you could also use esptools
4) Configure AmsToMqtt to use Omnipower and GPIO 13, remember AES keys if used.
5) Enjoy!

