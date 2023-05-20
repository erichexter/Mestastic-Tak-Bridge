# Mestastic-Tak-Bridge
Network communication to show mestastic devices in TAK / ATAK ecosystem.  Utilizes MQTT and Nodered

This project implements the servers and protocol translation so that a network of meshtastic devices can be displayed in ATAK system.

This includes a mqtt server and a node red server. 

![Architecture](https://github.com/erichexter/Mestastic-Tak-Bridge/assets/114692/e43593aa-e5d1-42a0-876b-0385e3537b6c)

The initial functionality is to allow meshtastic devices to be used as trackers in ATAK, they do not need to be connected to phones via bluetooth, they provide situational awarenes to the people runing atak clients.  This is not an offline solution for running atak without an existing network. There is a seperate project that tries to solve that use case.
