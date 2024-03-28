# Natacha
Compteur numérique belge via le port P1 avec Home Assistant et ESPHome

## ORES S211 M22/0071 Siconia
AAA ![aaa](https://github.com/rserroyen/Natacha/blob/main/img/Ores_1.png)
![Cover](https://github.com/rserroyen/Natacha/blob/main/img/Ores_2_pin.png).

## Physical port
![Cover](https://github.com/rserroyen/Natacha/blob/main/img/Physical_port_pinout.png).
![Cover](https://github.com/rserroyen/Natacha/blob/main/img/Physical_port.png).

## D1 MINI MINI PRO ESP8266
Connect the esp8266 to an RJ11 cable/connector following the diagram.

P1 pin	ESP8266 Pin

1 - +5v

2 - RTS	to 10k to 3.3v

3 - GND	

4 -	

5 - RXD (data)

6 - GND

![Cover](https://github.com/rserroyen/Natacha/blob/main/img/Schematic_Natacha-P1-Home-Assistant_2024-03-28.pdf).

# Home Assistant et ESPHome natacha.yaml
DSMR 4.0/4.2

115200 8N1:

Baudrate = 115200

Data bits = 8

Parity = None

Stop bits = 1

serial RS422

  uart:
  
  id: uart_bus

  rx_pin: 
  
    number: RX
    
    inverted: true
    
  baud_rate: 115200
  
  #data_bits: 7
  
  #parity: EVEN
  
  #stop_bits: 1
  
  rx_buffer_size: 1700

  inversé (Facultatif, booléen) : Si toutes les valeurs lues et écrites doivent être traitées comme inversées. La valeur par défaut est false.

# Link
Home-Assistant
https://github.com/DavyLandman/p1-esp8266
https://www.home-assistant.io/integrations/dsmr
Esphome
https://github.com/mmakaay/dsmr-reader-for-esphome
https://github.com/daniel-jong/esp8266_p1meter
https://esphome.io/components/sensor/dsmr.html?highlight=p1+port
https://github.com/mmakaay/dsmr-reader-for-esphome?tab=readme-ov-file
https://github.com/scheric/DSMR-P1-ESP-Home-Assistant/tree/master1-ESP-Home-Assistant
https://github.com/psvanstrom/esphome-p1reader
https://esphome.io/components/sensor/dsmr.html?highlight=p1+port
https://esphome.io/guides/configuration-types.html
https://esphome.io/components/sensor/dsmr.html
https://forum.hacf.fr/t/compteurs-electrique-belge-port-p1-sur-home-assistant/231

https://www.domohab.be/compteur-belge-recuperer-les-donnees-avec-home-assistant-et-esphome/
Domoticz
https://domoticx.com/p1-poort-slimme-meter-hardware/#
https://github.com/Raeymeister/BelgianSmartMeter2Domoticz?tab=readme-ov-file
https://www.youtube.com/watch?v=XpUMwQLgd2I
esp32
https://domoticx.com/p1-poort-slimme-meter-hardware/
Esp8266
https://github.com/daniel-jong/esp8266_p1meter
https://github.com/pkoerber/P1-Energy-Meter-Reader  P1-Energy-Meter-Reader 
https://github.com/UdoK/esp8266_p1meter_sv esp8266_p1meter_sv
https://www.weigu.lu/microcontroller/smartyReader_P1/index.html
https://github.com/jantenhove/P1-Meter-ESP8266
https://github.com/DavyLandman/p1-esp8266
https://github.com/daniel-jong/esp8266_p1meter/tree/master
https://github.com/sandervandegeijn/P1-Meter-ESP8266-MQTT
python
https://github.com/jensdepuydt/belgian_digitalmeter_p1
https://github.com/Josverl/micropython-p1meter
https://github.com/nrocco/smeterd
https://github.com/Eraser3/HomeWizard-Wifi-p1-plugin
https://github.com/rroethof/p1reader
PI
https://gejanssen.com/howto/Slimme-meter-uitlezen/
Doc
https://www.fluvius.be/sites/fluvius/files/2020-01/dmk-demo-v2.1-rtc.pdf
http://www.esp8266thingies.nl/wp/
https://blog.regout.info/category/slimmeter/



