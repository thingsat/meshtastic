# Automatic Packet Reporting System 📡🎈 for Meshtastic radiosondes

[Automatic Packet Reporting System (APRS)](https://en.wikipedia.org/wiki/Automatic_Packet_Reporting_System) is an amateur radio-based system for real time digital communications of information of immediate value in the local area.

The APRS message format is widely used by radiosondes carried on weather stratospheric balloons 🎈. Radio amateurs 📡 collects APRS messages to track and to recover radiosondes throught services such as [Sondehub](https://sondehub.org/#!mt=Mapnik&mz=5&qm=3h&mc=46.54375,3.7793&box=aboutbox).

This extension proposes a portnum and a protobuf message dedicated to APRS messages (which are text-based). Ground repeaters relay in priority the messages of the Meshtastic radiosondes.

Smartphone applications (iOS, Android) can decode APRS messages in order to track balloons during the flight and to recover lost radiosondes.
