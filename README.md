# Cisco Packet Tracer — VLAN Lab & IT Student Guide

A beginner-friendly practical guide for building a 2-Switch, 6-PC VLAN network in Cisco Packet Tracer, plus an installation and IT student guide for getting started with the software. This repository contains two guides: the first is a complete step-by-step practical for building a 2-switch, 6-PC, 3-VLAN network (VLAN 10, 20, and 30) using two Cisco 2960 switches connected by a trunk link with no router, where PC1–PC3 connect to S1 and PC4–PC6 connect to S2, each PC is assigned to its VLAN via an access port, IP addresses are set manually with an empty default gateway, and same-VLAN devices across both switches can ping each other while cross-VLAN communication fails as expected because Layer-2 switches alone cannot route between VLANs. The second guide explains what Packet Tracer is, how to install it, why it matters in an IT course, and a recommended beginner learning path. The key takeaway is that PCs are end devices, switches connect them, VLANs separate them into logical groups, access ports place individual PCs into VLANs, the trunk carries multiple VLANs between S1 and S2, IP addresses let devices in the same VLAN communicate, and no router is used here so different VLANs cannot route to one another.

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `Cisco_Packet_Tracer_2_Switch_6_PC_VLAN_Guide.docx` | Full step-by-step practical: build and configure a 2-switch, 6-PC, 3-VLAN network with a trunk link and no router. |
| `Cisco_Packet_Tracer_Installation_and_IT_Guide.docx` | How to install Packet Tracer, why it matters in an IT course, and a recommended learning path for beginners. |

---

## 🧪 Lab Overview — 2 Switches, 6 PCs, 3 VLANs

### What You Will Build

- 2 × Cisco 2960 switches (S1 and S2)
- 6 × PCs (PC1–PC6)
- 3 × VLANs (VLAN 10, 20, 30)
- 1 × trunk link between S1 Gi0/1 and S2 Gi0/1
- No router — this is a Layer-2 only design

### Topology

```text
            S1 ================= S2
           /  \  \             /  \  \
        PC1  PC2  PC3       PC4  PC5  PC6
      VLAN10 VLAN20 VLAN30 VLAN10 VLAN20 VLAN30
