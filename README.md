# HSKim's Portfolio

> **DevOps · Solution Development · Infrastructure Monitoring Engineer**

네트워크 및 시스템 모니터링을 기반으로  
**인프라 구축 → 아키텍처 분석 → 애플리케이션 개발 → 배포 → 고객사 구축 → 장애 대응 → 운영**까지  
서비스 전체 라이프사이클을 경험하고 있습니다.

현재 **PRTG 기반 NMS 엔지니어링 및 기술 지원**을 담당하면서,  
Java/Spring 기반 기업용 SaaS·On-Premise 솔루션과 Django 기반 모니터링 솔루션을 직접 개발하고 있습니다.

또한 AI를 활용한 기존 시스템 분석 및 AX 프로젝트, Docker/Kubernetes 기반 서비스 운영,  
Electron Agent를 이용한 Windows OS 제어 및 서버 통신 등  
**개발과 인프라의 경계를 연결하는 엔지니어링**을 지향합니다.

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

- 기업용 웹 서비스 설계 및 개발
- SaaS / On-Premise 환경 대응
- REST API 및 시스템 연동 개발
- Windows Desktop Agent 개발
- 레거시 시스템 분석 및 기능 개선
- 고객사별 Custom 기능 개발

### DevOps & Infrastructure

`Linux` `Docker` `Docker Compose` `Kubernetes` `containerd` `GitLab` `Git` `VMware` `Naver Cloud`

- 애플리케이션 배포 및 운영
- Docker 기반 서비스 패키징
- Kubernetes 클러스터 구축 및 트러블슈팅
- Cloud / 내부망 배포 환경 구성
- 고객사별 릴리즈 및 형상관리

### Monitoring & Network

`PRTG` `SNMP` `SSH` `TCP/IP` `PowerShell` `Net-SNMP` `Aruba` `SAN / FC`

- Network / Server / Storage Monitoring
- SNMP MIB 및 OID 분석
- PRTG Custom Sensor 개발
- SAN Switch 모니터링
- 네트워크 장애 및 트래픽 분석
- 고객사 모니터링 시스템 설계 및 구축

### Database

`PostgreSQL` `MySQL` `MSSQL` `Oracle` `MS Access` `Redis`

- 데이터베이스 모델 및 테이블 설계
- Multi-DB 환경 연동
- Legacy DB 연동
- Cache 및 비동기 처리 구조 설계

### AI & AX

`Dify` `Ollama` `LLM` `n8n`

- 사내 LLM 환경 구축
- Knowledge Base / RAG Pipeline 구성
- AI 기반 기존 프로젝트 Architecture 분석
- AI-assisted Development Workflow 구축
- LLM 기반 데이터 분석 및 자동화

---

# :office: Professional Projects

## 1. T 솔루션 — 기업용 근태관리 플랫폼

> 회사 자체 솔루션 / Source Code Private

기업의 **근태, 연차, 스케줄, 교대근무 및 HR 데이터**를 통합 관리하는 웹 기반 기업용 근태관리 시스템입니다.

Cloud 기반 SaaS 서비스와 고객사 내부망에 구축되는 On-Premise 환경을 모두 지원하며,  
웹 애플리케이션 개발부터 Windows Agent, 외부 HR 시스템 연동, 고객사 구축 및 운영까지 프로젝트 전반을 수행하고 있습니다.

### 주요 역할

- Java / Spring Boot 기반 Backend 및 Business Logic 개발
- JSP 기반 Web Application 기능 개발 및 유지보수
- PostgreSQL 기반 데이터 처리 및 SQL 개발
- Spring Security / JWT 기반 인증·인가 구조 관리
- 고객사 요구사항에 따른 기능 Customizing
- 버그 분석 및 기능 개선
- 서비스 Build / Deploy / Operation
- Naver Cloud 기반 SaaS 서비스 운영
- 고객사 폐쇄망 On-Premise 구축 및 유지보수
- 고객사별 Branch / Release 관리
- 외부 HR 및 ERP 시스템 데이터 연동
- Multi-DB 환경 연동

### Architecture

```text
Browser
   │
   ▼
솔루션-web
Spring Boot + JSP
   │
   ▼
솔루션-core
Service / DAO / Security / Business Logic
   │
   ├── PostgreSQL
   ├── MSSQL
   ├── MySQL
   └── MS Access

솔루션-hr-syncer
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

Windows Client 환경과 서버를 연결하는 Electron 기반 Agent를 함께 개발 및 운영하고 있습니다.

- Windows Background / System Tray Agent
- Windows 로그인 시 자동 실행
- Firebase Cloud Messaging 기반 Push Notification
- Agent 자동 업데이트
- PC Lock 상태 감지
- Web Application과 Client OS 간 연동

### HR / External System Integration

외부 인사 및 출입 시스템과의 데이터 연동 기능을 개발했습니다.

```text
Flexteam
    ↓ REST API / OAuth

