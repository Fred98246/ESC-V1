# ESC Version 1

First version of a fully functioning ESC for brushless motor control using 6-step commutation controlled by an STM32 microcontroller with AM32 firmware. The PCB is designed to match the pins specified in the AM32 code for HARDWARE_GROUP_G0_N (STM32G071K8U6). Simply flash the firmware and it is ready to use out-of-the-box with no pin remapping required. The ESC is designed for 4-6S li ion battery.

The device features a 6-MOSFET half-bridge for the control of each phase, current sensing with the use of a shunt resistor and current sensing amplifier, voltage sensing with a simple voltage divider, back-EMF sensing for accurate motor control, SWD for firmware installation, and Bidirectional DShot to control the ESC.

This first version focuses on single-motor validation before moving to a fully optimized layout. Future iterations will integrate a 4-in-1 design scaled down to standard 5-inch drone dimensions.

Components used:
* **STM32G071K8U6** - Microcontroller
* **DRV8300DRGER** - Gate driver
* **TPS62932DRLR** - Buck converter
* **BUK9M3R3-40HX** - MOSFETs
* **INA180B2QDBVRQ1** - Current sensing amplifier

**Schematic:**

<img width="1129" height="772" alt="image" src="https://github.com/user-attachments/assets/7d386da7-6b9b-45b4-889d-73891edff038" />

**PCB:**

Design in progress...

**Testing (after PCB i will test this circuit and see how it responds)...**

**Links to learn abaout ESC design and brushless motors:**

* 10xareo: https://www.youtube.com/watch?v=67gBlW3sq4E&t=408s (Example of similar ESC build)
* Phills labs: https://www.youtube.com/watch?v=dJjxcjJOlN0 (Great for understanding how to create the PCB)
* Electronoobs: https://www.youtube.com/watch?v=erppWLMzw8I&t=2189s (All the theory behind how the ESC works)
* The engeneering mindset: https://www.youtube.com/watch?v=yiD5nCfmbV0 (Understanding brushless motors)

* https://www.allpcb.com/allelectrohub/designing-pcbs-for-power-electronics-in-industrial-automation
* https://savobajic.ca/projects/personal/esc/esc-v1/ 
* https://vedder.se/2015/01/vesc-open-source-esc/
* https://www.ligpower.com/blog/complete-drone-motor-guide.html (Guide on drone Motors)

