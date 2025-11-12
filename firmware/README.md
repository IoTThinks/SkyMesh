# Custom Meshcore Firmware
Custom firmware files here are for Meshcore.
* Based on MeshCore and compatible with MeshCore. These features will be pushed to MeshCore for public use.
* Have more experimental / advances features.
* The firmware is provided as it is without any warranty or support.

Naming convention: firmware-role-boardtype-MeshCore_Version-feature[NUMBER]
* For example: firmware-repeater-heltecv3-v1.9.1-powersaving01.bin. This is the firmware for repeater using Heltec v3, based on MeshCore v1.9.1 (main) with added powersaving and the number is 01. The number is our own version.

## Instruction to flash
* Download the latest bin file above
* Go to Web Flasher: https://flasher.meshcore.co.uk/
* Select Custom Firmware
<img height="384" alt="image" src="https://github.com/user-attachments/assets/d75c1b40-a349-488f-b623-77fbab06ddca" />

* Select the downloaded bin file
* Do NOT erase device if you want to keep the existing configuration
* Click Flash
<img height="384" alt="image" src="https://github.com/user-attachments/assets/a783b5a6-494e-44f7-b38c-63e4277039e1" />

## Repeaters
This is the changelog for repeaters:

### 01. firmware-repeater-heltecv3-v1.9.1-powersaving01.bin: 
Reduced from 47mA down to 7mA. 
* To deepsleep after 2 minutes.

### 02. firmware-repeater-heltecv3-v1.9.1-powersaving02.bin: 
Reduced more power consumption. Optimized OLED, adverts and shorter operation time.
* In normal start / reset: To wake up 30s to allow sending an advert. To power on OLED for a while.
* When waken up from deepsleep: To sleep again in 5s. No OLED. No advert.

<img height="512" alt="image" src="https://github.com/user-attachments/assets/203c3459-5d14-4848-98d2-f75acdcfbf3e" />

## Companions
Coming soon

## Sensors