HR Sync Module
    ↓

솔루션

HR / ERP Database
    ↑ DB Integration
```

### 고객사 관리

Cloud 공통 버전과 고객사별 Custom 버전을 분리하여 관리하며,

- 고객사별 요구사항 분석
- Custom 기능 개발
- DB 환경 차이 대응
- 내부망 환경 구축
- 배포 및 버전 관리
- 장애 대응
- 유지보수

까지 수행하고 있습니다.

### Tech Stack

`Java 21` `Spring Boot` `Spring Security` `JSP` `MyBatis`  
`PostgreSQL` `MSSQL` `MySQL` `MS Access`  
`JWT` `LDAP` `WebSocket` `STOMP` `Quartz`  
`Electron` `Firebase Cloud Messaging`  
`Docker` `Gradle` `Naver Cloud`

---

## 2. SAN 솔루션 — SAN Switch Monitoring Solution

> **Architecture / Backend / Data Collection / Deployment — Solo Development**  
> 회사 내부 프로젝트 / Source Code Private

Brocade 등 FC 기반 SAN Switch를 대상으로  
**SNMP 및 SSH를 이용해 장비·포트·연결 장비·Zoning·성능 데이터를 자동 수집하고 시각화하는 전용 모니터링 솔루션**을 단독 설계·개발했습니다.

### 주요 기능

- SAN Switch 자동 Discovery
- SNMP 기반 장비 및 Port 정보 수집
- SSH 기반 Brocade CLI 데이터 수집
- FC Port 자동 Discovery
- Name Server 정보 수집
- WWN 기반 연결 장비 식별
- Port Neighbor Mapping
- SAN Fabric Topology 구성
- Zone / Zone Member 수집
- CPU / Memory 모니터링
- Port Traffic 모니터링
- SFP 상태 및 성능 정보 수집
- Monitoring Dashboard

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

### 비동기 Monitoring 구조

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

Redis와 Celery를 이용하여 장비 데이터를 주기적으로 수집하고,  
각 Collector를 독립적인 구조로 설계하여 모니터링 항목을 확장할 수 있도록 구성했습니다.

### 담당 영역

- 전체 Application Architecture 설계
- Django Backend 개발
- Django REST Framework API 개발
- PostgreSQL Database 설계
- SNMP Client 및 Collector 개발
- SSH Client 및 CLI Parser 개발
- SAN Port Discovery 로직 개발
- WWN 정규화 및 Device Mapping
- Fabric / Zone 데이터 구조 설계
- Topology 생성 로직 구현
- Celery + Redis 기반 비동기 수집 구조 개발
- Dashboard 개발
- Linux Production 환경 배포
- Gunicorn / Nginx 서비스 구성
- 장애 분석 및 운영

### Tech Stack

`Python` `Django 5` `Django REST Framework`  
`PostgreSQL` `Redis` `Celery`  
`SNMP` `pysnmp` `SSH` `Paramiko`  
`JavaScript` `Chart.js`  
`Gunicorn` `Nginx` `Linux`

---

## 3. PRTG 기반 Enterprise Infrastructure Monitoring

고객사 및 회사 내부 인프라 환경을 대상으로  
PRTG 기반 통합 모니터링 시스템을 설계·구축하고 운영했습니다.

### 담당 업무

- 서버 / Network Device Discovery
- SNMP / Ping / Traffic Sensor 구성
- Aruba Controller / AP Monitoring
- Server / Storage Monitoring
- Monitoring Threshold 설계
- 장애 Notification 정책 구성
- Active Directory 연동
- 사용자 및 Group 권한 구성
- PRTG Custom Sensor 개발
- 고객사 POC 및 기술지원
- 장애 및 Traffic 분석
- Windows Event Log / PRTG Log 분석
- 파트너 기술 및 영업 지원

### Tech Stack

`PRTG` `SNMP` `TCP/IP` `Windows Server`  
`Linux` `PowerShell` `Active Directory`  
`Aruba` `VMware`

---

## 4. PRTG Custom Monitoring Sensor Development

PRTG 기본 Sensor에서 지원하지 않는 장비와 서비스를 모니터링하기 위해  
PowerShell 및 SNMP 기반 Custom Sensor를 개발했습니다.

### Custom Sensor Examples

#### Printer Monitoring

RFC 3805 Printer-MIB를 분석하여 다음 정보를 수집합니다.

- Printer Cover 상태
- Total Page Count
- Consumable 상태
- Device Status

`PowerShell` `Net-SNMP` `PRTG EXE/Script Advanced` `XML`

#### Aruba CX Hardware Monitoring

Aruba CX Switch Hardware 상태를 Custom Sensor로 수집합니다.

- CPU
- Memory
- Interface
- Module Health
- NAE
- NTP
- PSU
- VSF
- VSX

#### JEUS Monitoring

JEUS Application Server의 주요 Runtime Resource를 수집합니다.

- CPU
- Memory
- Heap Memory
- Processor
- Thread
- Uptime

---

## 5. AI-based Monitoring Dashboard

PRTG Monitoring Data와 LLM을 결합하여  
운영 데이터를 보다 쉽게 분석하기 위한 Dashboard를 개발했습니다.

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

## 6. Dify · Ollama 기반 Private LLM Platform

외부 LLM API 의존도를 줄이고 내부 데이터를 안전하게 활용하기 위해  
Dify와 Ollama 기반 사내 LLM 환경을 구축했습니다.

### 담당 업무

- Docker Compose 기반 Dify 배포
- Ollama Model Server 구축
- PostgreSQL / Redis 구성
- Dify Plugin Daemon 구성
- Knowledge Base 구축
- RAG Pipeline 구성
- Excel / CSV 데이터 분석 Workflow 개발
- LLM / Code Node 기반 데이터 정규화
- 근태 데이터 집계 Workflow 구현
- Container Network 장애 분석
- Plugin / API 연결 장애 분석

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

## 7. AX — AI Assisted Software Development

기존 프로젝트의 개발 생산성과 유지보수성을 높이기 위해  
AI를 활용하여 Architecture와 Codebase를 분석하고 개발 프로세스를 정비하는 AX 프로젝트를 수행했습니다.

### 주요 업무

- Legacy Project 구조 분석
- Module Dependency 분석
- Application Architecture 분석
- Codebase 구조 정리
- 개발 Convention 정립
- AI가 프로젝트 Context를 이해할 수 있도록 개발 문서 구성
- Build / Test 구조 분석
- 기존 코드 안정화
- AI Assisted Development Workflow 구성

단순 Code Generation 목적이 아니라,

```text
Existing System
      ↓
