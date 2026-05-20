# 브이닥 프로 사용가이드 - Claude 작업 컨텍스트

> ⚠️ 이 파일은 Claude(AI)가 작업을 시작할 때 가장 먼저 읽는 파일입니다.
> 새 대화를 시작할 때 반드시 이 파일을 먼저 읽어주세요.

---

## 📌 프로젝트 기본 정보

| 항목 | 값 |
|--------|------|
| GitHub repo | `vd-prd1-cyber/vdoc-pro-guide` |
| GitBook Space ID | `AXFB4ou1UZ5tt15hyBwF` |
| GitBook Organization ID | `dY5gPwOK683T5cmr4Zjt` |
| GitBook Editor URL | `https://app.gitbook.com/o/dY5gPwOK683T5cmr4Zjt/s/AXFB4ou1UZ5tt15hyBwF/` |
| 기본 브랜치 | `main` |
| 백업 브랜치 | `backup-20260520` (2026년 5월 20일 기준 백업) |

---

## 📁 폴더 구조 매핑

| 폴더명 | 실제 섹션 | 주요 파일 |
|--------|----------|----------|
| `undefined-1` | 브이닥 프로 소개 | `vdoc-pro.md`, `workflow.md` |
| `undefined-2` | 시작하기 | `index/README.md`, `cloud.md`, `signup/`, `login.md` |
| `undefined-3` | 준비하기 | `menu/`, `notification.md` |
| `undefined-4` | 진료하기 | `pre-consult.md`, `during-ocr.md`, `during-recording.md`, `after-template.md` |
| `undefined-5` | 오늘 현황 | `today.md` |
| `undefined-6` | 환자 관리 | `patients.md` |
| `undefined-7` | 환자 목록 | `patient-list.md` |
| `undefined-8` | 환자 사전 문진 안내 | `index.md`, `qr-checkin.md` |
| `undefined-9` | 템플릿 설정 | `template-management.md` |
| `undefined-11` | 대시보드 | `undefined.md` |
| `undefined-12` | 관리자 설정 | `account.md`, `audit.md` |
| `undefined-13` | 도움말 | `faq.md`, `contact.md` |

> ⚠️ 폴더명이 `undefined-N` 형태인 것은 GitBook 초기 export 시 자동 생성된 것입니다.
> 기능상 문제없으므로 현재 그대로 유지 중입니다.

---

## 🖼️ 이미지 관리

- 모든 이미지는 `.gitbook/assets/` 폴더에 저장
- `.md` 파일에서 이미지 경로: `![](<../.gitbook/assets/파일명.png>)`
- 이미지 교체 시: 같은 파일명으로 `.gitbook/assets/`에 업로드하면 자동 반영
- GitHub에 이미지 업로드 → GitBook 자동 sync (별도 작업 불필요)

---

## ⚙️ 작업 원칙 (매우 중요)

### 반드시 지켜야 할 규칙

1. **모든 편집은 GitHub에서만** - GitBook 에디터 직접 편집 금지
2. **GitBook Change Request 생성 금지** - GitHub commit만 사용
3. **다른 목차/이미지 건드리지 않기** - 요청된 파일만 수정
4. **반복 실패 시 즉시 멈추고 사용자에게 질문**
5. **삭제 작업 전 반드시 범위 보고 후 승인 대기**

### GitHub 편집 워크플로우

1. SUMMARY.md에서 파일 경로 확인
2. GitHub 편집기에서 파일 열기 (`/edit/main/경로`)
3. 전체 선택(Cmd+A) → 수정된 내용 붙여넣기
4. Commit changes → commit 메시지 입력 → main 브랜치에 직접 commit
5. GitBook 자동 sync 확인 (보통 1-2분 내)

---

## ✅ 완료된 작업 이력 (2026-05-20)

| 파일 | 작업 내용 | Commit |
|------|----------|--------|
| `.gitbook/assets/` | 이미지 6개 업로드 (screen-flow-*.png, screen-template*.png) | - |
| `undefined-4/after-template.md` | `## 템플릿 내용 수정` 섹션 삭제 | dfbe339 |
| `undefined-9/template-management.md` | `생성하기` 행 + `## 템플릿 생성하기` + `## 템플릿 관리(더보기 메뉴)` 삭제 | 1dd527b |
| `README.md` | 원본 홈페이지 내용으로 복구 (Claude 컨텍스트로 덮어쓴 것 복구) | b18eec0 |
| GitBook Draft #51 | Archive 처리 | - |
| `backup-20260520` 브랜치 | 생성 완료 | - |

---

## 🔗 주요 URL

| 용도 | URL |
|------|-----|
| GitBook 에디터 | `https://app.gitbook.com/o/dY5gPwOK683T5cmr4Zjt/s/AXFB4ou1UZ5tt15hyBwF/` |
| GitBook 공개 사이트 | `https://v-doc-pro-guide.gitbook.io/vd-prd-docs/` |
| GitHub 저장소 | `https://github.com/vd-prd1-cyber/vdoc-pro-guide` |

---

## 💬 Claude에게 작업 요청하는 방법

새 대화를 시작할 때:
> "vd-prd1-cyber/vdoc-pro-guide 의 CLAUDE-CONTEXT.md 파일을 읽고 [작업 내용]을 진행해줘"
