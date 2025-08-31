# Zigbee End Device

Based on the Zigbee Minimal example with the following changes:

- Change the cluster #1 to a HA temperature sensor device (0x0302), profile ID 0x0104.

In the Simplicity Studio, go to the SOFTWARE COMPONENTS tab and install the software components:

- [Zigbee] → [Utility] → [Zigbee Device Config] → Configure as End Device
- [Zigbee] → [Stack] → [Pro Core] → [Pro Leaf Stack] → Uninstall
- [Zigbee] → [Stack] → [Pro Core] → [Pro Stack (Common)] → Uninstall
- [Zigbee] → [Cluster Library] → [Common] → [Reporting]
- [Zigbee] → [Zigbee 3.0] → [Network Steering]
- [Zigbee] → [Zigbee 3.0] → [Find and Bind Initiator]
- [Platform] → [Driver] → [Button] → [Simple Button] → [btn0]

Change file app.c


Issues:
- Got stuck at RTCC_SyncWait(void). Change Sleep Timer to TIMER