Architecture Analysis
      ↓
Project Context Structuring
      ↓
Development Rule / Convention
      ↓
AI Assisted Development
      ↓
Validation / Stabilization
```

형태로 AI를 실제 개발 프로세스에 적용하고 있습니다.

---

## 8. Kubernetes 기반 Container Platform 구축

컨테이너 기반 서비스의 배포 및 운영을 위해 Kubernetes 환경을 직접 구축했습니다.

### 담당 업무

- kubeadm 기반 Cluster 구축
- containerd Runtime 구성
- Flannel CNI 설치
- CoreDNS 구성
- Pod Network 장애 분석
- Kubernetes Service / Pod 상태 점검
- Docker Application의 Kubernetes 전환 검토
- NVIDIA GPU Runtime 환경 구성 및 장애 분석

### Tech Stack

`Kubernetes` `Docker` `containerd` `Flannel`  
`Linux` `Ubuntu` `Rocky Linux`

---

# :school: Team Projects

## Bello — IoT / Real-time Communication Platform

**5인 팀 프로젝트**

### 담당 업무

- MySQL Database Architecture 설계
- Table Relationship 설계
- Trigger 및 Constraint 구성
- Spring WebSocket 기반 실시간 통신 구현
- Application Server 배포 및 운영

### Tech Stack

`Java` `Spring` `MySQL` `WebSocket`

---

## YEAHA — Data / ML Service

**5인 팀 프로젝트**

### 담당 업무

- Database 설계 및 관리
- 공공 API 데이터 수집
- Machine Learning Algorithm 비교
- ML Model 함수화
- Backend Controller 개발
- Frontend / Backend Integration

### Tech Stack

`Python` `Machine Learning` `Java` `Spring` `MySQL`

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

- **GitHub Portfolio**  
  https://github.com/1SSoll2/HSKimPF

- **PRTG Custom Scripts**  
  https://github.com/1SSoll2/scriptsForPRTG

---

> Infrastructure를 이해하고, 직접 서비스를 개발하며,  
> 배포 이후의 장애와 운영까지 책임질 수 있는 엔지니어를 지향합니다.
