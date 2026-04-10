# Soojong Kim

**Cloud Solutions Architect | Infrastructure Lead at TBIT**

TBIT 클라우드 사업부 구축팀의 기술 책임을 맡고 있습니다. KT Cloud, NCP, AWS, NHN Cloud 환경에서 인프라 아키텍처 설계와 기술 검수를 수행하며, 모니터링 체계 구축 및 운영 프로세스 표준화를 담당합니다.

---

## Technical Stack

* **Cloud**: KT Cloud, Naver Cloud Platform, AWS, NHN Cloud
* **Container**: Kubernetes, Docker, Container Migration
* **Monitoring**: LGTM Stack (Loki, Grafana, Tempo, Mimir), Prometheus, VictoriaMetrics
* **Security & Network**: WAF Policy, IPsec VPN, Ingress/LB, Firewall Strategy
* **Automation**: Python / PowerShell / FastAPI 기반 운영 자동화 및 내부 플랫폼 개발

---

## 2026 Q1 — Key Achievements

### 인프라 구축 및 마이그레이션

* **마이그레이션 주도**: 공공기관 대상 레거시 환경 클라우드 마이그레이션 설계 및 구축, 아키텍처 문서화 작성
* **솔루션 연동 협의**: DB접근제어·DB암호화, ERP, 3rd Party 솔루션 연동 등 기술 협의 및 CSP 제약 분석
* **멀티 CSP 구축 병행**: KT Cloud, NCP, NHN G-Cloud 환경 신규 구축 사업 다수 주담당 대응 (공공·민간)

### 견적 및 영업 지원

* **멀티 CSP 기술 제안 20+**: 공공·민간 고객사 요구사항을 분석하여 CSP 환경별 최적 구성 설계 및 견적 산출. 단순 견적 작성을 넘어 아키텍처 구성도와 과업 범위 정의까지 함께 제공
* **CSP 전환 의사결정 지원**: 기존 레거시 또는 타 CSP 환경 대비 비용·성능·보안 요건을 종합 비교 분석한 기술 제안서 작성. 고객사가 직접 판단할 수 있는 근거 자료 제공으로 계약 전환 주도
* **장기 계약 구조 설계**: 7년 선납 방식 등 비정형 계약 구조에 대한 기술·비용 타당성 검토 및 협의 주도

### 자동화 시스템 개발 (4종 진행)

* **구축완료 문서 자동화**: CSP API 기반 구축완료보고서 자동 생성 시스템 1차 완료 (KT·NCP·NHN 공공 지원)
* **Grafana Alloy 모니터링 파이프라인**: 에이전트 기반 모니터링 체계 구성 및 팀 인수인계
* **견적서 초안 자동화**: 견적 조건 입력 → 초안 자동 생성 시스템 개발 중
* **매니지드 리포트 자동화**: Grafana 대시보드 기반 월간 고객사 리포트 자동 생성 체계 구축 중

### 팀 기여

* **트렐로 기반 팀 업무관리 체계 운영**: Q1 총 40건 처리 (주담당 33건), 워크플로우 투명성 확보
* **산출물 검수**: 구축·견적 이중검토(Double-Check) 체계 운영
* **사내 클라우드 기술 스터디 리딩**: 주 1회 정기 진행 및 신규 팀원 온보딩 지원

---

## Personal Projects

- MSP 업무는 구축·견적·매니지드·문서화 등 과업 전반에 걸쳐 반복적인 작업이 많고, 담당자별·팀별로 흩어져 관리되는 구조적 비효율이 존재. 
- 이를 해결하기 위해 **MSP 과업 전 과정의 자동화**를 목표로 일련의 내부 플랫폼을 직접 설계하고 개발. 
- 견적 작성부터 인프라 리소스 수집, 구축완료 문서 생성, 고객사별 모니터링 리포트까지 팀 내 흩어져 있던 자료와 프로세스를 단일 체계로 통합하고, 관리·시각화·시스템화하는 것이 핵심 방향.

### MSP Central Monitoring System `2026`
클라우드 MSP를 위한 다중 고객 서버 통합 모니터링 시스템. Ubuntu 중앙 서버 1대에서 모든 고객사 서버의 OS 메트릭(CPU/메모리/디스크/네트워크)을 수집·시각화하고 임계값 초과 시 이메일 알림을 발송한다.

* **Stack**: Grafana Alloy · VictoriaMetrics · VMAlert · Alertmanager · Grafana · Nginx · Docker Compose
* **특징**: Direct / Relay-Server / Relay-Agent 3가지 에이전트 모드로 폐쇄망 포함 전 환경 대응, Linux·Windows 공통 대시보드

### Cloud Resource Collector `2026`
MSP 환경에서 고객사별 클라우드 리소스를 API로 자동 수집하여 엑셀 및 구축완료보고서(PPT/Word)를 자동 생성하는 도구.

* **Stack**: Python · KT Cloud API · NCP API · NHN Cloud API · openpyxl · python-pptx
* **지원 CSP**: KT Cloud (공공/민간) · NCP (공공/민간) · NHN Cloud (공공) · AWS (예정)

