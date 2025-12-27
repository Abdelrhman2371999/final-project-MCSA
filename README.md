# MCSA Final Project: Secure Multi-Domain Network Infrastructure

## 📁 Project Repository Structure

### **Repository:** `final-project-MCSA`
A comprehensive network security project implementing secure, interconnected Windows Server domains with controlled user access and web services.

---

## 📂 **Project Files Overview**

### **📹 Video Demonstrations**
| File | Description | Purpose |
|------|-------------|---------|
| `DCD1_ADDC.mp4` | Domain Controller 1 Installation | Primary domain controller setup for MCS.Local |
| `DCD2_ADDC_CHILD.mp4` | Domain Controller 2 Installation | Child domain controller setup for Alex.mcs.local |
| `Internet config.mp4` | Network Configuration | Internet and network interface configuration |
| `User.policy@join_to_domin.mp4` | User Policy & Domain Join | User account creation and domain joining procedures |

### **📄 Documentation & Configuration**
| File | Description | Purpose |
|------|-------------|---------|
| `system_use_narrative.docx` | Complete System Documentation | Detailed requirements, scenarios, and architecture |
| `README.md` | Project Overview | Main project documentation |

### **🌐 Web Server Configurations**
| File | Description | Purpose |
|------|-------------|---------|
| `web1.png` | Web1 Server Configuration | HTTPS site binding for MCS.Local |
| `web1.1.png` | Additional Web1 Config | Supplementary web server settings |
| `web2.png` | Web2 Server Configuration | HTTP site binding for Alex.mcs.local |
| `web2.2.png` | Additional Web2 Config | Supplementary web server settings |

---

## 🎯 **Project Objectives Achieved**

### **1. Domain Infrastructure Setup**
- ✅ **Primary Domain**: `MCS.Local` with full AD DS implementation
- ✅ **Child Domain**: `Alex.mcs.local` as subdomain
- ✅ **Trust Relationship**: Bidirectional trust between domains
- ✅ **Domain Controllers**: Two DCs with FSMO roles properly distributed

### **2. Web Services Implementation**
- ✅ **Secure Web Server**: `web1.com` with HTTPS for MCS.Local
- ✅ **Standard Web Server**: `web2.com` with HTTP for Alex.mcs.local
- ✅ **Site Bindings**: Proper IP address, port, and protocol configurations
- ✅ **DNS Integration**: Web servers registered in respective domain DNS zones

### **3. User Management & Security**
- ✅ **User Accounts**: Ahmed (MCS.Local) and Aly (Alex.mcs.local)
- ✅ **Security Policies**: 
  - Control Panel restrictions for Ahmed
  - USB device blocking for Ahmed
  - Desktop branding for Aly
- ✅ **Authentication**: Domain-based login with proper credentials

### **4. Network Services**
- ✅ **DNS Configuration**: Primary/Secondary DNS with redundancy
- ✅ **NTP Services**: Time synchronization across domains
- ✅ **Network Connectivity**: Proper routing and firewall rules

---

## 🔧 **Technical Implementation Details**

### **Active Directory Setup**
- **Forest Creation**: Single forest with multiple domains
- **Domain Controller Promotion**: Using `dcpromo` or Server Manager
- **FSMO Roles**: Proper placement of Operation Master roles
- **Group Policy Objects**: Security policies and user restrictions

### **Web Server Configuration (IIS)**
- **Site Creation**: Individual sites for web1 and web2
- **Binding Configuration**: 
  - web1: Port 443 with SSL certificate
  - web2: Port 80 with HTTP
- **Authentication**: Windows Authentication for domain users
- **Authorization**: Proper access control lists

### **DNS Infrastructure**
- **Forward Lookup Zones**: Separate zones for each domain
- **Resource Records**: A, CNAME, and MX records as needed
- **Conditional Forwarding**: Between domains for name resolution
- **DNS Security**: DNSSEC implementation considerations

### **Security Implementation**
- **User Account Control**: Proper privilege management
- **Device Control Policies**: USB restriction via Group Policy
- **Network Security**: Firewall rules for web traffic
- **Encryption**: SSL/TLS for secure communications

---

## 🎬 **Video Demonstrations Summary**

### **1. Domain Controller Installation**
- **DCD1_ADDC.mp4**: Installation and configuration of first DC
- **DCD2_ADDC_CHILD.mp4**: Child domain DC installation
- **Key Steps**: 
  - Server preparation and network configuration
  - AD DS role installation
  - Forest and domain creation
  - DNS integration

### **2. Network Configuration**
- **Internet config.mp4**: 
  - Network adapter configuration
  - IP address assignment
  - DNS server settings
  - Default gateway configuration

### **3. User and Policy Management**
- **User.policy@join_to_domin.mp4**:
  - User account creation in AD
  - Computer joining to domain
  - Group Policy application
  - Security policy enforcement

---

## 📊 **Testing & Validation**

### **User Scenario Testing**
1. **Ahmed's Access**:
   - Login to MCS.Local domain ✅
   - Access web1.com via HTTPS ✅
   - Control Panel restriction ✅
   - USB device blocking ✅

2. **Aly's Access**:
   - Login to Alex.mcs.local domain ✅
   - Access web2.com via HTTP ✅
   - Company logo on desktop ✅
   - Proper DNS resolution ✅

### **Network Service Testing**
- DNS resolution between domains ✅
- Time synchronization via NTP ✅
- Inter-domain communication ✅
- Web service availability ✅

---

## 🚀 **Getting Started with the Project**

### **Prerequisites**
- Windows Server 2016/2019/2022
- Client machines (Windows 10/11)
- Virtualization platform (Hyper-V, VMware)
- Network isolation for testing

### **Setup Steps**
1. **Watch DCD1_ADDC.mp4** for primary domain setup
2. **Watch DCD2_ADDC_CHILD.mp4** for child domain setup
3. **Configure network** as shown in Internet config.mp4
4. **Set up web servers** using web1.png and web2.png references
5. **Create users and policies** following User.policy@join_to_domin.mp4
6. **Test scenarios** as documented in system_use_narrative.docx

---

## 📈 **Project Statistics**
- **Repository**: final-project-MCSA
- **Created**: Last year
- **Commits**: 4 commits
- **Activity**: Active development and documentation
- **Forks**: 1
- **Watching**: 1

---

## 🔮 **Future Enhancements**
1. **Advanced Security**: Implement two-factor authentication
2. **High Availability**: Add redundant DCs and load balancing
3. **Monitoring**: Implement SCOM or similar monitoring solution
4. **Automation**: PowerShell scripts for deployment
5. **Cloud Integration**: Hybrid Azure AD implementation

---

## 🏆 **Skills Demonstrated**
- ✅ Windows Server Administration
- ✅ Active Directory Domain Services
- ✅ DNS and Network Services
- ✅ IIS Web Server Management
- ✅ Group Policy Implementation
- ✅ Network Security Configuration
- ✅ Documentation and Testing

---

*This project serves as a comprehensive demonstration of MCSA-level skills in Windows Server administration, network security, and domain infrastructure management.*
