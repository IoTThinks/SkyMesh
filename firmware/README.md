# Custom Meshcore Firmware
Custom firmware files are for Meshcore.
* Based on MeshCore and compatible with MeshCore.
* These features will be pushed to MeshCore for public use.
* Have more experimental / advances features.
* The firmware is provided as it is without any warranty or support.
* If you want custom firmware or private support, please [contact us](https://iotthinks.com/contact-us/).

Naming convention: firmware-role-boardtype-MeshCore_Version-feature[NUMBER]
* For example: firmware-repeater-heltecv3-v1.9.1-powersaving01.bin. This is the firmware for repeater using Heltec v3, based on MeshCore v1.9.1 (main) with added powersaving and the number is 01. The number is our own version.

## Repeaters
This is the changelog for repeaters:

### firmware-repeater-heltecv3-v1.9.1-powersaving01.bin: [HERE](https://github.com/IoTThinks/LoRaMeshVietnam/blob/main/firmware/firmware-repeater-heltecv3-v1.9.1-powersaving01.bin)
Reduced from 47mA down to 7mA. 
* Based on MeshCore repeater v1.9.1 - main branch
* To deepsleep after 2 minutes.

### firmware-repeater-heltecv3-v1.9.1-powersaving02.bin: [HERE](https://github.com/IoTThinks/LoRaMeshVietnam/blob/main/firmware/firmware-repeater-heltecv3-v1.9.1-powersaving02.bin)
Reduced more power consumption. Optimized OLED, adverts and shorter operation time.
* Based on MeshCore repeater v1.9.1 - main branch
* In normal start / reset: To wake up 30s to allow sending an advert. To power on OLED for a while.
* When waken up from deepsleep: To sleep again in 5s. No OLED. No advert.
* Known issues: Only send one advert at first boot or reset. OTA via WiFi is not working.

<img height="384" alt="image" src="https://github.com/user-attachments/assets/203c3459-5d14-4848-98d2-f75acdcfbf3e" />

### firmware-repeater-heltecv3-v1.10.0-powersaving03.bin: [HERE](https://github.com/IoTThinks/LoRaMeshVietnam/blob/main/firmware/firmware-repeater-heltecv3-v1.10.0-powersaving03.bin)
Based on MeshCore v1.10.0 (main). 9mA power consumption with no latency.
* To use light sleep instead of deepsleep
* No latency due to quicker wakeup
* First boot: To wake up for 30s to send an advert at 18th second.
* Light sleep: To wake up when receiving a LoRa packet and light sleep again after 5s.
* Periodically wakeup: To wake up every 30 minutes to do some periodically tasks and and lightsleep again after 5s.
* Known issue: OTA via WiFi is not working yet.
* Source code changes: https://github.com/meshcore-dev/MeshCore/compare/main...IoTThinks:MeshCore:powersaving

<img height="384" alt="image" src="https://github.com/user-attachments/assets/d968ed38-9965-487e-a02e-7a571f7e7d90" />

### firmware-repeater-heltecv4-v1.10.0-powersaving03.bin: [HERE](https://github.com/IoTThinks/LoRaMeshVietnam/blob/main/firmware/firmware-repeater-heltecv4-v1.10.0-powersaving03.bin)
Same feature but for Heltec v4.

## Instruction to flash custom firmware
* Download the latest bin file [HERE](https://github.com/IoTThinks/LoRaMeshVietnam/tree/main/firmware)
* Go to Web Flasher: https://flasher.meshcore.co.uk/
* Select Custom Firmware
<img height="384" alt="image" src="https://github.com/user-attachments/assets/d75c1b40-a349-488f-b623-77fbab06ddca" />

* Select the downloaded bin file
* Do NOT erase device if you want to keep the existing configuration
* Click Flash
<img height="384" alt="image" src="https://github.com/user-attachments/assets/a783b5a6-494e-44f7-b38c-63e4277039e1" />

## Support
If you want custom firmware or private support, please [contact us](https://iotthinks.com/contact-us/).

