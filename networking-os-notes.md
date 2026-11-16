# Technical Reference & Study Notes
*Compiled from TryHackMe & Cisco Networking Academy*

---

## 1. Networking Fundamentals & Architecture
* **Internet Service Providers (ISPs):** Act as the bridge connecting home and corporate networks to the global internet backbone via technologies like subsea fiber-optic cables.
* **IP vs. MAC Addresses:**
  * **MAC Address:** Permanent physical hardware fingerprint; never changes.
  * **IP Address:** Network-assigned and location-dependent. Configurable via `fastEthernet` or checked via `ipconfig` / terminal tools.
* **Core Network Components:**
  * **Default Gateway:** A Layer 3 routing device on a local subnet providing an exit point for traffic destined for remote networks (the internet).
  * **DHCP (Dynamic Host Configuration Protocol):** Automatically assigns IP addresses to devices.
  * **Subnet Mask:** Differentiates the host portion (specific device) from the network ID portion (shared local network area).
* **Data Transmission:** 
  * Measured through **Bandwidth** (medium capacity), **Throughput** (actual data transfer rate over time), and **Latency** (delay in transit).
  * Transmitted via electrical signals (copper wire), optical signals (light pulses/fiber optics), or wireless signals (radio/microwaves).

---

## 2. Operating Systems & Linux CLI Basics
Essential terminal commands for system navigation and resource inspection:
* `pwd`: Print Working Directory.
* `ls` / `ls -l` / `ls -al`: List directory contents, detailed attributes, and hidden files.
* `cd [path]` / `cd ..`: Change directory and move back a level.
* `find <starting-point> -name <filename>`: Locate files in the file system.
* `cat`: Read file contents.
* `whoami` & `uname -a`: Display current user and full system architecture info.
* `df -h`: Check disk storage usage in human-readable format.

---

## 3. Virtualization & Cloud Computing
* **Virtualization:** Allows a single physical computer to act as multiple isolated systems using a **Hypervisor**:
  * *Type 1:* Runs directly on physical hardware (efficient, enterprise-grade).
  * *Type 2:* Runs within an existing OS (e.g., VirtualBox, VMware) for testing and learning.
* **Containers vs. VMs:** Containers (like Docker) share the host OS kernel, making them lightweight and fast to spin up, whereas VMs emulate an entire operating system.
* **Cloud Service Models:**
  * **IaaS:** Infrastructure as a Service (virtualized compute, storage, networking like AWS EC2).
  * **PaaS:** Platform as a Service (on-demand development and testing environments).
  * **SaaS:** Software as a Service (cloud-delivered applications).

---

## 4. Security Concepts
* **Offensive Security:** Proactively thinking like an attacker to find vulnerabilities before malicious actors do (e.g., using enumeration tools like DirBuster to find hidden directories).
* **Defensive Security:** Monitoring, investigating, and stopping attacks via Security Operations Centers (SOC), SIEM monitoring, Malware Analysis, and Digital Forensics & Incident Response (DFIR).
