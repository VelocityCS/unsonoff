# unsonoff
Tools enabling the use of a local sonoff server, decoupling from the requirement to use Smart Life or Ewelink

Components:
1. unsonoff module, defining classes etc
2. unsonoff server. This will have 2x interfaces: 1 to receive data from/send commands to sonoff devices, and 1 to listen for commands and provide feedback
3. unsonoff controller. This will be a HA component
4. desonoff. This is to reprogram the devices to use the unsonoff server

Unsonoff server:
The replacement for the sonoff cloud requires secure websockets for communications - both with devices and for commands/responses. To implement this we can use crossbar.io

## Banana
Fish
