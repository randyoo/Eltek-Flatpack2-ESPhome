# Eltek-Flatpack2-ESPhome
Configure and monitor Eltek Flatpack2 PSU using ESPhome. In my case, it will be used to charge a LFP battery pack, controlled and monitored from Home assistant.

I've made several improvements in this fork, including serial number detection and setting of the default voltage. More to come, hopefully.

## HW prototype
- ESP-WROOM-32
- SN65HVD230 CAN transceiver

## Sources
https://openinverter.org/forum/viewtopic.php?t=1351

## Notes
- note that PSU reverts to the default voltage with *no current limit* when in a no-communication state
- CAN bus is wired directly from the PSU--you a PCB to connect the backplane
- current limiting only works above 48V on the output terminals

## How it looks in Home assistant:
![HA lovelace](https://github.com/taHC81/Eltek-Flaptack2-ESPhome/blob/main/Eltek-Flatpack2-HA2.png?raw=true)
