## Network Port Scanning Task

**Author:** Harsh Gupta  
**Date:** June 23, 2025

---

### **Overview**

This repository contains documentation and steps for scanning your local network to discover open ports on connected devices. The goal is to understand network exposure and identify potentially vulnerable services.

---

### **Objective**

- Learn how to scan your local network for open ports.
- Assess the exposure of devices and understand possible security risks.

---

### **Tools Used**

- **Nmap:** A powerful network mapping tool (pre-installed on Kali Linux).
- **Wireshark (optional):** For deeper network traffic analysis.

---

### **Instructions**

1. **Identify Your Local IP Address**
   - Run the following command to find your IP address:
     ```bash
     ifconfig
     ```
   - Example output: `192.168.26.130`

2. **Scan the Network for Open Ports**
   - Use Nmap to scan your subnet (replace with your actual subnet):
     ```bash
     nmap -sS 192.168.26.0/24
     ```
   - The `-sS` flag performs a stealth SYN scan.

3. **Analyze Scan Results**
   - Review the open ports and associated services.
   - Example: If you find a service like `iad2` (a Cisco service), research known vulnerabilities (e.g., CVEs) and assess the risk of exploitation, such as Denial of Service (DoS) attacks.

4. **Repeat for Other Services**
   - Investigate each open port/service for potential vulnerabilities to ensure network security.

---

### **Disclaimer**

This task is intended for educational purposes on networks you own or have permission to scan. Unauthorized scanning may violate laws or terms of service.

---

### **File Structure**

- `task1.docx`: Step-by-step documentation for the port scanning task.

---

### **References**

- [Nmap Documentation](https://nmap.org/book/man.html)
- [Wireshark User Guide](https://www.wireshark.org/docs/wsug_html_chunked/)

---

**Feel free to contribute or raise issues for improvements!**

[1] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/69317259/62dabdba-a20a-4aef-b4b5-500696494f5d/task1.docx
