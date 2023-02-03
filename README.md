# Power Supply Upgrade Kit

Power Supply Upgrade Kit (PSUK) allows to turn a power supply into LiFePO4 charger

# Objectives

To convert the existing power supply [ATABA S-360-12](https://prom.ua/ua/p1276775685-impulsnyj-blok-pitaniya.html) into LiFePO4 battery charger.


# Requirements

1. Current regulation.

REQ-001. PSUK shall linearly regulate output current up to threshold value that depends on the current regulation threshold selection.

REQ-002. Current regulation threshold selection shall be done by the variable resistor in the range from 5A to 25A (wider range is also acceptable).

REQ-003. Switching to current regulation shall be indicated by the yellow LED.

REQ-004. Current regulation shall not decrease output voltage lower than 10V to preserve the Fan operation in current regulation mode.

2. Battery isolation.

REQ-005. If no AC power available the PSUK output shall be electically disconnected from the battery to avoid battery disharge by the fan and voltage feedback stages.

3. Voltage regulation.

REQ-006. PSUK shall extend the output voltage adjustment range up to 15V. Note: in the original state it is limited to 14-14.1V.

4. Fan control.

REQ-007. PSUK shall not activate the cooling FAN if the output current is near zero (0-0.3A) otherwise the FAN shall be operating.

Note: this requirement is for supporting the UPS use case when the soundless operation is preferred.

# Concept

![PSUK concept](/doc/images/rework_concept.png)

# Power Supply data

![FB schematics reverse engineering](/doc/images/fb_sch.png)

![FB schematics reverse engineering](/doc/images/fb_sch2.png)

# References

https://danyk.cz/reverz44_en.html

https://elektrotanya.com/s-360-12_12v_30a_power_supply_sch.pdf/download.html
