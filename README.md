# Power Supply Upgrade Kit

Power Supply Upgrade Kit (PSUK) allows to turn a power supply into LiFePO4 charger

# Objectives

To convert the existing power supply [ATABA S-360-12](https://prom.ua/ua/p1276775685-impulsnyj-blok-pitaniya.html) into LiFePO4 battery charger.


# Requirements

1. Current regulation.

REQ-001. PSUK shall linearly regulate output current up to threshold value that depends on the current regulation threshold selection.

REQ-002. If the current regulation threshold is set to "Boost mode" the PSUK regulates output current up to 25A±10%.

REQ-003. If the current regulation threshold is set to "Normal mode" the PSUK regulates output current up to 15A±10%.

REQ-004. If the current regulation threshold is set to "Gentle mode" the PSUK regulates output current up to 5A±10% (optional).

REQ-005. Current regulation threshold shall be manually selected by a mechanical switch.

REQ-006. Switching to current regulation shall be indicated by the yellow LED.

REQ-007. Current regulation shall not affect fan operation.

2. Battery isolation.

REQ-008. If no AC power available the PSUK output shall be electically disconnected from the battery to avoid battery disharge by the fan and voltage feedback stages.

3. Voltage regulation.

REQ-009. PSUK shall extend the output voltage adjustment range up to 15V. Note: in the original state it is limited to 14-14.1V.

# Concept

![PSUK concept](/doc/images/rework_concept.png)

# Power Supply data

![FB schematics reverse engineering](/doc/images/fb_sch.png)

![FB schematics reverse engineering](/doc/images/fb_sch2.png)
