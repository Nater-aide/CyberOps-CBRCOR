# NextGen Firewall
- FX-OS - The Cisco Firepower Extensible Operative System (FX-OS) controls the chassis hardware.
- FTD -The Cisco Firepower Threat Defense (FTD) runs the NGFW.
- DAQ - data acquisition Library

## NGFW - Next Generation Firewall 
- Routed Mode - Provides layer 3 between two or more segments
- Transparent mode - Layer 2 firewall that acts like a bump in the wire. It is not seen as a router hop to connected devices.

Firepower NGFW runs on 2 main engines
1. **LINA (think ASA)** -- process the ASA configuration rules. SNort engine processed the rules
2. **Threat Defense engine**

## Event Types
- **Connection Events** - Contain data about detected sessions
- **Security Intelligence Events** - special kind of connection event that you can view and analyze seperately
- **Intrusion Event** - This examines packets. When it detects, it creates an intrusion event
- **File Events** - Files that the system detects. AMP tries to hash as much of the file as possible
- **Malware Events** - This represents malware files that are detected.
  - **Malware**, **clean**, or **unknown** results
  - If no connection is made with AMP, it returns the status **unavailable** 
