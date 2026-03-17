<div align="center">
  <h1>PI System & Network Project</h1>
  <h3>TechSolutions SARL – Enterprise Network Infrastructure</h3>
  <p><strong>ESPRIT • Academic Year 2025–2026</strong></p>
</div>

---

## 📌 Repository Content

- **Full Team Report** → [`HH-4_Final_Documentation.pdf`](Final_Documentation.pdf)
- **My Personal Module** → [`Yassine-Arfaoui_My-Module.pdf`](Yassine-Arfaoui_My-Module.pdf) ← **(Yassine Arfaoui)**
- Screenshots & configs

---

*(rest of your previous README stays the same)*

---

## 📋 Project Overview

Complete design, implementation, and securing of a **multiservice enterprise network** for **TechSolutions SARL** using professional standards.

The infrastructure includes:
- Full-mesh OSPF backbone for redundancy
- VLSM IP addressing plan
- 4 departmental zones (Web, IT, Database, Collaboration)
- Production services: Apache Web, MySQL, NFS File Sharing
- Centralized monitoring with Prometheus + Grafana
- Security layer: Extended ACLs, GRE tunnels, UFW firewalls

---

## 🛠 Technologies Used

| Layer              | Technologies                              |
|--------------------|-------------------------------------------|
| Simulation         | GNS3 + Cisco IOS routers                  |
| Routing            | OSPF (Area 0) + GRE tunnels               |
| Addressing         | VLSM                                      |
| Web                | Apache2                                   |
| Database           | MySQL Community Server                    |
| File Sharing       | NFS (Kernel Server)                       |
| Monitoring         | Prometheus + Node Exporter + Grafana      |
| Security           | Extended ACLs, UFW, GRE                   |
| OS                 | Ubuntu 22.04 LTS (Linux VMs)              |

---

## 📐 Network Architecture

**Full-mesh OSPF backbone** interconnecting 4 departmental routers + central BB router.

![Global Architecture](screenshots/figure1-global-architecture.png)

**IP Addressing Plan (VLSM)**

| Department      | Subnet          | Network          | Usable Range              |
|-----------------|-----------------|------------------|---------------------------|
| Backbone        | /26             | 192.168.43.0     | .1 – .62                  |
| Web/Marketing   | /19             | 192.168.0.0      | .1 – 31.254               |
| IT/Monitoring   | /21             | 192.168.32.0     | .1 – 39.254               |
| Database        | /23             | 192.168.40.0     | .1 – 41.254               |
| Collaboration   | /24             | 192.168.42.0     | .1 – .254                 |

---

## 📚 Project Phases

### Phase 1 – Network Core
- Backbone physical & logical design
- OSPF configuration + GRE UDP tunnel
- VLSM + DHCP

### Phase 2 – Services Deployment
- Apache Web Server (Marketing)
- MySQL Database (Management)
- NFS File Sharing (Collaboration)
- Prometheus + Grafana Monitoring (IT)

### Phase 3 – Security & Hardening
- Extended ACLs on backbone
- UFW firewall rules on all servers
- GRE secure tunneling
- Server-level protection

---

## 📊 Results & Validation

- 100% OSPF neighbor adjacency
- Full inter-department connectivity
- All services reachable with ACL restrictions
- Real-time monitoring dashboards
- Secure remote access validated

**Full 34-page technical report** → [`HH-4_Final_Documentation.pdf`](Final_Documentation.pdf)

---

## 👥 Team

- **Ryma Yahmadi**
- **Seif Meddeb**
- **Hiba Dkhil**
- **Yesmine Kacem**
- **Yassine Arfaoui** (me)

  ## 👤 My Individual Contribution (Yassine Arfaoui)

**Module Focus:** [Write 1 short line here – e.g. "Security Implementation (Phase 3) + Monitoring Service + ACLs & GRE Tunneling"]

📄 **My dedicated module documentation** (only my part):

[📥 Download Yassine-Arfaoui_My-Module.pdf](Yassine-Arfaoui_My-Module.pdf)

---

## 📚 Full Team Documentation
[📥 Download Complete 34-page Final Report (HH-4.pdf)](HH-4_Final_Documentation.pdf)

**Supervised by**  
- Nawal Hamdi  
- Ryhem Matoussi

---

## 🎓 Skills Demonstrated

Network Design • Dynamic Routing (OSPF) • VLSM • Linux Services • Firewalling • Monitoring • Project Documentation • Team Collaboration

---

## 📬 How to Explore

1. Download the [PDF report](Final_Documentation.pdf)
2. Look at `configs/` for router & Linux configuration files

---

<div align="center">
  <strong>Made with ❤️ at ESPRIT – Tunis</strong><br>
  Academic Year 2025–2026
</div>
