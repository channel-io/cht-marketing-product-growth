# Bloomreach Clarity 분석

> **목적**: B2C Conversational Sales 엔터프라이즈 플레이어 분석
> **조사일**: 2026-02-04

---

## 회사 개요

| 항목 | 내용 |
|------|------|
| 회사명 | Bloomreach |
| 설립 | 2009년 |
| 본사 | Mountain View, California |
| 창업자 | Arje Cahn, Ashutosh Garg, Raj De Datta |
| 직원 수 | ~1,100명 |
| 고객 수 | **1,400+ 브랜드** (40+ 국가) |

### 펀딩 & 밸류에이션

| 항목 | 내용 |
|------|------|
| 총 펀딩 | **$422M~$927M** |
| 최근 라운드 | $175M (2024년 11월) |
| 밸류에이션 | **$2.2B** (2024) |
| 주요 투자자 | Goldman Sachs, Bain Capital, Sixth Street |
| 단계 | Series F |

### 매출 & 성장률

| 시점 | ARR/매출 | YoY 성장률 |
|------|---------|-----------|
| 2021 | $100M ARR | - |
| 2022 | $150M ARR | **50%** |
| 2024 | $219.5M | ~20-25%/년 |

→ 2024년 Inc. 5000 (미국 가장 빠르게 성장하는 비상장 기업) 선정

> **출처**: [GetLatka - Bloomreach](https://getlatka.com/companies/bloomreach), [Axios - Bloomreach crosses $200M](https://www.axios.com/pro/retail-deals/2024/11/22/bloomreach-revenue-growth-search-ecommerce-shopping), [Inc. 5000 선정](https://www.bloomreach.com/en/news/2024/bloomreach-named-to-inc-5000/)

---

## 제품 포트폴리오

Bloomreach는 **Commerce Experience Cloud** 플랫폼으로, Clarity는 그 중 하나:

| 제품 | 기능 |
|------|------|
| **Clarity** | AI Conversational Shopping |
| Discovery | 이커머스 검색/추천 |
| Engagement | 마케팅 자동화 (CDP) |
| Content | Headless CMS |

→ Clarity는 **기존 제품 위에 얹는 AI 레이어**

---

## Clarity: 파는 가치 (Value Proposition)

### 핵심 메시지

**"최고의 판매원을 온라인에 배치한다"**

| 문제 | Clarity 해결책 |
|------|---------------|
| 상품 발견 어려움 | AI 대화로 니즈 파악 → 추천 |
| 구매 전 질문 | 사이즈, 호환성, 관리법 안내 |
| 장바구니 이탈 | 체크아웃 단계에서 질문 응대 |
| 24/7 대응 불가 | AI가 항상 응대 |

### 고객 성과

| 고객 | 결과 |
|------|------|
| **TFG** (남아프리카 최대 패션 리테일) | 전환율 **35.2%↑**, RPV **39.8%↑**, 이탈률 28.1%↓ |
| 평균 | 전환율 9%↑, AOV 20%↑ |
| Black Friday 2024 | 쇼퍼 참여 **113%↑** |

> **출처**: [TFG Case Study](https://www.bloomreach.com/en/case-studies/tfg-boosts-online-conversion-rate-with-bloomreach-clarity)

---

## Clarity: 기능 상세

### 작동 방식

```
쇼퍼 쿼리 입력
    ↓
LLM (Gemini 2.0 Flash) 의도 파악
    ↓
상품 데이터 벡터 검색 (Qdrant)
    ↓
개인화 추천 + 대화 응답
```

### 기술 스택

| 구성요소 | 기술 |
|----------|------|
| LLM | Gemini 2.0 Flash |
| 임베딩 | Vertex AI |
| 벡터 DB | Qdrant |
| 데이터 소스 | Bigtable, S3, Shopify API |

### 핵심 기능

| 기능 | 설명 |
|------|------|
| **Proactive 개입** | 검색 결과 깊이 들어가거나, PDP에서 멈출 때 트리거 |
| **옴니채널** | 웹, 이메일, SMS 연결 |
| **개인화** | 브라우징, 구매 이력, 장바구니 기반 |
| **브랜드 톤** | 브랜드 보이스에 맞게 커스터마이징 |
| **다국어** | 17개국 지원 |

### Rep AI와 비교

| 기능 | Rep AI | Bloomreach Clarity |
|------|--------|-------------------|
| Proactive 감지 | ⭕ 92% 정확도 | ⭕ |
| 대화형 추천 | ⭕ | ⭕ |
| 채팅 내 장바구니 | ⭕ | ? |
| 옴니채널 | △ | ⭕ 이메일, SMS |
| CDP 연동 | ❌ | ⭕ (자체 Engagement) |
| 다국어 | ⭕ | ⭕ 17개국 |

---

## 타겟 고객

### 세그먼트

| 세그먼트 | 적합도 |
|----------|--------|
| **Enterprise** | ⭕ 핵심 타겟 |
| Mid-Market | △ 가능하나 비용 부담 |
| SMB | ❌ |

### 가격

| 항목 | 내용 |
|------|------|
| 모델 | 커스텀 견적 (사용량 기반) |
| 최소 연간 계약 | **$50K~$100K+** |
| 셀프서브 | ❌ 없음 |

→ **엔터프라이즈 세일즈 모델**, SMB/Mid 접근 어려움

### 대표 고객

| 고객 | 업종 |
|------|------|
| TFG | 패션 리테일 (남아프리카) |
| Pandora | 주얼리 |
| American Eagle | 패션 |
| Puma | 스포츠웨어 |
| Marks & Spencer | 리테일 |
| Bosch | 가전 |

---

## Rep AI vs Bloomreach Clarity

| 항목 | Rep AI | Bloomreach Clarity |
|------|--------|-------------------|
| **타겟** | SMB~Mid | **Enterprise** |
| **고객 수** | 500 | 1,400+ (전체) |
| **펀딩** | $8.2M | **$422M+** |
| **밸류에이션** | ? | **$2.2B** |
| **가격** | $299/월~ | $50K+/년 |
| **플랫폼** | Shopify 전용 | 플랫폼 무관 |
| **셀프서브** | ⭕ | ❌ |
| **제품 범위** | Conversational만 | CDP, Search, CMS 포함 |

### 포지션 차이

```
Enterprise ─────── Bloomreach Clarity
                        │
Mid-Market ─────── Rep AI
                        │
SMB ─────────────── Rep AI
```

---

## 출처

- [Bloomreach 공식 사이트](https://www.bloomreach.com)
- [Bloomreach Clarity 제품 페이지](https://www.bloomreach.com/en/products/clarity)
- [GetLatka - Bloomreach Revenue](https://getlatka.com/companies/bloomreach)
- [TFG Case Study](https://www.bloomreach.com/en/case-studies/tfg-boosts-online-conversion-rate-with-bloomreach-clarity)
- [Bloomreach Funding Announcement](https://www.bloomreach.com/en/blog/with-usd175-million-in-funding-bloomreach-is-authoring-the-next-chapter-of-e-commerce)
