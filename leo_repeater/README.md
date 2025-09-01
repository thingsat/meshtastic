# Low-Earth Orbit (LEO) Meshtastic Repeater

## Thingsat payloads

The [Thingsat payloads for LEO cubesats](https://gricad-gitlab.univ-grenoble-alpes.fr/thingsat/public/-/tree/master/cubesat_mission_2) host a LoRa gateway (SX1303+1250) and a LoRa/LR-FHSS transceiver (SX1262).

The Thingsat payload can repeat LoRa messages from terrestrial Meshtastic networks (according to the preset configuration and the community public channels of the overflown region).

Three launches are planned in 2026.

However, a first experiment has been tested aboard [stratospheric balloons in June 2025](https://gricad-gitlab.univ-grenoble-alpes.fr/thingsat/public/-/tree/master/balloons/2025-05)

Best distance : 496,48 Km with [29TRG1ML8ClN_H3-🗼-finiz | h3fz - !33691c48](https://map.gaulix.fr/node/3733)
```
Expéditeur : 40CSUG-Balloon🎈-73-868 | CB38 - !435b98b4
Carte
Destinataire : !ffffffff
Passerelle MQTT Gaulix : 29TRG1ML8ClN_H3-🗼-finiz | h3fz - !33691c48
Distance de 496,48 Km - 0 sauts | SNR : -18,5 | RSSI : -128
Carte
Canal : Fr_Balise
Reçu en direct
```

```
Passerelle MQTT Gaulix : 01VILLLM8ClP 🏡🛜 | 01VL - !c4f7c30c
Distance de 464,48 Km | SNR : -9 | RSSI : -133
Voir la trame
Passerelle MQTT Gaulix : 33YVRALM8ClP_Michel | f7a4 - !433df7a4
Distance de 76,79 Km | SNR : -12,5 | RSSI : -127
Voir la trame
Passerelle MQTT Gaulix : 29TRG1ML8ClN_H3-🗼-finiz | h3fz - !33691c48
Distance de 496,48 Km | SNR : -18,5 | RSSI : -128
```

![Thingsat payload @ SatRev's SOWA cubesat platform](https://gricad-gitlab.univ-grenoble-alpes.fr/thingsat/public/-/raw/master/cubesat_mission_2/media/thingsat-em-v2-01.jpg)

## LEO module for Meshtastic

The LEO module for Meshtastic allows the node to enter sleep mode and wake up when a satellite is in view.

The LEO module for Meshtastic enables to trig message exchanges (RX/TX) when a satellite is in view.

Prediction of satellite passes can be computed using the [AioP13 library](https://github.com/dl9sec/AioP13).

[Proposition of `protobuf` description for node configuration](protobuf/leo.proto)