# Home Network Documentation

## About this Documentation

The purpose of this document is to describe my home network and how they are physically connected both physically and logically.

## Network Diagram

<img width="889" height="679" alt="image" src="https://github.com/user-attachments/assets/a27b7197-968b-4a4f-8c9c-189c244744d1" />

----

<img width="761" height="628" alt="image" src="https://github.com/user-attachments/assets/d2d233c6-bddc-4626-93b9-9dc3fa40d8d8" />

----

The network contains:

- Home Router
- 24 port POE switch
- Desktop Computers
- IP cameras and NAS
- Laptops
- Smart Phones and tablets
- IoT devices
- Smart TV

The network was segmented into five VLANs
| VLAN # | Devices               |
|--------|-----------------------|
| VLAN 1 | Management and admins |
| VLAN 2 | Home Users |
| VLAN 3 | IoT Devices |
| VLAN 4 | IP cameras and NAS |
| VLAN 5 | Guest Users |

## IP Addressing
 
| VLAN # | User        | Purpose                                | Network           | Gateway        |     DHCP Range      |
| ------ | ----------- | -------------------------------------- | ----------------- | -------------- | --------------------|
| VLAN 1 | Admins      | Router, switch, management             | 192.168.80.0/24 | 192.168.80.1 | 192.168.80.25-75  |
| VLAN 2 | Home Users  | Desktop, laptops, smartphones,tablets  | 192.168.40.0/24 | 192.168.40.1 | 192.168.40.100-200|
| VLAN 3 | IoT         | Smart TVs, smart sensors, IoT hubs		| 192.168.30.0/24 | 192.168.30.1 | 192.168.30.100-200|
| VLAN 4 | Cameras/NAS | IP network cameras and NAS             | 192.168.90.0/24 | 192.168.90.1 | 192.168.90.80-130 |
| VLAN 5 | Guest       | Guest smartphones/tablets              | 192.168.10.0/24 | 192.168.10.1 | 192.168.10.50-150 |

## Device Inventory

- Router - ASUS RT-BE92U BE9700 Tri-Band WiFi 7
- Switch - 24 port switch
- Desktop - 2 desktop computer
- Laptops - 3 laptops
- Phones - Smartphones
- Tablets - tablets
- IoT Devices - Sensors and hubs
- IP Cameras - 3 wired network cameras
- NAS - Ugreen 2 bay Nasync

## Revision History

**Author:** nmontan
| Version | Date | Description |
|---|---|---|
| 1.0 | July 28, 2026 | Created initial home network documentation |
| 1.1 | July 30, 2026 | Updated network diagrams and final documentation |

## References

- GitHub Markdown documentation
- Cisco networking learning resources
- Microsoft learn networking documentation
- Diagrams were created using Lucidapp, an online networking diagraming tool
- https://stevessmarthomeguide.com/documenting-your-home-network/

