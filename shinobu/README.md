# shinobu - Home NAS & Network Server

Repurposed a 2014 ASUS Q551LN Laptop into a home server running Ubuntu Server. 
Part of my "Hashira" home lab

# Goals
- Network file storage (NAS)
- Network-wide ad blocking (pi-hole)
- VPN for remote access

# Hardware
ASUS Q551LN (i7 - 451OU, 8GB DDR3L)
128GB SATA SSD - 1TB HDD optical bay caddy (replaced DVD Drive) 
Runs on AC only

# 1. Hardware Prep
- checked specs with powershell
- removed the battery, swapped the HDD for an SSD for the boot drive, and moved the HDD to the DVD Drive

# 2. OS Install
- flashed Ubuntu server onto a USB with Rufus
- installed to the SSD with LVM, and enabled OpenSSH

# 3. Post-Install Configuration
- expanded the root volume since the installer allocated only 58GB of the SSD
- disabled suspend on lid close /etc/systemd/logind.conf


### Remote management
- SSH from Windows workstation
- Cockpit web dashboard on port 9090

## 4. Storage — in progress
## 5. Samba file sharing — planned
## 6. Pi-hole — planned

## Lessons learned
- broke the battery connector, since we are not using a battery on it it's okay 
