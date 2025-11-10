# Firmware
Custom firmware files here are for Meshcore.
* Based on MeshCore and compatible with MeshCore. These features will be pushed to MeshCore for public use.
* Have more experimental / advances features.
* The firmware is provided as it is without any warranty or support.

Naming convention: firmware-role-boardtype-MeshCore_Version-feature[NUMBER]
* For example: firmware-repeater-heltecv3-v1.9.1-powersaving01.bin. This is the firmware for repeater using Heltec v3, based on MeshCore v1.9.1 (main) with added powersaving and the number is 01. The number is our own version.

## Change logs:
### firmware-repeater-heltecv3-v1.9.1-powersaving01.bin: 
Reduced from 47mA down to 7mA. 
* To deepsleep after 2 minutes.

### firmware-repeater-heltecv3-v1.9.1-powersaving02.bin: 
Reduced more power consumption. Optimized OLED, adverts and shorter operation time.
* In normal start / reset: To wake up 30s to allow sending an advert. To power on OLED for a while.
* When waken up from deepsleep: To sleep again in 5s. No OLED. No advert.

<img height="512" alt="image" src="https://github.com/user-attachments/assets/203c3459-5d14-4848-98d2-f75acdcfbf3e" />


