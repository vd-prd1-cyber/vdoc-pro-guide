# 브이닥 프로 사용가이드 - 작업 컨텍스트

> ⚠️ 이 파일은 Claude(AI)가 작업을 시작할 때 가장 먼저 읽는 파일입니다.
> > 새 대화를 시작할 때 반드시 이 파일을 먼저 읽어주세요.
> >
> > ---
> >
> > ## 📌 프로젝트 기본 정보
> >
> > | 항목 | 값 |
> > |------|-----|
> > | GitHub repo | `vd-prd1-cyber/vdoc-pro-guide` |
> > | GitBook Space ID | `AXFB4ou1UZ5tt15hyBwF` |
> > | GitBook Organization ID | `dY5gPwOK683T5cmr4Zjt` |
> > | GitBook Editor URL | `https://app.gitbook.com/o/dY5gPwOK683T5cmr4Zjt/s/AXFB4ou1UZ5tt15hyBwF/` |
> > | 기본 브랜치 | `main` |
> > | 백업 브랜치 | `backup-20260520` (2026년 5월 20일 기준 백업) |
> >
> > ---
> >
> > ## 📁 폴더 구조 매핑
> >
> > | 폴더명 | 실제 섹션 | 주요 파일 |
> > |--------|-----------|-----------|
> > | `undefined-1` | 브이닥 프로 소개 | `vdoc-pro.md`, `workflow.md` |
> > | `undefined-2` | 시작하기 | `index/README.md`, `cloud.md`, `signup/`, `login.md` |
> > | `undefined-3` | 준비하기 | `menu/`, `notification.md` |
> > | `undefined-4` | 진료하기 | `pre-consult.md`, `during-ocr.md`, `during-recording.md`, `after-template.md` |
> > | `undefined-5` | 오늘 현황 | `today.md` |
> > | `undefined-6` | 환자 관리 | `patients.md` |
> > | `undefined-7` | 환자 목록 | `patient-list.md` |
> > | `undefined-8` | 환자 사전 문진 안내 | `index.md`, `qr-checkin.md` |
> > | `undefined-9` | 템플릿 설정 | `template-management.md` |
> > | `undefined-11` | 대시보드 | `undefined.md` |
> > | `undefined-12` | 관리자 설정 | `account.md`, `audit.md` |
> > | `undefined-13` | 도움말 | `faq.md`, `contact.md` |
> >
> > > ⚠️ 폴더명이 `undefined-N` 형태인 것은 GitBook 초기 export 시 자동 생성된 것입니다.
> > > > 기능상 문제없으므로 현재 그대로 유지 중입니다.
> > > >
> > > > ---
> > > >
> > > > ## 🖼️ 이미지 관리
> > > >
> > > > - 모든 이미지는 `.gitbook/assets/` 폴더에 저장
> > > > - - md 파일에서 이미지 경로: `![](<../.gitbook/assets/파일명.png>)`
> > > >   - - 이미지 교체 시: 같은 파일명으로 `.gitbook/assets/`에 업로드하면 자동 반영
> > > >     - - GitHub에 이미지 업로드 → GitBook 자동 sync (별도 작업 불필요)
> > > >      
> > > >       - ---
> > > >
> > > > ## ⚙️ GitBook ↔ GitHub 연동 규칙 (충돌 방지)
> > > >
> > > > ### 절대 하지 말 것
> > > > - ❌ GitBook 에디터에서 **Edit 버튼** 클릭 금지
> > > > - - ❌ GitBook에서 Change Request 생성 금지
> > > >   - - ❌ GitHub와 GitBook 양쪽에서 동시 편집 금지
> > > >    
> > > >     - ### 반드시 지킬 것
> > > >     - - ✅ **모든 작업은 GitHub에서만** 진행
> > > >       - - ✅ GitHub commit → GitBook 자동 반영 (sync 정상 상태)
> > > >         - - ✅ GitBook은 **결과 확인 용도로만** 사용
> > > >          
> > > >           - ### GitHub Sync 상태 확인
> > > >           - - GitBook 에디터 상단 GitHub 아이콘 옆 ✅ 초록색 체크 = 정상
> > > >             - - 문제 발생 시: GitBook → GitHub 아이콘 클릭 → Sync 상태 확인
> > > >              
> > > >               - ---
> > > >
> > > > ## 📝 작업 유형별 처리 방법
> > > >
> > > > ### 이미지 교체
> > > > 1. GitHub `.gitbook/assets/` 폴더에 새 파일 업로드 (같은 파일명)
> > > > 2. 2. 자동 반영 완료
> > > >   
> > > >    3. ### 페이지 내용 수정/삭제
> > > >    4. 1. 위 폴더 매핑에서 해당 `.md` 파일 경로 확인
> > > >       2. 2. GitHub에서 파일 직접 편집 후 commit
> > > >         
> > > >          3. ### 새 페이지 추가
> > > >          4. 1. 해당 폴더에 새 `.md` 파일 생성
> > > >             2. 2. `SUMMARY.md`에 경로 추가
> > > >                3. 3. commit
> > > >                  
> > > >                   4. ---
> > > >                  
> > > >                   5. ## 🤖 Claude에게 작업 요청하는 방법
> > > >                  
> > > >                   6. ### 새 대화 시작 시 첫 메시지 형식
> > > > ```
> > > > vd-prd1-cyber/vdoc-pro-guide README 읽고 [할 작업 내용] 해줘
> > > > ```
> > > >
> > > > ### 요청 예시
> > > > - `"README 읽고 진료 흐름 한눈에 보기 페이지 이미지 교체해줘"`
> > > > - - `"README 읽고 템플릿 활성화 페이지에 내용 추가해줘"`
> > > >   - - `"README 읽고 새 페이지 만들어줘"`
> > > >    
> > > >     - ### Claude가 작업 시작 전 확인할 것
> > > >     - 1. 이 README.md 읽기
> > > >       2. 2. 폴더 매핑 확인
> > > >          3. 3. GitHub Sync 상태 정상 여부 확인
> > > >             4. 4. GitBook에 열려있는 Change Request 없는지 확인
> > > >               
> > > >                5. ---
> > > >               
> > > >                6. ## 🔄 롤백 방법
> > > >               
> > > >                7. 문제 발생 시 `backup-20260520` 브랜치로 복구:
> > > > 1. GitHub repo → branches 탭
> > > > 2. 2. `backup-20260520` 브랜치 선택
> > > >    3. 3. main 브랜치에 PR 생성 후 merge
> > > >      
> > > >       4. ---
> > > >      
> > > >       5. ## 📅 작업 이력
> > > >      
> > > >       6. | 날짜 | 작업 내용 |
> > > > |------|-----------|
> > > > | 2026-05-20 | 이미지 교체 (screen-flow-*, screen-template-*) |
> > > > | 2026-05-20 | 템플릿 수정/생성 관련 내용 삭제 (after-template.md, template-management.md) |
> > > > | 2026-05-20 | backup-20260520 브랜치 생성 |
