# AI-RedTeam-Lab

> **A personal Cyber Range for Cybersecurity, Embedded Security, Reverse Engineering, and AI-powered Red Team research.**

한국어 기반으로 네트워크·웹·시스템 보안부터 리버스 엔지니어링, 임베디드 보안, Blue Team, AI Agent 기반 보안 연구까지 단계적으로 학습하는 프로젝트입니다.

- **Learn:** 컴퓨터 시스템과 보안 원리 이해
- **Test:** 허가된 실습 환경에서 취약점 검증
- **Analyze:** 패킷·로그·펌웨어·바이너리 분석
- **Defend:** 탐지 규칙과 방어 대책 작성
- **Automate:** 안전한 범위에서 보안 분석 워크플로 자동화

> [!IMPORTANT]
> 모든 실습은 본인이 소유하거나 명시적으로 허가받은 시스템, 로컬 Cyber Range, CTF 및 교육용 환경에서만 수행합니다. 타인의 시스템에 대한 무단 스캔, 침투, 계정 탈취, 데이터 접근, 서비스 방해는 금지합니다. 자동화 도구와 AI Agent에는 명시적인 대상 범위, 실행 제한, 로그 기록 및 사람의 승인 절차를 적용합니다.

## 프로젝트 목표

```text
Hardware / FPGA
       ↓
Embedded Systems
       ↓
Linux / Networking
       ↓
Cybersecurity Foundations
       ↓
Web / System Security
       ↓
Reverse Engineering
       ↓
Red Team + Blue Team
       ↓
LLM / Agent Engineering
       ↓
AI-assisted Security Research
```

## 저장소 구조

```text
AI-RedTeam-Lab/
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── SECURITY.md
├── CODE_OF_CONDUCT.md
├── .gitignore
├── docs/
│   ├── roadmap.md
│   ├── cyber-range-setup.md
│   └── ethics-and-scope.md
├── 00-foundation/
├── 01-network-security/
├── 02-web-security/
├── 03-ctf/
├── 04-system-security/
├── 05-reverse-engineering/
├── 06-embedded-security/
├── 07-red-team/
├── 08-blue-team/
├── 09-ai-security/
├── 10-ai-redteam/
├── labs/
│   └── LAB-TEMPLATE.md
└── resources/
    └── learning-resources.md
```

## 학습 로드맵

| 단계 | 주제 | 핵심 결과물 |
|---|---|---|
| 00 | 기초 | Linux, TCP/IP, HTTP, 권한 모델 노트 |
| 01 | 네트워크 보안 | Wireshark 패킷 분석 보고서 |
| 02 | 웹 보안 | OWASP 학습 노트 및 안전한 재현 보고서 |
| 03 | CTF | 문제 풀이 기록과 근본 원인 분석 |
| 04 | 시스템 보안 | Linux/Windows 보안 설정 점검표 |
| 05 | 리버스 엔지니어링 | Ghidra 기반 교육용 바이너리 분석 |
| 06 | 임베디드 보안 | 본인 소유 보드의 UART/펌웨어 분석 |
| 07 | Red Team | 승인된 범위의 공격 표면 및 공격 경로 분석 |
| 08 | Blue Team | 로그 분석, Sigma/IDS 탐지 아이디어 |
| 09 | AI Security | LLM 안전성, 프롬프트 인젝션, 도구 권한 통제 |
| 10 | AI Red Team | 제한된 범위의 AI 보안 분석 워크플로 프로토타입 |

## 추천 학습 플랫폼

- [OverTheWire](https://overthewire.org/wargames/)
- [PortSwigger Web Security Academy](https://portswigger.net/web-security)
- [TryHackMe](https://tryhackme.com/)
- [Hack The Box](https://www.hackthebox.com/)
- [picoCTF](https://picoctf.org/)
- [OWASP Juice Shop](https://owasp.org/www-project-juice-shop/)
- [OWASP WebGoat](https://owasp.org/www-project-webgoat/)
- [MITRE ATT&CK](https://attack.mitre.org/)
- [Ghidra](https://ghidra-sre.org/)
- [Wireshark](https://www.wireshark.org/)

플랫폼과 도구의 라이선스, 이용약관, 각 실습의 허가 범위를 확인한 뒤 사용합니다.

## 시작하기

1. 저장소를 로컬 PC로 복제하거나 ZIP 파일을 풉니다.
2. `docs/roadmap.md`에서 현재 학습 단계를 선택합니다.
3. `docs/cyber-range-setup.md`의 격리 원칙에 따라 실습 환경을 구성합니다.
4. 각 실습은 `labs/LAB-TEMPLATE.md` 형식으로 기록합니다.
5. 가능하면 모든 실습에 방어 관점, 로그/증거, 개선 방안을 포함합니다.

## 6개월 권장 계획

- **1개월:** Linux 및 네트워크 기초
- **2개월:** HTTP 및 웹 보안
- **3개월:** CTF와 취약점 근본 원인 분석
- **4개월:** Linux/Windows 시스템 보안
- **5개월:** ARM, 펌웨어, 리버스 엔지니어링
- **6개월:** Blue Team, LLM Agent, AI 보안 실험

개인의 기존 경험과 학습 시간에 따라 기간을 조정합니다.

## 실습 기록 원칙

각 보고서는 다음 질문에 답하도록 작성합니다.

1. 무엇을 검증했는가?
2. 실습 대상과 허가 범위는 무엇인가?
3. 어떤 증거를 수집했는가?
4. 원인은 무엇인가?
5. 영향은 무엇인가?
6. 어떻게 탐지하고 방어할 수 있는가?
7. 재현을 제한하거나 안전하게 종료하는 방법은 무엇인가?

## License

이 저장소의 문서와 템플릿은 MIT License를 따릅니다. 외부 도구·자료·플랫폼에는 각자의 라이선스와 약관이 적용됩니다. 자세한 내용은 [`LICENSE`](LICENSE)를 확인하세요.
