# HSKim's PF
>
2024 ~ PRTG Engineer, Network Engineer <br>
PRTG Certificate Sales Professional (2024/9 ~ ), PRTG Certificate Monitoring Expert (2024/10 ~ )<br>
HPE Aruba ACA-CA ( 2025/01 ~ )
>
</br>

## :pushpin: 좌우명
Better Than Yesterday<br>


## :pushpin: Contact
- 이메일: hansoll1215@naver.com
- 깃헙: <br>
https://github.com/1SSoll2/HSKimPF ( Overall PortFolio )<br>
https://github.com/1SSoll2/scriptsForPRTG ( Custom Script Sensor )

</br>

## :pushpin: Projects
### 1. [포트폴리오](https://github.com/2023-SMHRD-KDT-IOT-4/Bello/tree/new_socket_version)

<br><br>
Bello : 5인 팀 프로젝트 <br><br>
역할 : <br><br>
서비스 요구사항을 기반으로 MySQL 데이터베이스와 테이블 관계를 설계하고,
데이터 정합성 유지를 위한 Trigger 및 제약조건을 구성했습니다. <br>
Spring WebSocket을 활용해 클라이언트와 서버 간 실시간 통신 기능을 구현하고,
애플리케이션 서버 배포 및 운영을 담당했습니다. <br><br>
개발 기간: 2024.01.04 ~ 2024.01.15<br><br>
 
>기술 스택:  
><b>Java 8</b> / <b>Spring 4</b> / <b>Maven</b> / <b>Web Socket</b> / Python / Flask / <b>JavaScript</b> / <b>MySQL</b> <br>
> HTML / CSS  <br>
>/ Raspberry-Pi (Flask, Picamera2, OpenCV, RPi.GPIO)/
><br>

### 2. [포트폴리오](https://github.com/2023-SMHRD-KDT-IOT-4/yeahaRepo)
<br><br><br>
YEAHA : 5인 팀 프로젝트 <br><br>
역할 : <br><br>
(DB) DB설계, 테이블 생성 및 관리, DB관련 문서 작성 테이블 생성 및 관리 <br>
식품안전나라 및 건강보험심사평가원 API를 통한 자료 수집 <br>
(M.L) 알고리즘별 모델링 점수 분석, 알고리즘 함수화 <br> 
(Back) Controller <br>
(Front) Back과 연동
<br>
<br><br>

개발 기간: 2024.02.26 ~ 2022.03.13<br><br>

## :office: Professional Projects

### 1. SAN Switch 전용 모니터링 웹 애플리케이션

> 회사 내부 프로젝트로 소스코드는 공개하지 않습니다.

**프로젝트 개요**

다양한 벤더의 SAN Switch 상태와 성능 정보를 통합 수집하고, 장애 및 성능 이상을 시각적으로 확인할 수 있는 전용 모니터링 웹 애플리케이션을 개발했습니다.

**담당 업무**

* Django 기반 백엔드 및 REST API 개발
* PostgreSQL 데이터베이스 설계 및 모니터링 데이터 관리
* Redis를 활용한 캐시 및 데이터 처리 구조 구성
* SAN Switch 장비 정보와 성능 지표 수집 로직 개발
* 장비 상태, 포트 사용량 및 장애 현황을 확인할 수 있는 대시보드 구현
* Docker 기반 애플리케이션 배포 및 운영 환경 구성

**기술 스택**

`Python` `Django` `PostgreSQL` `Redis` `Docker` `JavaScript` `HTML` `CSS`

---

### 2. PRTG 기반 통합 인프라 모니터링 구축

> 고객사 및 회사 내부 인프라를 대상으로 수행한 프로젝트입니다.

**프로젝트 개요**

서버, 네트워크 장비, 무선 컨트롤러, Access Point 및 기타 인프라 장비를 통합 모니터링하기 위해 PRTG 기반 NMS 환경을 구축하고 운영했습니다.

**담당 업무**

* 서버 및 네트워크 장비 자동 탐색과 모니터링 센서 구성
* Ping, SNMP, Traffic 기반 장비 가용성 및 성능 모니터링
* Aruba Controller 및 AP 상태 모니터링
* 장애 임계값, 알림 정책 및 사용자 권한 구성
* Active Directory 연동 및 사용자 그룹 구성
* 고객 요구사항에 따른 Custom Sensor 및 Lookup 개발
* 장애 발생 시 Windows Event Log 및 PRTG 로그 분석

**기술 스택**