### TBIT 클라우드 견적서 관리 시스템 `2026`
AWS · KT · NCP · NHN Cloud 서비스 카탈로그 기반 견적서 작성·관리·Excel 출력 플랫폼. AI 자연어 파싱으로 요구사항 텍스트를 견적 항목으로 자동 변환.

* **Stack**: FastAPI · Jinja2 · Alpine.js · SQLite · openpyxl · Docker Compose
* **기능**: 대시보드 · 견적서 CRUD · 카탈로그 연동 · Excel 가져오기/내보내기 · AI 파싱 · 관리자

### MSA 에러 처리 패턴 구현
gRPC 환경에서의 장애 전파 방지 패턴 구현

---

## Work Archive

<details>
<summary><strong>2025 — Key Achievements & Operations (펼치기)</strong></summary>

### Key Achievements

* **기술 검수 및 승인**: 연간 50건 이상의 인프라 설계서 및 산출물 최종 기술 검토 수행
* **기술 교육 실적**: 대학 및 공공 교육기관 대상 연간 200시간 이상의 클라우드 기술 교육 진행
* **운영 안정성**: 담당 고객사 인프라 가용성 99.9% 유지 및 기술 지원 120건 이상 완료

### 인프라 구축 및 설계

* **멀티 클라우드 아키텍처 설계**: 공공 및 민간 서비스 대상 KT Cloud Managed KS 중심의 멀티 CSP 인프라 설계 및 구축 주도. CSP별 네트워크 구조·보안 정책·가용성 요건을 반영한 아키텍처 산출물 작성
* **레거시 컨테이너 전환**: 기존 VM 기반 워크로드를 Kubernetes 환경으로 마이그레이션. 서비스 중단 없는 전환 계획 수립 및 컷오버 주도
* **AI 인프라 도입 지원**: 의료·교육기관 AI 서비스 도입을 위한 인프라 구성 검토, API 연동 설계 및 데이터 파이프라인 기술 지원

### 모니터링 및 운영

* **통합 모니터링 체계 구축**: Prometheus + Grafana 기반 다중 고객사 모니터링 대시보드 설계 및 로그 수집 파이프라인 구성. 임계값 알림 체계 수립으로 장애 선제 대응 기반 마련
* **운영 비용 최적화**: 담당 고객사 리소스 전수 조사 및 구조 재설계를 통해 운영 비용 30% 절감 달성
* **보안 운영**: 공공 클라우드 환경 WAF 정책 고도화, 보안 취약점 정기 점검 및 대응 프로세스 체계화

### 품질 관리 및 교육

* **산출물 품질 관리**: 구축팀 전체 산출물 표준화 기준 수립 및 최종 기술 승인(Approval) 프로세스 책임 운영. 연간 50건 이상 검수 수행
* **클라우드 기술 교육**: 대학 및 공공 교육기관 대상 AWS·NCP 실무 교육, SW마이스터고 클라우드 직무 역량 강화 멘토링 등 연간 200시간 이상 진행
* **사내 기술 공유**: 팀 내 정기 기술 세미나 리딩 및 온보딩 가이드 작성

</details>

<details>
<summary><strong>2024 — Infrastructure & Operations (펼치기)</strong></summary>

### 공공 클라우드 관제 및 안정성

* **10개 이상 공공기관 인프라 관제**: 에이전트 기반 실시간 관제 체계 운영, 연간 가용성 99.9% 및 보안 사고 Zero 달성
* **SLA 기반 운영 관리**: 고객사별 SLA 기준 수립 및 이행, 장애 발생 시 에스컬레이션 프로세스 운영
* **중앙 집중형 로그 수집 환경 구축**: 다수 고객사 로그를 단일 체계로 수집·보관하는 기반 마련

### 인프라 설계 및 최적화

* **가용성 중심 아키텍처 설계**: L4/L7 로드밸런서 기반 트래픽 분산, AZ 이중화, CDN 캐싱·라우팅 설계로 서비스 가용성 확보
* **운영 비용 절감**: 리소스 전수 조사 및 구조 개선을 통한 운영 비용 절감 달성
* **API 응답 최적화**: 주요 서비스 API 전송량 효율화 분석 및 지연 시간 개선 제안

### 보안 및 컴플라이언스

* **공공기관 보안 요건 대응**: 공공 클라우드 보안 가이드라인 기반 시스템 강화(Hardening) 수행 및 보안 당국 제출용 기술 분석 보고서 작성
* **AI 플랫폼 도입 보안 검토**: 신규 AI 플랫폼 도입에 따른 기존 인프라 보안 충돌 분석 및 위험 요소 식별

### 팀 역량 강화

* **사내 기술 공유 세미나 리딩**: 클라우드 운영 실무 중심의 정기 세미나 운영
* **온보딩 가이드 작성**: 신규 팀원 적응을 위한 업무 환경·프로세스 문서화

</details>

---

### Contact

* **Organization**: TBIT (으뜸정보기술)
* **Blog**: [cloudrepo.kro.kr](https://cloudrepo.kro.kr/)
* **Role**: Infrastructure Build Team Lead
