# PCB for Fenix
 PCB to implement Fenix autopilot
## Configuration
V1.1 patch to fix V1.0 known errors
WARNING! This patch has not been tested. Use at your own risk.
- PWM/DIR pins where wrongly allocated to D11, D12. Reallocated to D6, D7.
- Removed serial I/F expansion: No specific use.
- J1, J2 screwed plugs shifted. In case of shield pins too short there was a risk of short-circuit with USB plug.
- Screwed plug pin tags shifted. After screwed plug installation it was not possible to read the text.  
