# Mestastic-Tak-Bridge
Network communication to show [meshtastic](https://meshtastic.org/) devices in TAK / ATAK ecosystem.  Utilizes MQTT and Nodered

This project implements the servers and protocol translation so that a network of meshtastic devices can be displayed in ATAK system.

This includes a mqtt server and a node red server. 

## Architecture
![Architecture](https://github.com/erichexter/Mestastic-Tak-Bridge/assets/114692/e43593aa-e5d1-42a0-876b-0385e3537b6c)

## Use Case
The initial functionality is to allow meshtastic devices to be used as trackers in ATAK, they do not need to be connected to phones via bluetooth, they provide situational awarenes to the people runing atak clients.  This is not an offline solution for running atak without an existing network. There is a seperate project that tries to solve that use case.


## Node Red flow

![flow](https://github.com/erichexter/Mestastic-Tak-Bridge/assets/114692/c8283f86-ee1b-43cc-b475-cd4f45ab362a)


## Mapping

| Meshtastic | ATAK | example |
| ---------  | ---- | ------- |
| Long Name | Callsign | meshtastic e9f3 |
| 1st char of short name | Team Role | **M**Y02 = Team **M**ember |
| 2nd char of short name | Team Color | M**Y**02 = **Y**ellow |
| Battery level | Battery Level | |

## Install

This solution is designed to run in docker utilizing docker compose.  It is setup to work out of the box to connect to a local tak server runing on the same machine.

To start run the following command run.ps1 or run.sh 

