# PCB for Fenix
 PCB to implement Fenix autopilot
 ## Configuration
 ### V1.0
 Known errors and limitations
 There is an identified error in the current Fenix PCB design. The pins for PWM/DIR are not correctly allocated. PIN 6&7 are the right PINS. PIN 11&12 should be discarded. In consequence, provisions for these signals in Fenix PCB are not valid.

 Mitigations proposed:
 1 - Usage of a motor controller Arduino shield instead where PWM/DIR pins are directly connected to Arduino through the shield and can be configured correctly to PIN6&7. For this purpose I recommend the shield version of MD10C,
 https://www.robotshop.com/es/es/moto...no-shield.html

 2 - If you already have the MD10C R2 or any other "wired version", and still wants to use Fenix PCB you can still do so, just connect the PWM/DIR pins from motor controller to the arduino 6&7PINS through cables.

 ### V1.1 patch to fix V1.0 known errors
 WARNING! This patch has not been tested. Use at your own risk.
 - PWM/DIR pins where wrongly allocated to D11, D12. Reallocated to D6, D7.
 - Removed serial I/F expansion: No specific use.
 - J1, J2 screwed plugs shifted. In case of shield pins too short there was a risk of short-circuit with USB plug.
 - Screwed plug pin tags shifted. After screwed plug installation it was not possible to read the text.  
