# HSKim's Portfolio

> **DevOps · Solution Development · Infrastructure Monitoring Engineer**

I specialize in infrastructure monitoring, DevOps, and solution development, with hands-on experience across the entire service lifecycle:

**Infrastructure Design → Architecture Analysis → Application Development → Deployment → Customer Implementation → Troubleshooting → Operations**

Currently, I work as a PRTG-based NMS engineer while also developing enterprise SaaS and On-Premise solutions using Java/Spring and Django.

My experience also includes AI-assisted architecture analysis and AX projects, Docker/Kubernetes-based infrastructure, Windows client integration with Electron, and monitoring solution development.

I aim to bridge the gap between **infrastructure, software development, and operations**.

---

## :pushpin: Profile

- **PRTG Engineer / Network & Infrastructure Engineer**
- **DevOps / Solution Engineer**
- **Backend & Monitoring Solution Developer**
- **AX / AI-assisted Development**
- PRTG Sales Professional
- PRTG Monitoring Expert
- HPE Aruba ACA-CA

> **Better Than Yesterday**

---

## :hammer_and_wrench: Core Competencies

### Solution Development

`Java` `Spring Boot` `Spring Security` `JSP` `Python` `Django` `REST API` `Electron`

- Enterprise web application design and development
- SaaS and On-Premise solution development
- REST API and external system integration
- Windows desktop agent development
- Legacy system analysis and stabilization
- Customer-specific application customization

### DevOps & Infrastructure

`Linux` `Docker` `Docker Compose` `Kubernetes` `containerd` `GitLab` `Git` `VMware` `Naver Cloud`

- Application deployment and operations
- Container-based application packaging
- Kubernetes cluster deployment and troubleshooting
- Cloud and isolated internal-network environments
- Customer-specific release and version management

### Monitoring & Network

`PRTG` `SNMP` `SSH` `TCP/IP` `PowerShell` `Net-SNMP` `Aruba` `SAN / FC`

- Network / Server / Storage Monitoring
- SNMP MIB and OID analysis
- PRTG Custom Sensor development
- SAN Switch monitoring
- Network failure and traffic analysis
- Customer monitoring system design and deployment

### Database

`PostgreSQL` `MySQL` `MSSQL` `Oracle` `MS Access` `Redis`

- Database schema and table design
- Multi-database integration
- Legacy database integration
- Cache and asynchronous data processing

### AI & AX

`Dify` `Ollama` `LLM` `n8n`

- Internal LLM platform deployment
- Knowledge Base / RAG pipeline implementation
- AI-based legacy architecture analysis
- AI-assisted software development workflows
- LLM-based data analysis and automation

---

# :office: Professional Projects

## 1. T Solution — Enterprise Workforce Management Platform

> Internal company solution / Source Code Private

T Solution is an enterprise workforce management platform for managing attendance, leave, work schedules, shifts, HR information, and related operational data.

The platform supports both **Cloud SaaS** and **On-Premise deployments in customer internal networks**.

I participate across the entire project lifecycle, including backend development, desktop agent development, external HR integration, customer deployment, troubleshooting, and operations.

### Responsibilities

- Developed backend services and business logic using Java and Spring Boot
- Developed and maintained JSP-based web application functionality
- Developed SQL and data-processing logic using PostgreSQL
- Managed authentication and authorization using Spring Security and JWT
- Implemented customer-specific application functionality
- Performed bug analysis, troubleshooting, and feature improvements
- Managed application build, deployment, and operations
- Operated SaaS environments on Naver Cloud
- Deployed and maintained On-Premise environments inside customer networks
- Managed customer-specific branches and releases
- Integrated external HR and ERP systems
- Implemented multi-database integration

### Architecture

```text
Browser
   │
   ▼
T Solution-web
Spring Boot + JSP
   │
   ▼
T Solution-core
Service / DAO / Security / Business Logic
   │
   ├── PostgreSQL
   ├── MSSQL
   ├── MySQL
   └── MS Access

T Solution-hr-syncer
   │
   ├── REST API
   └── External HR Database

Electron Agent
   │
   ├── Windows OS Control
   ├── Push Notification
   ├── Auto Update
   └── Server Communication
```

### Electron Desktop Agent

Developed and maintained an Electron-based Windows background agent that connects the client operating system with the web application.

Main capabilities include:

- Windows background process / system tray agent
- Automatic startup on Windows login
- Firebase Cloud Messaging push notifications
- Automatic software updates
- PC lock-state detection
- Communication between the web application and client operating system

### HR / External System Integration

Integrated external HR and access-control systems through REST APIs and direct database access.

```text
Flexteam
    ↓ REST API / OAuth

HR Sync Module
    ↓

T Solution

HR / ERP Database
    ↑ DB Integration
```

### Customer Deployment & Operations

Managed both shared Cloud versions and customer-specific Custom versions.

Responsibilities included:

- Customer requirement analysis
- Custom feature development
- Customer-specific database environment handling
- On-Premise internal-network deployment
- Release and version management
- Troubleshooting and incident response
- Maintenance and operational support

