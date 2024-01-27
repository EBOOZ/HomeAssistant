# Introduction
Home Assistant is an open-source home automation platform that allows you to monitor and control various aspects of your home, such as lighting, climate, entertainment systems, and appliances. It is a flexible and customizable platform that can be integrated with thousands of devices and brands, often without dependency on the cloud. 

It's the leading platform that offers a wide range of features and integrations. It is known for its flexibility, ease of use, and ability to work with a variety of devices and brands. Home Assistant is also highly customizable, allowing users to create their own automations and scripts to suit their specific needs. 

I'm using Home Assistant for several years now and I'm sharing my setup and configuration for inspiration purposes for others. And I'm also using this repository as a to-do list for the few things I (still) need to fix or add to the setup :smile:

> [!NOTE]
> If you came here by searching for building a 3D floorplan and integrate it in Home Assistant, you may want to go to the [floorplan](floorplan/README.md) folder immediately.

# Hardware
Starting with Home Assistant is easy, and you can already start by installing in on a RaspberryPi 4, or via their own [Home Assistant Green](https://www.home-assistant.io/installation/). After I started with a RaspberryPi myself, I decided to purchase a second hand Intel NUC after a while to have better performance.
* Processor: Intel Celeron N2820 (2,41Ghz)
* Memory: 4GB DDR3L
* Harddrive: 128GB SSD
* Network: 1Gbps
* WLAN: 802.11b, 802.11g, Wi-Fi 4 (802.11n)
* Bluetooth: 4.0
* USB: 2x USB 2.0 (back), 1x USB 3.2 (front)
* Zigbee: [ConBee II USB Dongle](https://www.phoscon.de/en/conbee2)

> [!NOTE]
> I do own a Z-wave stick which I used before moving to Zigbee due to instability issues back in the days. I don't have plans to use Z-Wave in my setup because Zigbee works perfectly and stable.

# Integrations
99% of the people interested in Home Automation will probably start with automating their lights. And so did I. I want to keep vendor-specific solutions, like hubs to control your lights, out of my house as much as possible. Over time the number of integrations grew to the list below.

## Builtin into Home Assistant
| Integration | Description |
| --- | --- |
| Apple TV | Used for Apple TV status monitoring |
| Bluetooth | To connect with the bluetooth blinds motors in the living room |
| deCONZ | Controlling all Zigbee devices |
| Denon HEOS | Control the speaker in the kitchen, which has a Logitech Media Player connected |
| DLNA Digital Media Renderer | Not actively used |
| DSMR Slimme Meter | Measuring power and gas usage |
| Electricity Maps | Used for CO2 Signal statistics |
| ESPHome | Used for water usage readings |
| Google Cast | Was used to cast a dashboard to Google Home |
| Home Assistant iOS | |
| Home Assistant Supervisor | |
| HomeKit Bridge | Pushing selected entities to HomeKit on our phones and tablets |
| Internet Printing Protocol (IPP) | Monitoring the cartridge levels on the HP printer |
| Logitech Harmony Hub | Controlling the home cinema system | 
| Meater | Monitoring BBQ sessions on our Grill Guru Large |
| Meteorologisk institutt (Met.no) | Providing weather information |
| MJPEG IP Camera | Not actively used, and will be deprecated |
| Mobile app | |
| MQTT | Used to control the blinds motors in the living room |
| Ping (ICMP) | Monitoring the availability of the server running LMS and LMS players |
| Shell | |
| Sonos | Control the Sonos Playbar in the guestroom |
| Squeezebox (Logitech Media Server) | A streaming audio server supported by Logitech, supports a range of digital audio receivers |
| Tado | Thermostat and radiator thermostats | 
| Xiaomi BLE | Gains information from plant sensors |
| Xiaomi Miio | Controls the Xiaomi air filter |
| Sun | |

## Community integrations via Home Assistant Community Store (HACS)
| Integration | Description | Repository |
| --- | --- | --- |
| Afvalinfo | Get's information about when garbage is picked up | [link](https://github.com/heyajohnny/afvalinfo) |
| Browser mod | Used for the [floorplan](floorplan/README.md) tablet dashboard | [link](https://github.com/thomasloven/hass-browser_mod) |
| Eufy Security | Displays and controls all Eufy cameras | [link](https://github.com/fuatakgun/eufy_security) |
| Gree A/C | Controlling the airconditioning in the bedroom | [link](https://github.com/RobHofmann/HomeAssistant-GreeClimateComponent) |
| HACS | Communicty Add-on store | [link](https://github.com/hacs/integration) |
| Smart Irrigation | Calculates how long the plants on the roof terrace need to be moistured | [link](https://github.com/jeroenterheerdt/HAsmartirrigation) |
| TP-Link Omada | Integrating data from the home network which is based on TP-Link Omada | [link](https://github.com/zachcheatham/ha-omada) |
| Tronity | Get's data from the electric car | [link](https://github.com/tronity/homeassistant) |
| WebRTC Camera | Required for Eufy camera-streams to be displayed | [link](https://github.com/fuatakgun/WebRTC) |

