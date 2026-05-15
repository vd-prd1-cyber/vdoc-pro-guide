# 브이닥 프로 설치하기

V.Doc Pro는 병원 환경에 따라 **Cloud** 방식과 **On-premise** 방식 두 가지로 설치할 수 있습니다.\
설치 방식은 도입 상담 시 AITRICS 담당자와 함께 결정합니다.

***

## 방식 비교

| 구분         | Cloud                       | On-premise         |
| ---------- | --------------------------- | ------------------ |
| **설치 위치**  | AITRICS 클라우드 서버 (AWS 서울 리전) | 병원 내부 서버           |
| **초기 설정**  | 간단 (계약 후 1주 이내)             | 별도 서버 구축 필요 (2–4주) |
| **EMR 연동** | API 방식 또는 수동 방식             | 내부 네트워크 기반         |
| **유지보수**   | AITRICS 자동 관리               | 병원 IT 담당자 협조       |
| **업데이트**   | 자동                          | 일정 조율 후 배포         |
| **적합 환경**  | 일반 의원·중소병원                  | 폐쇄망·보안 강화 환경       |

***

## 도입까지의 전체 흐름

```
도입 문의 → 상담 및 계약 → 설치 방식 결정 → 설치 및 EMR 연동 → 교육 → 운영 시작
```

<table><thead><tr><th width="206.83203125">단계</th><th>내용</th><th>소요 기간</th></tr></thead><tbody><tr><td><strong>STEP 1. 도입 문의 및 상담</strong></td><td>신청서 작성 → 담당자 검토 후 연락</td><td>1–2 영업일</td></tr><tr><td><strong>STEP 2. 계약</strong></td><td>라이선스 계약 체결</td><td>협의</td></tr><tr><td><strong>STEP 3. 커스텀 문진 설정</strong></td><td>병원 진료과별 맞춤 문진 콘텐츠 설계</td><td>1주</td></tr><tr><td><strong>STEP 4. 시스템 연동</strong></td><td>EMR 연동 및 테스트 실행</td><td>1–3주</td></tr><tr><td><strong>STEP 5. 교육 실시</strong></td><td>역할별 사용법 교육 후 정식 운영</td><td>방문 교육 1일</td></tr></tbody></table>

{% hint style="info" %}
EMR 연동이 필요 없는 스탠드얼론(독립 운영) 방식은 **1주 이내** 설치가 가능합니다.
{% endhint %}

***

## 시스템 공통 요구사항

<table><thead><tr><th width="156.98046875">항목</th><th>요구사항</th></tr></thead><tbody><tr><td><strong>브라우저</strong></td><td>Chrome 최신 버전 (필수)</td></tr><tr><td><strong>화면 해상도</strong></td><td>1280 × 800 이상 권장</td></tr><tr><td><strong>마이크</strong></td><td>STT 기능 사용 시 외장 USB 마이크 권장</td></tr><tr><td><strong>운영체제</strong></td><td>Windows 10 이상 / macOS</td></tr><tr><td><strong>네트워크</strong></td><td>안정적인 인터넷 연결 (Cloud) / 내부망 (On-premise)</td></tr></tbody></table>

{% hint style="warning" %}
V.Doc Pro 콘솔은 **Chrome 브라우저에 최적화**되어 있습니다. 다른 브라우저 사용 시 일부 기능이 정상 작동하지 않을 수 있습니다.
{% endhint %}

***

설치 방식별 자세한 안내는 아래를 참고하세요.

→ [Cloud 설치](cloud.md) | [On-premise 설치](on-premise.md)
