# Derar Chekrouni

**Network & Systems Engineer** · Linux · Routing & Switching · Infrastructure Automation

CCNA · ISC2 CC · RHCSA in progress

---

## About

Final-year Master's student in Networks & Embedded Systems at the University of Algiers 1, doing freelance network field work in Oslo on the side.

I like infrastructure that keeps working when parts of it don't. Most of what I build is about that: redundant routing, databases that elect a new leader on their own, provisioning that runs without me touching it, and a home lab designed to survive its own failures while I'm in another country.

Currently studying for the RHCSA.

---

## Projects

### Multi-Site IaaS Provider Infrastructure
[GitHub](https://github.com/Mothrxa/Multi-Site-IaaS-Provider-Infrastructure) · [Report](https://github.com/Mothrxa/Multi-Site-IaaS-Provider-Infrastructure/blob/main/Report.pdf)

| **Tech** | GNS3, Containerlab, Cisco IOS/IOL, Arista cEOS, pfSense, OSPF, IPsec, Ansible, Terraform, KVM/libvirt, Docker |
|---|---|
| **My role** | Network, systems and automation (team of 2) |
| **Domain** | Network Infrastructure · Cloud · Automation |

Network and systems infrastructure for Strata, a fictional IaaS provider with two sites: a corporate headquarters and a cloud datacenter, linked over an untrusted ISP transit.

- Site-to-site IPsec VPN terminated on pfSense at each perimeter, with multi-area OSPF (area 0 at HQ, area 1 in the datacenter)
- Containerized 2-spine / 4-leaf Clos fabric in the datacenter (Cisco IOL + Arista cEOS) with ECMP, built at full target scale
- HQ campus segmented into IT, HR, BizOps, Data Center, DMZ and Management VLANs. Built single-device-per-tier in GNS3 due to lab resources; the full redundant design (HSRP, LACP, dual firewalls) was validated in Packet Tracer
- BIND9 and ISC DHCP with TSIG dynamic DNS, FreeRADIUS for AAA, Postfix/Dovecot mail, LibreNMS monitoring and centralized logging in Graylog
- A customer signs up on the portal and Terraform provisions a KVM VM (cloud-init, SSH key injection) or a Docker container, exposed publicly through the datacenter NAT gateway
- Ansible playbooks push device config (NTP, SNMP, syslog, STP edge hardening) and web host baselines, with vaulted credentials

---

### Distributed Online Voting Platform
[GitHub](https://github.com/Mothrxa/Distributed-Voting)

| **Tech** | HAProxy, PostgreSQL, Patroni, etcd, Node.js, Nginx, Tailscale VPN |
|---|---|
| **Domain** | Distributed Systems · Infrastructure |

Highly available distributed system built on 12 virtual machines with no single point of failure. Each tier runs behind its own HAProxy load balancer. Failures at any tier don't cascade.

- PostgreSQL + Patroni + etcd for automatic leader election and synchronous replication
- Stateless Node.js backend, horizontally scalable by design
- Resilience validated through live failure scenarios: nodes taken down mid-operation, auto-recovery at every tier

---

### Homelab
[GitHub](https://github.com/Mothrxa/Homelab)

| **Tech** | Raspberry Pi 4, Fedora Server, Pi-hole, Docker, Dockge, Uptime Kuma, Stirling-PDF, Tailscale, Wake-on-LAN |
|---|---|
| **Domain** | Self-Hosting · Linux · Networking |

Self-hosted replacements for paid services, built to run unattended while I'm abroad. Rule of the design: nothing in it should take the house offline if it fails.

- An always-on Raspberry Pi 4 (booting from USB SSD) handles DNS, DHCP and light services; a Fedora Server machine takes heavier workloads and sleeps when idle
- Tailscale can't reach a sleeping host because the tunnel goes down with the OS, so the Pi relays the Wake-on-LAN packet from inside the LAN. Getting there meant replacing a USB NIC that had no WoL support with an RTL8153-based one
- Pi-hole runs DHCP and hands out the router as secondary DNS, so if the Pi dies the house keeps resolving
- Compose stacks are managed with Dockge across both hosts, monitored with Uptime Kuma and reachable over Tailscale

---

## Experience

### IT Support & Network Engineer
*QIT Solutions 247 · Freelance · Oslo, Norway · Jun 2026 - Sep 2026*

- On-site IT support
- Network device installation in offices and data centers
- Issue troubleshooting (hardware/software/network)

---

## Education & Certifications

| | |
|---|---|
| **Master's, Networks & Embedded Systems** | University of Algiers 1 · 2025 - 2027 |
| **Bachelor's, Computer Science** | University of Algiers 1 · 2022 - 2025 |
| **Cisco Certified Network Associate (CCNA)** | April 2026 |
| **ISC2 Certified in Cybersecurity (CC)** | July 2026 |
| **Red Hat Certified System Administrator (RHCSA)** | In progress |
| **TryHackMe** | Legend rank (top 1%) |

**Languages:** Arabic (native) · French (fluent) · English (fluent) · Norwegian (learning)

---

## Contact

[![Email](https://img.shields.io/badge/Email-chekrouni.derar@gmail.com-D14836?style=flat&logo=gmail&logoColor=white)](mailto:chekrouni.derar@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Derar%20Chekrouni-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/derar-chekrouni/)
[![GitHub](https://img.shields.io/badge/GitHub-Mothrxa-181717?style=flat&logo=github)](https://github.com/Mothrxa)
