# 오늘현황 (간호사용)

오늘 현황 화면에서 당일 진료 흐름 전체를 실시간으로 확인합니다.\
의사별 진료 현황을 한눈에 파악하고, 환자 카드 상태를 관리합니다.

***

## 화면 구성

<table><thead><tr><th width="153.90625">영역</th><th>내용</th></tr></thead><tbody><tr><td><strong>상단 집계</strong></td><td>총 예약 수 / 접수 완료 / 진료 중 / 진료 완료 현황</td></tr><tr><td><strong>의사별 현황</strong></td><td>교수님(의사)별 진료 현황 탭 분리 표시</td></tr><tr><td><strong>환자 카드</strong></td><td>각 환자의 접수·문진·진료 상태 카드 형태로 표시</td></tr><tr><td><strong>완료 탭</strong></td><td>진료 완료 환자 목록 및 템플릿 발송 버튼</td></tr></tbody></table>

***

## 환자 카드 상태

<table><thead><tr><th width="137.41015625">상태</th><th>의미</th><th>조치</th></tr></thead><tbody><tr><td><strong>문진 생략</strong></td><td>환자가 문진을 작성하지 않은 상태</td><td>QR 재발송 또는 대신 입력</td></tr><tr><td><strong>문진 중</strong></td><td>환자가 문진 작성 진행 중</td><td>대기</td></tr><tr><td><strong>문진 완료</strong></td><td>AI 분석 완료, 진료 준비 완료</td><td>진료실 안내</td></tr><tr><td><strong>진료 중</strong></td><td>의사가 진료 화면에서 해당 환자 선택 중</td><td>—</td></tr><tr><td><strong>진료 보류</strong></td><td>검사·시술로 진료 잠시 중단</td><td>보류 탭에서 확인</td></tr><tr><td><strong>진료 완료</strong></td><td>진료 저장 완료</td><td>템플릿 발송 가능</td></tr></tbody></table>

***

## 주요 기능

### 접수 취소

환자 카드의 **X 버튼** 클릭 → 접수 취소 확인 창 → 확인

### 템플릿 발송

완료 탭의 환자 카드에서 **"템플릿 발송"** 버튼 클릭\
→ 템플릿 선택 후 발송\
→ 발송 완료된 카드에는 발송 버튼이 표시되지 않음

{% hint style="info" %}
진료 당일 템플릿을 발송하지 못한 경우, 과거 날짜의 환자도 **환자 목록**에서 이후에 발송할 수 있습니다.
{% endhint %}

### QR 재발송

환자 카드 옆 **··· 메뉴 → "QR 재발송"** 선택\
→ 등록된 연락처로 카카오톡 또는 SMS 재발송
