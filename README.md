# University IP Address Management (IPAM)

[![Ansible](https://img.shields.io/badge/Ansible-2.9+-red.svg)](https://www.ansible.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.6+-blue.svg)](https://www.python.org/)

## Project Overview

Complete IP Address Management solution for a **large university** with:

- **4 Buildings** (Main, Engineering, Science, Hostels)
- **15 Floors** across all buildings
- **12 Departments** (Admin, CS, EE, ME, Physics, Chemistry, Biology, Math, etc.)
- **10,000+ Device IP Capacity**
- **3,900+ Students**
- **270+ Staff Members**

---

## 📊 Network Statistics

| Category | Value |
|----------|-------|
| **Buildings** | 4 |
| **Floors** | 15 |
| **Departments** | 12 |
| **Total IP Capacity** | 10,000+ |
| **Students** | 3,900+ |
| **Staff** | 270+ |
| **Subnets** | 20+ |
| **DHCP Pools** | 10+ |

---

## IP Addressing Scheme

### Main Building (10.1.0.0/16)
| Department | Subnet | IP Range | Hosts |
|------------|--------|----------|-------|
| Admin | 10.1.1.0/24 | 10.1.1.1-254 | 254 |
| IT | 10.1.2.0/24 | 10.1.2.1-254 | 254 |
| Library | 10.1.3.0/24 | 10.1.3.1-254 | 254 |
| Auditorium | 10.1.4.0/25 | 10.1.4.1-126 | 126 |
| Staff WiFi | 10.1.10.0/23 | 10.1.10.1-510 | 510 |
| Student WiFi | 10.1.12.0/22 | 10.1.12.1-1022 | 1022 |

### Engineering Block (10.2.0.0/16)
| Department | Subnet | IP Range | Hosts |
|------------|--------|----------|-------|
| Computer Science | 10.2.1.0/24 | 10.2.1.1-254 | 254 |
| Electrical | 10.2.2.0/24 | 10.2.2.1-254 | 254 |
| Mechanical | 10.2.3.0/24 | 10.2.3.1-254 | 254 |
| Civil | 10.2.4.0/25 | 10.2.4.1-126 | 126 |
| Labs Network | 10.2.10.0/23 | 10.2.10.1-510 | 510 |

### Science Block (10.3.0.0/16)
| Department | Subnet | IP Range | Hosts |
|------------|--------|----------|-------|
| Physics | 10.3.1.0/24 | 10.3.1.1-254 | 254 |
| Chemistry | 10.3.2.0/24 | 10.3.2.1-254 | 254 |
| Biology | 10.3.3.0/24 | 10.3.3.1-254 | 254 |
| Mathematics | 10.3.4.0/25 | 10.3.4.1-126 | 126 |

### Hostels (10.4.0.0/16)
| Hostel | Subnet | IP Range | Hosts |
|--------|--------|----------|-------|
| Hostel A | 10.4.1.0/23 | 10.4.1.1-510 | 510 |
| Hostel B | 10.4.3.0/23 | 10.4.3.1-510 | 510 |
| Hostel C | 10.4.5.0/23 | 10.4.5.1-510 | 510 |
| Hostel D | 10.4.7.0/23 | 10.4.7.1-510 | 510 |
| Hostel E | 10.4.9.0/23 | 10.4.9.1-510 | 510 |

### Management Network (10.255.0.0/16)
| Purpose | Subnet | IP Range | Hosts |
|---------|--------|----------|-------|
| Network Devices | 10.255.1.0/24 | 10.255.1.1-254 | 254 |
| Servers | 10.255.2.0/24 | 10.255.2.1-254 | 254 |
| Printers | 10.255.3.0/24 | 10.255.3.1-254 | 254 |
| CCTV | 10.255.4.0/24 | 10.255.4.1-254 | 254 |

---

## Features

### IP Management
- **Subnet Calculator** - Calculate network, broadcast, and usable IPs
- **VLSM Support** - Variable Length Subnet Masking
- **CIDR Notation** - Classless Inter-Domain Routing
- **IP Utilization Tracking** - Monitor used vs available IPs

### DHCP Configuration
- **Scope Definition** - IP ranges for each department
- **Option Configuration** - Gateway, DNS, domain name
- **Lease Management** - Configurable lease times

### DNS Configuration
- **Forward Zones** - Domain to IP resolution
- **Reverse Zones** - IP to domain resolution
- **Record Management** - A, CNAME, MX records

### Reporting
- **IP Allocation Reports** - Complete subnet details
- **Utilization Reports** - Percentage used per subnet
- **Capacity Planning** - Alerts for high utilization

---
### Screenshots

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/d1f2039b-b12c-41d2-8e7f-1a29978f4bc9" />

<img width="960" height="600" alt="image" src="https://github.com/user-attachments/assets/36dbf58c-da35-450a-bfc2-39a8a2c075e2" />

## 📁 Project Structure
