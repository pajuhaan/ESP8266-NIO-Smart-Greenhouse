# Smart Greenhouse by NIO + ESP8266 

With this sample you can connect and control LEDs and Electrical valves by ESP8266 (NodeMCU - Arduino) via Wi-Fi in your Android devices. 

Android application can created by NIO as simple applets.

Get NIO from this link: http://niomatic.com


### Schematic:
![alt text](https://github.com/pajuhaan/ESP8266-NIO-Smart-Greenhouse/blob/master/Schematic/wifi-nio-nodemcu-esp8266-Greenhouse.jpg?raw=true)

Implement web socket server in an ESP8266. Command send from NIO to ESP in the JSON structure via Websocket.

Parse Json:
```javascript
JsonObject &root = jsonBuffer.parseObject(payload);
bool led_mod          = root["led"];
bool water_mode    = root["water"];
```

### NIO Back Panel:
![alt text](https://github.com/pajuhaan/ESP8266-NIO-Smart-Greenhouse/blob/master/Schematic/BackPanel.png?raw=true)

### NIO File:
Download esp8266 greenhouse.nio and open in your tablet.