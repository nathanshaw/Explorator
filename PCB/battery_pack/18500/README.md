## Schematic
[Schematic](schematic_18500_pack_both_sides.png)
# PCB Layout

[Both Sides!](layout_18500_pack_both_sides.png)
## 18500 Pack V2 Notes
This pack is specifically designed to be placed within a 60mm wide enclosure. 

** IF YOU ARE USING THIS DESIGN FOR YOUR OWN PROJECT, IT IS STRONGLY RECOMMENDED THAT YOU increase the PCB width before manufacturing**

The traces for user controls are EXTREMELY close to the boards edge.

Please keep in mind the expected current requirements for your device
when choosing the copper weight during the manufacturing process. Likewise,
keep in mind the values and current requirements for your physical user
controls (if attached through the PCB).
- The PWR traces for the board are 100 mil thick and are doubled up for all connections to increase current capacity.
- This means that if the copper thickness is 1 oz. the board can withstand continuous currents of around 4.7 Amps per-trace or 9.4 amps total.
- If the copper thickness is increased to 2 oz the board can withstand around 7.7 amps per trace, or 15.4 amps total
- Both of these numbers are very rough estimates that are assuming an ambient temperature of 25 C, and a maximum trace temperature ride of 10 C
- The PCB Trace Width Calculator by 4pcb.com is a great tool to help with these calculators: [Try Their Tool Here!]<https://www.4pcb.com/trace-width-calculator.html>

### Notes for Future Revisions
- Move logic traces away from side of PCB
- Consider combining GND and PWR for user controls to reduce traces i
- - (must investigate the EE implication of this)
