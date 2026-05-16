# 진료화면 (의사용)

의사용 진료 화면은 AI 문진 요약 확인, 녹음 STT, AI 추천 의증, 차팅 기록까지 진료 전 과정을 하나의 화면에서 처리합니다.

***

## 진료 흐름

```
환자 카드 선택 (진료 전)
    ↓
AI 문진 요약 확인 (C.C. / Onset / PHx / P.I.)
    ↓
진료 녹음 시작 (●)
    ↓
AI 추천 의증 확인 및 선택
    ↓
진료 저장 → 템플릿 발송
```

***

## 진료 상태 구분

<table><thead><tr><th width="169.64453125">상태</th><th>설명</th></tr></thead><tbody><tr><td><strong>진료 전</strong></td><td>환자 카드 선택 시 → 진료 중으로 전환</td></tr><tr><td><strong>진료 중</strong></td><td>문진 요약, 녹음, AI 의증 활용</td></tr><tr><td><strong>진료 보류</strong></td><td>검사·시술이 있는 경우 보류 상태로 변경, 보류 탭으로 이동</td></tr><tr><td><strong>진료 완료</strong></td><td>진료 저장 클릭 또는 다른 환자 카드 선택 시 완료 처리</td></tr></tbody></table>

***

## 화면 모드

V.Doc Pro는 진료 환경에 맞게 두 가지 모드를 제공합니다.

<table><thead><tr><th width="172.375">모드</th><th>특징</th><th>적합한 환경</th></tr></thead><tbody><tr><td><a href="/broken/pages/cGHcshlx4gDbyWD2Zq7F"><strong>전체 모드</strong></a></td><td>모든 기능을 하나의 넓은 화면에서 사용</td><td>전용 모니터가 있는 진료실</td></tr><tr><td><a href="/broken/pages/rCQs9UPtdaufFlHXPaJZ"><strong>미니 모드</strong></a></td><td>작은 창으로 EMR과 나란히 사용</td><td>EMR 화면과 함께 사용할 때</td></tr></tbody></table>

진료 화면 우측 상단의 **"미니 모드"** 버튼으로 언제든지 전환할 수 있습니다.
