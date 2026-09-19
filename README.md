\# Cisco Enterprise VoIP / CME PBX Lab



\## Overview



A simulated enterprise VoIP/PBX environment built using Cisco Packet Tracer, featuring Cisco CallManager Express (CME), SCCP IP phones, Voice VLANs, DHCP with Option 150, extension dialing, and VoIP troubleshooting.



\## Topology



\- Cisco 2811 Router — VOICE-RTR

\- Cisco 2960 Switch — VOICE-SW

\- Cisco 7960 IP Phones

&#x20; - PHONE-101

&#x20; - PHONE-102

&#x20; - PHONE-103

\- Three PCs connected through the IP phones



\## Network Design



| Component | Configuration |

|---|---|

| Voice VLAN | VLAN 10 |

| Voice Subnet | 192.168.10.0/24 |

| Gateway | 192.168.10.1 |

| CME/SCCP Server | 192.168.10.1 |

| SCCP Port | 2000 |

| DHCP Option 150 | 192.168.10.1 |



\## Extensions



| Phone | Extension |

|---|---:|

| PHONE-101 | 101 |

| PHONE-102 | 102 |

| PHONE-103 | 103 |



\## Features Implemented



\- Voice VLAN configuration

\- 802.1Q trunking

\- DHCP for IP phones

\- DHCP Option 150

\- Cisco CME / SCCP

\- IP phone registration

\- Extension assignment

\- MAC address mapping

\- Internal VoIP calling

\- Layer 2 / Layer 3 troubleshooting

\- Packet Tracer Simulation Mode



\## Validation



All three IP phones successfully registered with CME.



Successful call tests included:



\- 101 → 102

\- 102 → 101

\- 101 → 103

\- 103 → 102



\## Troubleshooting Case



\### Problem



PHONE-103 initially failed to register with CME and repeatedly produced:



```text

Phone-Reg-Rej
```

