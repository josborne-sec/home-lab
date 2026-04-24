# Home Lab

A living documentation of my cybersecurity focused home lab. This repo captures everything I build, break, and learn. From network architecture and firewall configuration to SIEM deployment and detection engineering.

## Purpose

This lab exists to bridge the gap between classroom knowledge and real-world security operations. Every project here reflects a deliberate effort to understand not just *how* something works, but *why* it matters from a security perspective.

## Current Architecture

| Component | Details |
|-----------|---------|
| Hypervisor | Proxmox VE on ThinkCentre |
| Firewall | OPNsense 26.1.2 (VM) | 
| Switch | TP-Link TL-SG108E (managed, 802.1Q VLANs) |
| WAN Uplink | GL.iNET Beryl MT3000 |
| Future | NAS, SIEM (Wazuh), IDS (Suricata/Zeek) | 

## Network Segmentation

| VLAN | Name | Subnet | Purpose |
|------|------|--------|---------|
| 20 | HOME | 192.168.20.0/24 | Primary Devices |
| 30 | SERVERS | 192.168.30.0/24 | Proxmox, NAS |
| 40 | LAB | 192.168.40.0/24 | Isolated practice environment | 
| 50 | GUEST | 192.168.50.0/24 | Untrusted devices |

## Labs
| # | Lab | Status | 
|---|-----|--------|
| 01 | [Proxmox + OPNsense + VLAN Segmentation](labs/01-proxmox-opnsense-vlan/) | Complete |

## Skills Demonstrated

- Network Segmentation and VLAN design
- Firewall configuration and inter-VLAN routing
- Hypervisor deployment and VM management
- Troubleshooting complex network issues
- Security-focused network architecture

## Background

I am a cybersecurity major at Kennesaw State University and IT Security Intern. I have hands-on experience with enterprise tools including Microsoft Sentinel, Defender, Mimecast, Qualys, Cisco ISE, and Zscaler. This lab is where I take what I learn and go deeper.

## Roadmap

- [ ] Proxmox SDN configuration for true VM VLAN isolation
- [ ] NAS deployment on VLAN 30
- [ ] Wazuh SIEM deployment
- [ ] Suricata/Zeek IDS on dedicated monitoring interface
- [ ] Detection rule development (KQL, Suricata rules)
- [ ] Active Directory lab on VLAN 40

