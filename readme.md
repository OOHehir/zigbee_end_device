# Zigbee End Device

Based on the Zigbee Minimal example with the following changes:

- Change the cluster to a HA temperature endpoint, profile ID 0x0104.

In the Simplicity Studio, go to the SOFTWARE COMPONENTS tab and install the software components:

- [Zigbee] → [Utility] → [Zigbee Device Config] → Configure as End Device
- [Zigbee] → [Stack] → [Pro Core] → [Pro Leaf Stack]
- [Zigbee] → [Stack] → [Pro Core] → [Pro Stack (Common)] → Uninstall
- [Zigbee] → [Cluster Library] → [Common] → [Reporting]
- [Zigbee] → [Zigbee 3.0] → [Network Steering]
- [Zigbee] → [Zigbee 3.0] → [Find and Bind Initiator]
- [Platform] → [Driver] → [Button] → [Simple Button] → [btn0]


Change app.c