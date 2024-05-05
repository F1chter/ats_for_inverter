This project is used for control for home solar stations

In this case used:
1) Solar panel
2) MPPT controller, thar charge battery
3) Inverter that convert DC to AC
4) Automatic Transfer Switch that switch between Main Supply and Inverter
5) Arduino that controls ATS by next rules:
   -when battery voltage drops to low_level -> switch to main supply
   -when battery is charged to high_level voltage -> switch to inverter

Arduino components:
- Arduino with ATMega 328P(tested on Arduino Nano v3)
- OLED 0,96" I2C display
- Rotary Encoder Module
- three resistors for voltage divider and measurement of battery voltage
- PZEM-004T-100A(v3.0) for gathering statistics
- MicroSD module with card for store statistics
- DC-DC converter for powering Arduino from battery
