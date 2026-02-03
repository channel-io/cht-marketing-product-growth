# 마케팅 팀 방향성: Conversational Marketing + Sales

> **상태**: 탐색 중
>
> **제안**: CRM 마케팅이 아닌 Conversational Marketing + Sales에 집중

---

## 1. 왜 이 방향인가?

### 시장 기회

글로벌 플레이어들이 같은 방향으로 수렴 중:

| 회사 | 움직임 |
|------|--------|
| **Drift** | Salesloft에 인수 (2024) - Revenue Orchestration으로 통합 |
| **Intercom** | Fin을 SDR로 확장, CRM 마케팅은 유지만 |
| **Zendesk** | Suite + Sell 통합, 마케팅 명시적으로 안 함 |

**시장 규모:** Conversational Commerce $14.9B → $63.4B (CAGR 15.6%)

> 상세: [Conversational 시장 리서치](../references/conversational-market-research.md)

### CRM 마케팅의 한계

| 구분 | CRM Marketing | Conversational |
|------|---------------|----------------|
| 타이밍 | 비동기 (캠페인 발송 후 대기) | 실시간 (의도 발생 순간 포착) |
| 위치 | 상담 밖 (데이터 추출 → 별도 채널) | 상담 안 (대화 = 전환) |
| 해자 연결 | ❌ | ⭕ |

CRM 마케팅은 상담 해자와 연결이 약함 → 채널톡이 경쟁 우위를 갖기 어려움

> 상세: [CRM 마케팅 검증](../context/market/crm-marketing-moat-research.md)

---

## 2. Conversational Marketing + Sales란?

### 개념

```
기존 CRM 마케팅:
고객 데이터 수집 → 세그먼트 → 이메일/푸시 캠페인 → (며칠 후) 반응 확인

Conversational:
방문자 → 실시간 대화 → 의도 파악 → 즉시 전환 (같은 세션)
```

- **Conversational Marketing**: 방문자 → 실시간 대화 → 리드 생성/육성
- **Conversational Sales**: 리드 자격검증 → 세일즈팀 핸드오프 → 계약 전환

### 핵심

> "CRM은 고객을 '아는 방법'이고, Conversational은 고객과 '돈을 버는 방법'이다"

- CRM: 인프라/백엔드 (고객 상태, 히스토리, 규칙)
- Conversational: 전면 제품 (실제 전환이 일어나는 곳)

---

## 3. 채널톡에 맞는 이유

### 이미 보유한 자산

| 자산 | 설명 |
|------|------|
| 실시간 대화 인프라 | 웹챗, 인앱 메시지 이미 구축 |
| 상담 자동화 경험 | ALF(AI 상담원) 기술 보유 |
| "지금 의도" 순간 점유 | 고객이 문제/관심이 생긴 순간 이미 채널톡에 있음 |

### 자연스러운 확장 경로

```
현재: CS 상담 (문제 해결)
  ↓
확장: Pre-sales 상담 (구매 전환)
  ↓
확장: Post-sales (Upsell, Expansion)
```

상담 해자 위에서 자연스럽게 확장 가능

### vs 경쟁

| vs | 채널톡 이점 |
|----|------------|
| CRM 마케팅 툴 | 대화 인프라 없음. 새로 구축해야 함 |
| 순수 Chatbot 툴 | 상담 깊이 없음. CS 경험 부족 |

---

## 4. 팀 역할

### 제안

| 구분 | 현재 | 제안 |
|------|------|------|
| 팀 이름 | Feat-Marketing | Feat-Marketing (유지) |
| 집중 영역 | CRM Marketing | Conversational Marketing + Sales |
| 방식 | 이메일, 푸시, 캠페인 | 실시간 대화 기반 전환 |

### CRM 마케팅의 역할

- ❌ 확장 대상 아님
- ⭕ 최소 유지 (기존 고객 지원)
- ⭕ Conversational의 백엔드로 활용 (고객 데이터, 히스토리)

---

## 5. 다음 단계

### 검증 필요 사항

- 채널톡 맥락에서 Pre-sales 상담 볼륨/가치
- 현재 Sales ALF PoC가 상담 해자를 활용하는 방향인지

### TODO

| 항목 | 설명 | 상태 |
|------|------|------|
| Sales ALF 해자 연결 검토 | 현재 PoC가 상담 해자를 활용하는지 vs 별개 기능인지 | 🔲 |
| 로드맵 구체화 | Conversational Marketing + Sales 방향의 제품 로드맵 | 🔲 |

---

## 변경 이력

| 날짜 | 변경 내용 |
|------|----------|
| 2026-02-02 | 초안 작성 |
| 2026-02-03 | 시장 리서치 분리, "피벗" → "방향 제안"으로 뉘앙스 변경 |
