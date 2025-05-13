# Cisco Advanced Malware Protection (AMP)
Cisco Advanced Malware Protection (AMP) solutions provide threat intelligence, sandboxing, and real-time malware blocking to prevent breaches.  
AMP monitors all traffic continuously  
It will monitor both good and bad traffic  


It is powered by 3 things
1. Threat Grid
2. Talos
3. Propietary detections and analytics

Cisco AMP for Endpoint (AMP4E)  
![image](https://github.com/user-attachments/assets/8249745a-c3ec-42d6-8d91-98ebda44caba)  

- Network based detections are different than endpoint detections
- Device calculates the hash. It will return status **clean** or **malware** after checks
- File hashes not detected previously return an **unknown** status
- Whe na file is detected in a data stream, it will pull the file and analyze it. If it comes back **clean** it will release it

## Process
![image](https://github.com/user-attachments/assets/93db2300-b093-4a92-8cb6-8a53715ce3ee)
1. The SHA-256 is calculated by the managed device.
2. The managed device checks its cache to see if it has a disposition.
3. If no disposition is found on the local cache, then the SHA-256 is sent to the Cisco Firepower Management Center (FMC), where the Cisco FMC cache is checked.
4. If no disposition is found on the Cisco FMC, then the SHA-256 is sent to Cisco AMP Cloud.
5. Cisco AMP Cloud sends down a disposition and populates the cache of the managed device and the Cisco Firepower Management Center.
