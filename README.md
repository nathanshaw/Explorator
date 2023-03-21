# Explorator Hardware

This repo contains the PCB layout and schematic files for the Explorator genus.

The files included in this repo were created within EAGLE CAD. 
## Repo Structure
PCB
- battery_pack
  - [18500](##Battery-Pack---18500)
  - [18650](##Battery-Pack---18650) 
- [breakout_board](##Explorator-Breakout-PCB)
- mainboard
  - [v1_large_pcb](##Explorator-v1-Mainboard-(large))
  - [v2_small_pcb](##Explorator-v2-Mainboard-(small))

### Repo Files
- .brd files are EAGLE's board files and contain information about the PCB's layout. 
- .sch files are EAGLE's schematic files and contain information about the schematic from which the PCB's are designed.
- .lbr files are EAGLE's library files and contain all the libraries used to create the individual PCB's, there should be a libary file for each folder in the repo. The entire libraries are exported for the battery pack and breakout PCB(including parts not in the design), but for the mainboards only the footprints used in the design are exported to save repo space.
- README.md files accompany each board in the appropiate folder and contains information about manufacturing the PCB, known issues, and other notes
- .png's are included for each board and include the schematic, and the layout of the board.
  - Files that start with "schematic_" are schematic images 
  - Files that start with "layout_" are layout images.
- parts_list.txt is a text file created by EAGLE showing the components used to populate each board. 
- pin_list.txt is a list of all the pin and pad names in the layout and schematic files
- BOM_*.csv is a comma separated list that contains all of the electronic components needed for the PCB (similar to parts_list.txt, but more useful most of the time)
- net_list.txt is a list of all the connections between different nets in the schematic
- CAMOutputs contains two folders, one for the drill file and one for the other gerbers. These outputs were created in EAGLE using the PCBWay_2_layer.cam file at the root level of the PCB folder

Please note, if you do not have access to EAGLE CAD, the easiest way to view these boards is by using an online gerber viewer such as this one provided by [pcbway.com!]<https://www.pcbway.com/project/OnlineGerberViewer.html>. To use this method simply .zip the CAMOutputs folder and drag the compressed .zip file into the browser and an interactive PCB generated from the Gerbers can be viewed. Pretty cool =)

# Repo Contents
The following PCB designs are included in this repo:

## Explorator v1 Mainboard (large)
    
- 99mm diameter
- Teensy 3.2 Microcontroller
- 1x SHTC3 Temperature and Humidity Sensor
- 3x channel of DC motor control
- 9x channels of solenoid control
- 1x power switch
- 1x power input jack
- 2x pots
- 4x buttons

## Explorator v2 Mainboard (small)
- 58mm diameter
- Teensy 3.2 Microcontroller
- 1x channel of DC motor control
- 2x channels of solenoid control
- 2x VEML 6030 Ambient Light Sensors
- 1x SHTC3 Temperature and Humidity Sensor
- 10x WS2813 NeoPixel LEDs
- 1x power switch
- 1x power input jack
- 2x pots
- 2x buttons

## Explorator Breakout PCB
- 40mm diameter
- 10-pin JST connector to mate with mainboard
- 10x WS2813 NeoPixel LEDs
- 1x VEML 6030 Ambient Light Sensor
- 1x TDK ICS-43434 MEMs microphone

## Battery Pack - 18500
- 3x 18500 Lithium Ion Batteries
- Support for routing user controls through PCB
- 2x 100 mil traces for all power connections 
  - providing around 14 amps of current on 2 oz copper PCBs

## Battery Pack - 18650
- 3x 18650 Lithium Ion Batteries
- 1x 100 mil trace for all power connections
  - providing around 7 amps of current on 2 oz copper PCBs

# Related Repos and Work

The Explorator genus firmware is contained in this repo:
- https://github.com/nathanshaw/unified_hss_firmware
More information about this project can be found here: 
- https://nathanvillicanashaw.com/archive


