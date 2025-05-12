# Netflow
- Netflow Connector -- aggregates and stores in records and forwards to analyzer
- Netflow Exporter -- Collects and exports flow telemtry
- Netflow analyzer  -- this correlates the flows

This of this as a wiretap  
It will not show details on every packet  
**Flow** -- Traffic moving from one destination to another. One IP/port to another IP/Port. Bidirectional flows can be seen as two different flows

### Netflow versions
- 1: Original
- 5: Traditional. Was commonly used
- 9: Flexible, most used today

# Integrating Cisco Stealthwatch
- UDP director - allows netflow, syslog, snmp and other data to be send to multiple colletion points, such as a SIEM
- NVM (Anyconnect Network visbility module) - software for anyconnect that helps you see user and endpoint behavior. This is both on and off premise
- ISE - This integrates with stealthwatch using pxGrid
- CTA (Cognitive Threat Analytics) -- Integrates with stealthwatch for visibility into web based threats

# Cisco Stealthwatch host groups
Host groups are logical containers of IP space.  
Once a host group is defined, you can map relationships

# Anomaly-Based Detection
- Concern index - this tracks bad actors and hosts that are doing bad things
- Target index - endpoint that is having bad things done to it. Think opposite of concerned index
- Recon - potential malicious scans
- C&C - indicates the existence of bots
- Exploitation - tracks attempts
- DDos Source
- DDos target
- Data hoarding - when data is moved within the network
- Exfiltration - data moved outside of the network
- Policy Violation
- Anomaly

# Cisco ETA (Encrypted Traffic Analytics)
Can locate anomamly-based detections without having to decrpyt traffic  
- IDP - initial data packet -- hello packet
- SPLT - sequence of packet lengths and times
- Global Risk map - backed by cisco talos

## 2 cases for Cisco ETA
1. ETA for malware detection -- used to find ransomware
2. ETA for Cyprogrpahic compliance audit -- used to identify the protocol version or cipher suites