### Tech Stack

`Java 21` `Spring Boot` `Spring Security` `JSP` `MyBatis`  
`PostgreSQL` `MSSQL` `MySQL` `MS Access`  
`JWT` `LDAP` `WebSocket` `STOMP` `Quartz`  
`Electron` `Firebase Cloud Messaging`  
`Docker` `Gradle` `Naver Cloud`

---

## 2. SAN Solution — SAN Switch Monitoring Solution

> **Architecture / Backend / Data Collection / Deployment — Solo Development**  
> Internal company project / Source Code Private

SAN:Solution is a dedicated SAN Switch monitoring solution that collects and visualizes device status, port information, connected devices, zoning configurations, and performance metrics using SNMP and SSH.

I independently designed and developed the solution from architecture to production deployment.

### Key Features

- SAN Switch automatic discovery
- SNMP-based device and port data collection
- SSH-based Brocade CLI data collection
- FC Port automatic discovery
- Name Server data collection
- WWN-based connected-device identification
- Port Neighbor mapping
- SAN Fabric topology generation
- Zone / Zone Member collection
- CPU / Memory monitoring
- Port Traffic monitoring
- SFP status and performance collection
- Monitoring dashboard

### Data Collection Architecture

```text
SAN Switch
   │
   ├── SNMP
   │     ├── Device Health
   │     ├── Port Discovery
   │     ├── Traffic
   │     └── SFP
   │
   └── SSH
         ├── switchshow
         ├── nsshow
         └── cfgshow

              ↓

       Collector Layer

              ↓

    Normalize / Parse Data

              ↓

       PostgreSQL
              │
              ▼
        Django REST API
              │
              ▼
         Web Dashboard
```

### Asynchronous Monitoring Architecture

```text
Celery Beat
     ↓
Scheduler
     ↓
Celery Worker
     ↓
Device Collector
     ↓
SNMP / SSH
     ↓
PostgreSQL
```

Redis and Celery are used to periodically collect device information.

The collector structure was designed to allow monitoring functions to be extended independently.

### Responsibilities

- Designed the overall application architecture
- Developed the Django backend
- Developed REST APIs using Django REST Framework
- Designed the PostgreSQL database schema
- Developed SNMP communication and collection modules
- Developed SSH communication and CLI parsers
- Implemented SAN Port Discovery logic
- Implemented WWN normalization and device mapping
- Designed Fabric and Zone data structures
- Implemented network topology generation
- Developed asynchronous collection using Celery and Redis
- Developed monitoring dashboards
- Deployed the application to Linux production environments
- Configured Gunicorn and Nginx services
- Performed troubleshooting and operations

### Tech Stack

`Python` `Django 5` `Django REST Framework`  
`PostgreSQL` `Redis` `Celery`  
`SNMP` `pysnmp` `SSH` `Paramiko`  
`JavaScript` `Chart.js`  
`Gunicorn` `Nginx` `Linux`

---

## 3. PRTG-Based Enterprise Infrastructure Monitoring

Implemented and operated PRTG-based monitoring environments for customer and internal infrastructure.

### Responsibilities

- Server and network device discovery
- SNMP / Ping / Traffic sensor configuration
- Aruba Controller / AP monitoring
- Server / Storage monitoring
- Monitoring threshold design
- Notification policy configuration
- Active Directory integration
- User and group permission management
- PRTG Custom Sensor development
- Customer POC and technical support
- Network failure and traffic analysis
- Windows Event Log / PRTG Log analysis
- Partner technical and sales support

### Tech Stack

`PRTG` `SNMP` `TCP/IP` `Windows Server`  
`Linux` `PowerShell` `Active Directory`  
`Aruba` `VMware`

---

## 4. PRTG Custom Monitoring Sensor Development

Developed custom monitoring sensors using PowerShell and SNMP for infrastructure and applications not fully supported by standard PRTG sensors.

### Printer Monitoring

Analyzed RFC 3805 Printer-MIB and developed custom monitoring for:

- Printer cover status
- Total page count
- Consumable status
- Device status

`PowerShell` `Net-SNMP` `PRTG EXE/Script Advanced` `XML`

### Aruba CX Hardware Monitoring

Developed custom monitoring for Aruba CX Switch hardware status.

Monitoring items include:

- CPU
- Memory
- Interface
- Module Health
- NAE
- NTP
- PSU
- VSF
- VSX

### JEUS Monitoring

Developed monitoring functions for JEUS application server runtime resources.

Monitoring items include:

- CPU
- Memory
- Heap Memory
- Processor
- Thread
- Uptime

---

## 5. AI-Based Monitoring Dashboard

Developed a dashboard integrating PRTG monitoring data with LLM-based analysis.

### Architecture

```text
PRTG
  ↓
Monitoring Data
  ↓
Node.js / JavaScript
  ↓
Dify
  ↓
LLM Analysis
  ↓
Dashboard
```

### Tech Stack

`Node.js` `JavaScript` `PRTG` `Dify` `LLM`

---

