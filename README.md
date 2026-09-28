# operationg-sustems-server-labs
Windows Server 2022 and Ubuntu Linux virtual network labs: Active Directory, Group Policy, DHCP/DNS, IIS, Apache, firewalls, SSH, Samba, Docker and Wireshark traffic analysis. Year 1 Operating Systems, CCT College Dublin.
# 🖥️ Operating Systems – Windows & Linux Server Labs

Two proof-of-concept virtual network projects built for the Operating Systems
module (Year 1, BSc (Hons) Computing & IT, CCT College Dublin, 2024).
Each lab set up and secured a small business network from scratch in
Oracle VirtualBox, based on a fictional client scenario.

---

## 🪟 Lab 1 – Windows Server Active Directory Network

**Scenario:** Setting up domain and web servers for a fictional company, *DigiTech*.

### What I built
- **Two Windows Server 2022 VMs** – a Domain Controller and a Web Server,
  renamed via System Properties and PowerShell, with static IPv4 and DNS
  configuration and verified connectivity
- **Active Directory Domain Services** – new forest and domain, with the web
  server joined to it
- **Users and access control** – Organisational Units for Accounting and Sales,
  global security groups, domain users, and department shared folders with
  NTFS and share permissions (tested by logging in as users from each department)
- **Security policies** – password complexity, history and age rules, plus an
  account lockout policy
- **Web hosting** – IIS installed through PowerShell, a company website hosted,
  and a DNS host record created for it
- **DHCP** – scope, exclusion ranges, 24-hour lease, and a MAC-based address
  reservation, tested with a client picking up its reserved IP
- **Group Policy** – software deployment (.msi) per department, department
  wallpapers, and restricted Control Panel access
- **Research** – patch management best practices (with the 2018 British Airways
  breach as a case study) and Windows Server Update Services (WSUS)

---

## 🐧 Lab 2 – Ubuntu Linux Virtual Network

**Scenario:** An ICT consultancy providing a proof-of-concept network to a
fictional college.

### What I built
- **Two Ubuntu VMs** – a web server and a web client, set up with Host-only
  and NAT network adapters
- **Web server** – Apache hosting a site, accessed from the Linux client
  (Lynx browser) and the Windows host
- **Network management** – permanent hostname changes (`/etc/hostname`,
  `/etc/hosts`) and a static IP address configured with Netplan
- **Secure access** – SSH remote login through PuTTY
- **Firewalls** – rules to allow and block HTTP and SSH traffic with both
  UFW and iptables, tested from the host machine
- **Samba file server** – a shared folder accessible and editable from Windows,
  enabling cross-platform file sharing over SMB
- **Docker** – installed Docker, ran existing container images, and built a
  custom container from a Dockerfile to serve a website
- **Traffic analysis** – used Wireshark to capture ICMP, the TCP three-way
  handshake, and encrypted SSH traffic
- **Research** – Samba and the SMB protocol, and Linux password recovery
  through recovery mode

---

## 🛠️ Tools & Technologies
Windows Server 2022 · Active Directory · Group Policy · DHCP · DNS · IIS ·
PowerShell · Ubuntu Linux · Apache · Netplan · UFW · iptables · SSH · PuTTY ·
Samba · Docker · Wireshark · Oracle VirtualBox

## 📁 Repository Contents
- `windows-lab/` – Windows Server report (PDF) and screenshots
- `linux-lab/` – Linux report (PDF) and screenshots
