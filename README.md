# secure-network-design
# My Secure Network Design Project

Hey there! This is the actual Cisco Packet Tracer (`.pkt`) lab file for a secure corporate network I designed from scratch. Even though it was originally part of a group assignment, I handled the entire design, configuration, and security setup myself, so I'm hosting the raw file here to show off my network engineering skills.

## 🛠️ What I Built
The goal was to make a corporate network that is highly organized and tough to break into. Here is how I set it up:

* **Separating the Network (VLANs):** I didn't want everyone sharing the same space. I split the network into different zones so that guests on the Wi-Fi (`VLAN 20`) are completely isolated and can't touch internal staff files (`VLAN 10`) or management servers (`VLAN 30`).
* **Central Logins (AAA/RADIUS):** Instead of typing passwords into every single device, I set up a central RADIUS server using `aaa new-model`. This handles logins securely from one main spot.
* **Firewall Rules (ACLs):** I wrote custom Access Control Lists (ACLs) that block guest traffic from snooping around internal servers while still letting them browse the internet normally.
* **Network Basics:** Configured automated IP addressing (DHCP pools) and Inter-VLAN routing so the allowed devices talk to each other perfectly.

## 📂 What's in Here?
* **`*.pkt`** - The main Cisco Packet Tracer file. You can open this up directly in Packet Tracer to see the full topology map and look through my router and switch CLI configurations!