## 6. Private LLM Platform Using Dify & Ollama

Built an internal LLM environment using Dify and Ollama to reduce dependency on external LLM APIs and enable secure use of internal data.

### Responsibilities

- Deployed Dify using Docker Compose
- Built and operated an Ollama model server
- Configured PostgreSQL and Redis
- Configured Dify Plugin Daemon services
- Built Knowledge Bases
- Implemented RAG pipelines
- Developed Excel / CSV data-analysis workflows
- Implemented LLM and Code Node-based data normalization
- Developed attendance-data aggregation workflows
- Troubleshot container networking issues
- Analyzed plugin and API connectivity problems

### Architecture

```text
User
 ↓
Dify
 ↓
Knowledge Base
 ↓
LLM / Code Node
 ↓
Ollama
 ↓
Private LLM
```

### Tech Stack

`Dify` `Ollama` `LLM` `Docker Compose`  
`PostgreSQL` `Redis` `Python`

---

## 7. AX — AI-Assisted Software Development

Performed an AX project focused on using AI to analyze and stabilize existing software architecture and improve the software development process.

The goal was not simply to generate code with AI, but to structure the project so AI could understand the existing system architecture and participate reliably in development.

### Responsibilities

- Analyzed legacy project structures
- Analyzed module dependencies
- Analyzed application architecture
- Reorganized codebase structure
- Established development conventions
- Prepared architecture and project-context documentation for AI
- Analyzed build and test structures
- Stabilized existing code
- Established AI-assisted development workflows

### Development Flow

```text
Existing System
      ↓
Architecture Analysis
      ↓
Project Context Structuring
      ↓
Development Rules / Conventions
      ↓
AI-Assisted Development
      ↓
Validation / Stabilization
```

---

## 8. Kubernetes-Based Container Platform

Built and operated Kubernetes environments for container-based application deployment and infrastructure experimentation.

### Responsibilities

- Built Kubernetes clusters using kubeadm
- Configured containerd as the container runtime
- Installed and configured Flannel CNI
- Configured CoreDNS
- Troubleshot Pod networking issues
- Monitored Kubernetes Pods and Services
- Evaluated migration from Docker-based services to Kubernetes
- Configured and troubleshot NVIDIA GPU runtime environments

### Tech Stack

`Kubernetes` `Docker` `containerd` `Flannel`  
`Linux` `Ubuntu` `Rocky Linux`

---

# :school: Team Projects

## Bello — IoT / Real-Time Communication Platform

**Five-member team project**

### Responsibilities

- Designed MySQL database architecture
- Designed table relationships
- Configured triggers and constraints
- Implemented real-time communication using Spring WebSocket
- Managed application server deployment and operations

### Tech Stack

`Java 8` `Spring 4` `Maven` `WebSocket`  
`Python` `Flask` `JavaScript` `MySQL`  
`HTML` `CSS` `Raspberry Pi` `OpenCV`  
`Picamera2` `RPi.GPIO`

**Development Period:** January 4, 2024 – January 15, 2024

---

## YEAHA — Data / Machine Learning Service

**Five-member team project**

### Responsibilities

- Designed and managed the database schema
- Created database documentation
- Collected public healthcare and food-safety API data
- Compared machine-learning algorithm performance
- Converted ML algorithms into reusable functions
- Developed backend controller logic
- Integrated frontend and backend components

### Tech Stack

`Java 8` `Spring 4` `Python` `Flask`  
`JavaScript` `MySQL` `HTML` `CSS`

**Development Period:** February 26, 2024 – March 13, 2024

---

# :computer: Tech Stack

## Backend

`Java` `Spring Boot` `Spring Framework`  
`Python` `Django` `Django REST Framework`  
`Node.js`

## Database & Cache

`PostgreSQL` `MySQL` `MSSQL` `Oracle`  
`MS Access` `Redis`

## DevOps & Cloud

`Docker` `Docker Compose` `Kubernetes`  
`containerd` `GitLab` `Git`  
`Linux` `VMware` `Naver Cloud`

## Monitoring & Network

`PRTG` `SNMP` `SSH` `TCP/IP`  
`PowerShell` `Net-SNMP`  
`Aruba Network` `SAN / Fibre Channel`

## AI & Automation

`Dify` `Ollama` `LLM` `n8n`

## Frontend / Client

`JSP` `JavaScript` `HTML` `CSS`  
`Electron` `Chart.js`

## Embedded & IoT

`Raspberry Pi` `Arduino` `OpenCV`  
`Picamera2` `RPi.GPIO`

---

# :mailbox: Contact

- **Email**  
  hansoll1215@naver.com

- **GitHub Portfolio**  
  https://github.com/1SSoll2/HSKimPF

- **PRTG Custom Scripts**  
  https://github.com/1SSoll2/scriptsForPRTG

---

> I aim to be an engineer who understands infrastructure, develops production-ready software, and takes responsibility for deployment, troubleshooting, and operations.

<br>

<a href="https://github.com/1SSoll2/HSKimPF">Korean Version Portfolio</a>
