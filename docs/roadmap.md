# 학습 로드맵

## 원칙

- 개념을 이해한 뒤 도구를 사용한다.
- 허가된 범위 안에서만 실습한다.
- 공격 기법은 방어·탐지·완화와 함께 학습한다.
- CTF write-up에는 정답뿐 아니라 근본 원인과 예방 방법을 기록한다.
- AI Agent는 기본적으로 읽기 전용으로 시작하고, 실행 도구는 allowlist와 사람의 승인을 적용한다.

## 단계별 목표

### 00 — Foundation
- TCP/IP, DNS, HTTP/HTTPS
- Linux 프로세스, 권한, 서비스, 소켓
- Git, Python, 로그 읽기

**완료 기준:** 로컬 서비스의 네트워크 흐름을 설명하고 기초 로그를 분석할 수 있다.

### 01 — Network Security
- Wireshark, tcpdump, DNS, TCP handshake
- 로컬 실습 트래픽 캡처 및 필터링
- 서비스 인벤토리와 네트워크 분리

**완료 기준:** 캡처 파일과 설명이 포함된 패킷 분석 보고서 3개.

### 02 — Web Security
- HTTP 요청/응답, 쿠키, 세션
- 인증과 권한 확인의 차이
- OWASP Top 10 개념
- PortSwigger Academy 및 로컬 OWASP Juice Shop

**완료 기준:** 교육용 실습 5개에 대해 원인, 영향, 수정 방안을 문서화한다.

### 03 — CTF
- OverTheWire, picoCTF, TryHackMe 등
- 문제 해결 과정과 근본 원인 기록
- 공개된 풀이를 그대로 복사하지 않고 직접 분석

**완료 기준:** 초급 문제 5개 이상에 대한 자체 write-up.

### 04 — System Security
- Linux 권한과 서비스 설정
- Windows 보안 기초
- 로그, 패치, 최소 권한, 백업
- Active Directory는 전용 실습 환경에서만 학습

**완료 기준:** 로컬 VM의 보안 점검표 및 개선 전후 기록.

### 05 — Reverse Engineering
- C/Assembly 기초, ELF/PE
- GDB, objdump, strings
- Ghidra를 이용한 교육용 바이너리 분석

**완료 기준:** 출처와 사용 권한이 분명한 샘플 바이너리의 분석 보고서.

### 06 — Embedded / IoT Security
- UART, SPI, I2C, JTAG/SWD 개념
- 부트 과정, 펌웨어 구조, Secure Boot
- 본인 소유의 개발 보드와 장비를 사용

**완료 기준:** 장비 설명, 테스트 범위, 수집 증거, 방어 권고를 포함한 보고서.

### 07 — Red Team
- 자산 인벤토리와 공격 표면
- MITRE ATT&CK의 전술/기술
- 테스트 계획, 범위, 증거 보존, 보고서 작성

**완료 기준:** 로컬 실습 범위에 대한 위험 기반 테스트 계획서.

### 08 — Blue Team
- 시스템/네트워크 로그 분석
- Wazuh, Suricata, Zeek 개념
- Sigma 규칙의 구조와 테스트
- 경보 튜닝과 오탐 관리

**완료 기준:** 교육용 로그에서 탐지 시나리오와 대응 절차를 작성한다.

### 09 — AI Security
- LLM API, 구조화된 출력, tool calling
- 프롬프트 인젝션과 데이터 유출 위험
- 최소 권한, 입력 검증, 감사 로그
- Human-in-the-loop와 실패 안전 설계

**완료 기준:** 도구 실행 없이 입력을 분류하고 안전 정책 위반을 기록하는 분석 프로토타입.

### 10 — AI Red Team
- 제한된 테스트 대상 목록
- 읽기 전용 정찰/분석 단계부터 시작
- 도구 호출 전 정책 검사
- 실행 제한, timeout, 결과 검증
- 증거와 보고서의 출처 추적

**완료 기준:** 격리된 교육용 환경에서만 동작하는 프로토타입과 안전성 테스트 문서.

## 권장 일정

| 월 | 집중 분야 | 산출물 |
|---|---|---|
| 1 | Linux / Network | 네트워크 노트와 패킷 분석 |
| 2 | Web Security | 웹 보안 학습 보고서 |
| 3 | CTF | 풀이 기록 |
| 4 | System Security | 하드닝 점검표 |
| 5 | Reverse Engineering / Embedded | 교육용 펌웨어 분석 |
| 6 | Blue Team / AI Security | 탐지 시나리오와 제한된 Agent 설계 |
