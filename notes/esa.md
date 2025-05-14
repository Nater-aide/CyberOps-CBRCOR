# Ciso Email Security Applicance
Protects against phishing, BECs, ransomware, and malware through email.  
![image](https://github.com/user-attachments/assets/efec7a35-c39f-4f89-8bd3-e72cb4c9f3d8)

## Inbound email processing. 
6 Layers of security controls  
1. Threat Prevention with reputation filters
2. Policy Enforcement with message filters
3. Spam detections with antispam
4. Virus Detection with Sophos/Mcafee
5. Content Filters
6. Outbreak Filters

## outbound email processing
Antispam, content filters, and outbreak filters are disabled by default  
DLP scanning can be performed on outgoing messages only  
Reputation filtering is also not used  

## Log Files
Log files can be retrieved using on of the file transfer protocols below
- Manually downloaded -- This is downloaded through the lo subscriptions pages
- FTP Push -- Transferred based on schedule you set
- SCP Push -- pushes files to an SCP server. Requires SSH on the remote computer.
- Syslog Push --RFC 3164. You need a hostname for the syslog server

### Log Subscriptions
- Log Type -- defines type of information of subscription
- Name -- nicnkname
- Rollover by file size
- Rollover by time
- Log Level
- Retrieval method
- Log Filename

### Log Levels
- **Critical**
- **Warning**
- **Informational** -- Captures second by second operations of the system
- **Debug**
- **Trace** -- causes serious degradation and is not recommended for anyone but developers
