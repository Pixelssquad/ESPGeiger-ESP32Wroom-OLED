![Build](https://github.com/steadramon/ESPGeiger/workflows/Build/badge.svg?branch=main)
# <img src="https://raw.githubusercontent.com/steadramon/ESPGeiger/main/docs/img/ESPGeiger.svg" width="30px"/> ESPGeiger

ESPGeiger is a project for collecting, calculating and reporting from Geiger counters with a pulse output signal. Some serial counters are support, for example the GC10 range.
The firmware is written to be installed onto the common esp8266 and esp32 boards.

- 😃  Easy to install and configure - contribute to monitoring!
- 📈  Built in webserver with graphing
- 🔴  Live CPM and μSv/h readings
- 🔢  Smoothed and averaged values over 1, 5 and 15 minutes
- ✅  Compatible with generic Geiger counters with Pulse output and some serial based - GC10next (GC10 currently untested)
- 🎛️  Configurable filtering and noise control
- 📟  Accurate counting via interrupt and non-blocking functions. Hardware counter (ESP32 only - PCNT)
- 🌐  Upload and share statistics to services online and locally via MQTT

<img src="https://raw.githubusercontent.com/steadramon/ESPGeiger/main/docs/img/statuspage.png"/>

## Outputs
- MQTT
- ThingSpeak
- Radmon.org
- gmcmap.com

Planned:
- ESPGeiger API
- Async Webserver
- Display support

## Geiger counters

The project is compatible with Generic Pulse-based geiger counters and the GC10next serial based counters.

- [DIY GeigerKit](https://sites.google.com/site/diygeigercounter/)
- [NetIO GC10](https://www.ebay.co.uk/usr/pelorymate)
- [RHElectronics](https://www.rhelectronics.store/diy-geiger-counter-kit)
- [GeigerHV](https://www.ebay.co.uk/usr/geigerhv)
- [GGreg20](https://www.tindie.com/stores/iotdev/)
- [MightOhm Kit](https://www.tindie.com/stores/mightyohm/)

*Currently the GC10 integration is untested until I can gain access to a device.*

Other Serial based should in theory be supportable with small changes to the codebase.

## Contributions

Contributions are welcomed, please feel free to raise a Pull Request for this. I am a new Arduino/C coder, so please feel free to suggest improvements to the code here to make it better for everyone!

## Thanks 🙏
Thanks for libraries goes to:
- https://github.com/tzapu/WiFiManager
- https://github.com/khoih-prog/AsyncHTTPRequest_Generic
- https://github.com/gmag11/ESPNtpClient
- https://github.com/MattFryer/Smoothed
- https://github.com/knolleary/pubsubclient/
- https://github.com/bblanchon/ArduinoJson

And inspiration:
- https://github.com/1technophile/OpenMQTTGateway
- https://github.com/G4lile0/tinyGS/
