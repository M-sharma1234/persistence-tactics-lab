# Persistence Tactics Lab

## Overview
This lab demonstrates simulated Linux persistence techniques used by attackers to maintain access to compromised systems.  
The purpose is for cybersecurity learning and research — **do not use maliciously**.

---

## Techniques Demonstrated
1. **Cron Jobs**
   - Scheduled a malicious script to run at boot.
   - Simulated persistence via task scheduling.

2. **Reverse Shell**
   - Simulated an attacker connecting back to a remote system.
   - Used `nc` (netcat) to demonstrate.

3. **Timestomping**
   - Modified file timestamps to evade detection.

---

## Lab Setup
- **OS**: Ubuntu 20.04 (VM)
- **Tools Used**: bash, cron, netcat, touch
- **Network**: Isolated lab network

---

## Steps Performed
1. Created a simple bash payload.
2. Configured a cron job to execute the payload.
3. Set up a netcat listener to receive reverse shell.
4. Changed timestamps of files to hide activity.
5. Monitored logs to observe attacker activity.

---

## Detection & Mitigation
- **Detection**: Used `ps`, `netstat`, and log inspection to find abnormal processes and connections.
- **Mitigation**: Removed cron jobs, killed malicious processes, restored original timestamps.

---

## Disclaimer
This project is for educational purposes only.  
Any misuse is strictly prohibited.