`PRTG` `SNMP` `PowerShell` `Windows Server` `Active Directory` `Aruba Network` `TCP/IP`

---

### 3. Custom SNMP 프린터 모니터링 센서 개발

**프로젝트 개요**

PRTG 기본 프린터 센서에서 정상적으로 수집하지 못하는 장비의 상태 정보를 모니터링하기 위해 Printer-MIB 기반 Custom Sensor를 개발했습니다.

**담당 업무**

* RFC 3805 Printer-MIB 기반 OID 분석
* Net-SNMP를 활용한 프린터 상태 및 소모품 정보 수집
* PowerShell 기반 PRTG EXE/Script Advanced Sensor 개발
* 프린터 커버 상태, 누적 출력 페이지 및 소모품 상태 모니터링
* PRTG Value Lookup 파일을 통한 상태값 시각화
* SNMP 응답값 인코딩 및 장비별 MIB 차이 분석

**기술 스택**

`PRTG` `SNMP` `PowerShell` `Net-SNMP` `Printer-MIB` `XML`

---

### 4. Dify·Ollama 기반 사내 LLM 서비스 구축

**프로젝트 개요**

외부 LLM API 의존도와 운영 비용을 줄이기 위해 Dify와 Ollama를 활용한 사내 LLM 서비스 환경을 구축했습니다.

**담당 업무**

* Docker Compose 기반 Dify 서비스 배포
* Ollama 서버 구축 및 오픈소스 LLM 모델 연동
* PostgreSQL, Redis 및 Plugin Daemon 서비스 구성
* Dify Knowledge Base 및 문서 검색 파이프라인 구성
* Excel·CSV 기반 데이터를 활용한 근태 분석 워크플로 개발
* LLM 및 Code Node를 이용한 데이터 정규화와 집계 로직 개발
* 컨테이너 간 통신, 포트 및 플러그인 연결 장애 분석

**기술 스택**

`Dify` `Ollama` `LLM` `Docker Compose` `PostgreSQL` `Redis` `Python`

---

### 5. Kubernetes 기반 컨테이너 운영 환경 구축

**프로젝트 개요**

컨테이너 기반 서비스의 배포 및 운영 자동화를 위해 Kubernetes 단일 노드 클러스터를 구축하고 서비스 배포 환경을 구성했습니다.

**담당 업무**

* kubeadm 기반 Kubernetes 클러스터 구축
* containerd Container Runtime 구성
* Flannel CNI 설치 및 Pod 네트워크 구성
* CoreDNS 및 클러스터 내부 통신 장애 분석
* Docker 기반 서비스를 Kubernetes 환경으로 전환하기 위한 구조 검토
* Pod, Service 및 컨테이너 상태 점검과 장애 대응

**기술 스택**

`Kubernetes` `Docker` `containerd` `Flannel` `Linux` `Rocky Linux`

---

### 6. 고객사 전용 웹 애플리케이션 개발 및 배포 관리

> 고객사 내부망에서 운영되는 비공개 프로젝트입니다.

**프로젝트 개요**

Cloud 버전을 기반으로 고객사 요구사항에 맞는 Custom 버전을 개발하고, 고객사별 기능 및 데이터베이스 구조를 분리하여 관리했습니다.

**담당 업무**

* Cloud 및 고객사 Custom 버전 형상관리 전략 수립
* 고객사별 기능과 설정 분리
* 고객사별 데이터베이스 스키마 차이를 고려한 구조 설계
* GitLab 기반 브랜치 및 Repository 운영 방안 검토
* 내부망 배포 환경과 문서 버전 관리 체계 구성
* 고객사별 배포 및 유지보수 프로세스 개선

## :hammer_and_wrench: Tech Stack

### Backend

`Java 8` `Spring Framework` `Python` `Django` `Flask` `Node.js`

### Database & Cache

`PostgreSQL` `MySQL` `Oracle` `Redis`

### DevOps & Infrastructure

`Docker` `Docker Compose` `Kubernetes` `GitLab` `Git` `Linux` `VMware`

### Network & Monitoring

`PRTG` `SNMP` `Aruba Network` `TCP/IP` `Net-SNMP` `PowerShell`

### AI & Automation

`Dify` `Ollama` `LLM` `n8n`

### Frontend

`JavaScript` `HTML` `CSS`

### Embedded & IoT

`Raspberry Pi` `Arduino` `OpenCV` `Picamera2` `RPi.GPIO`

If you need English version, <a href="https://github.com/1SSoll2/HSKimPF/blob/main/EnglishVer.md">Click Here!</a>
