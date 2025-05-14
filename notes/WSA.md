# Cisco Web Security Appliance
Cisco WSA runs on CAsyncOS and has 3 software blades
1. Acceptable use policy -- use URL filtering technology
2. Malware Defense -- blocks navigation to bad URLs. Can block against legitimate websites that are compromised. Every piece of content on a site is blocked. It uses the following technologies
  - Web reputation filters
  - Malware scanning
  - HTTPS inspection
  - Layer 4 traffic monitor (L4TM)
3. Data Security

### Explicity proxy deployment
This is when a cleint proxy-aware application has a congifuration area within for proxy settings to declare and use a proxy, such as a WSA.  
This is combined with firewall restricting web traffic that does not originate from teh WSA IP
This assists in tricking applications to use the proxy
Good way to test the Cisco WSA as you deploy it because it doesnt depend on anything else in the network

### Transparent proxy deployment
All port 80 and 443 traffic is redirected to the Cisco WSA by another network device

### WSA Log Types
- AMP engine Logs -- File reputation and file analysis logs
- Audit Logs - records aaa events. User interaction events
- AVC Engine logs -- Debug messages for the AVC engine
- data security logs -- Client history for upload requests that are evaluated by security filters
- Anyconnect secure mobility Daemon Logs -- Interaction between WSA and anyconnect client
- SNMP logs -- debug messages that are related to the SNMP network engine
- Webroot logs -- status of anti-malware scanning activity of the webroot engine
- System Logs -- dns, error, and commit activity

