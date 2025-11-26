# 🌐 Azure Hub-and-Spoke Virtual Network Project (AZ-104)

This repository contains a complete **Azure networking environment** deployed entirely using **Azure CLI**.  
It showcases real-world Cloud System Administrator skills including VNet design, network security, routing, load balancing, and automation.

---

## 🏗️ Project Overview

This project implements a full Hub-and-Spoke architecture similar to what you'd see in a production Azure environment.

### 🔧 Components Deployed

#### **Networking**
- Hub VNet + Spoke VNet
- Subnets (Web, App, DB, Firewall, Gateway, Management)
- Network Security Groups (Web / App / DB tiers)
- VNet Peering (with Gateway Transit)
- Public & Private IP address management
- User-Defined Routes (UDRs)

#### **Security**
- Azure Firewall deployed in the Hub VNet
- Forced tunneling through the firewall
- Subnet-level NSG rules
- Segmented workloads across subnets

#### **Load Balancing**
- Azure Load Balancer (L4) for the Web tier
- Application Gateway (L7) for HTTP routing/WAF

#### **Hybrid Networking**
- Azure VPN Gateway
- Local Network Gateway (simulated on-prem)
- S2S VPN Connection

#### **DNS**
- Private DNS Zone (internal.contoso.com)
- Linked to Spoke only
- A-records for internal VM name resolution

---

## 📁 Repository Structure

