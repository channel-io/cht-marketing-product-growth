# 빌더사별 연동 스펙 정리

## 개요

채널톡과 연동 가능한 빌더사 목록과 각 빌더사별 수집되는 고객 프로필, 이벤트 정보를 정리한 문서.

> **참고**: 이 문서는 공식 개발자 문서 기반으로 작성됨. 정확한 최신 정보는 [채널톡 개발자 문서](https://developers.channel.io) 참고.

---

## 연동 가능한 빌더사

| 빌더사 | 연동 수준 | 비고 |
|--------|----------|------|
| **카페24 (Cafe24)** | 풍부 | 이벤트 14개, 프로필 20개+ |
| **샵바이 (Shop by)** | 중간 | 이벤트 3개, 주문 내역 연동 (2023.11~) |
| **아임웹 (Imweb)** | 제한적 | 기본 프로필 + 제한된 이벤트 |
| **고도몰** | 제한적 | 기본 프로필 + 제한된 이벤트 |
| **메이크샵** | 제한적 | 기본 프로필 + 제한된 이벤트 |
| **식스샵** | 제한적 | 기본 프로필 + 제한된 이벤트 |
| **가비아 퍼스트몰** | 제한적 | 기본 프로필 + 제한된 이벤트 |
| **쇼피파이 (Shopify)** | 제한적 | 기본 프로필 + 제한된 이벤트 |
| **워드프레스** | 제한적 | 기본 프로필 + 제한된 이벤트 |
| **셀러허브 스토어** | 제한적 | 기본 프로필 + 제한된 이벤트 |
| 네이버 스마트스토어 | 제한적 | 직접 설치 불가, 주문 내역만 연동 |

---

## 카페24 (Cafe24)

### 고객 프로필

| 데이터 | 설명 |
|--------|------|
| memberId | 회원 고유값 |
| name | 이름 |
| email | 이메일 |
| mobileNumber | 휴대폰 번호 |
| gender | 성별 |
| signedUpAt | 가입일시 |
| groupName | 회원 등급 |
| availableMileage | 잔여 마일리지 |
| totalDeposit | 총 예치금 |
| couponCount | 보유 쿠폰 수 |
| cartCount | 장바구니 상품 수 |
| cartPrice | 장바구니 총 금액 |
| wishCount | 위시리스트 상품 수 |
| recentPurchaseAmount | 최근 구매 금액 (기본 3개월) |
| recentPurchaseCount | 최근 구매 횟수 (기본 3개월) |
| lastCheckoutCompletedAt | 최근 주문 시간 |
| unsubscribeEmail | 이메일 수신거부 여부 |
| unsubscribeTexting | 문자 수신거부 여부 |
| mallId | 쇼핑몰 ID |
| shopNo | 쇼핑몰 번호 |
| currency | 화폐 단위 |

### 이벤트

| 이벤트 | 설명 | 주요 속성 |
|--------|------|----------|
| SignUp | 회원 가입 | id, name |
| CustomerGradeChange | 등급 변경 | grade |
| ProductView | 상품 조회 | id, name, price |
| AddToWish | 위시리스트 추가 | id, name |
| AddToCart | 장바구니 담기 | id, name, quantity, amount, currency, variantId, options |
| CheckoutBegin | 주문서 작성 | - |
| CheckoutComplete | 주문 완료 | id, totalAmount, paymentMethods, shippedAmount, products |
| Purchase | 결제 완료 | id, totalAmount, paymentMethods, shippedAmount, products |
| ShippingBegin | 배송 시작 | id, orderId, trackingNumber, shippingCompany, products |
| ShippingComplete | 배송 완료 | id, orderId, trackingNumber, shippingCompany, products |
| CancelAccepted | 취소 접수 | id, orderId, currency, products |
| ReturnAccepted | 반품 접수 | id, orderId, currency, products |
| ExchangeAccepted | 교환 접수 | id, orderId, originalProducts, exchangedProducts |
| Refund | 환불 완료 | id, orderId, currency, products, refundAmount |

### 참고
- [카페24 개발자 문서](https://developers.channel.io/docs/cafe24-app)
- [카페24 설치 가이드](https://guide-kr.channel.io/2614fcfb-0c88-4ac1-ae5c-3a5791fef75e)

---

## 샵바이 (Shop by)

### 고객 프로필

| 데이터 | 설명 |
|--------|------|
| memberId | 회원 고유값 (회원 번호) |
| name | 이름 |
| email | 이메일 |
| mobileNumber | 휴대폰 번호 |
| groupName | 회원 등급 |
| signedUpAt | 가입일시 |
| extMemberId | 샵바이 로그인 ID |
| unsubscribeEmail | 이메일 수신거부 여부 |
| unsubscribeTexting | 문자 수신거부 여부 |
| lastCheckoutCompletedAt | 최근 주문 시간 |

### 이벤트

| 이벤트 | 설명 | 주요 속성 |
|--------|------|----------|
| SignUp | 회원 가입 | id, name |
| ProductView | 상품 조회 | id, name, price |
| CheckoutComplete | 주문 완료 | id, totalAmount, paymentMethods, shippedAmount, products |

### 참고
- [샵바이 개발자 문서](https://developers.channel.io/docs/%EC%83%B5%EB%B0%94%EC%9D%B4-shop-by)

---

## 아임웹 (Imweb)

### 고객 프로필

| 데이터 | 설명 |
|--------|------|
| memberId | 회원 고유값 |
| name | 이름 |
| email | 이메일 |
| mobileNumber | 휴대폰 번호 |

> 상세 프로필 정보는 개발자 문서에서 확인 필요

### 이벤트

| 이벤트 | 설명 |
|--------|------|
| SignUp | 회원 가입 |
| CheckoutComplete | 주문 완료 |

> 상세 이벤트 목록은 개발자 문서에서 확인 필요

### 참고
- [아임웹 설치 가이드](https://imweb.me/faq?mode=view&category=29&category2=47&idx=36831)

---

## 기타 빌더사 (고도몰, 메이크샵, 식스샵 등)

### 공통 특징

- 기본 고객 프로필 (이름, 이메일, 휴대폰) 연동
- 제한된 이벤트 지원 (SignUp, CheckoutComplete 등 기본 이벤트)
- 상세 스펙은 각 빌더사별 개발자 문서 참고

### 참고
- [빌더사 설치 가이드](https://developers.channel.io/docs/kr-builder-installation)
- [이벤트 정보](https://docs.channel.io/help/ko/articles/%EC%9D%B4%EB%B2%A4%ED%8A%B8-%EC%A0%95%EB%B3%B4-353347a0)

---

## 빌더사별 이벤트 지원 비교

| 이벤트 | 카페24 | 샵바이 | 아임웹 | 기타 |
|--------|:------:|:------:|:------:|:----:|
| SignUp | ✅ | ✅ | ✅ | ✅ |
| ProductView | ✅ | ✅ | ? | ? |
| AddToWish | ✅ | ❌ | ? | ? |
| AddToCart | ✅ | ❌ | ? | ? |
| CheckoutBegin | ✅ | ❌ | ? | ? |
| CheckoutComplete | ✅ | ✅ | ✅ | ✅ |
| Purchase | ✅ | ❌ | ? | ? |
| ShippingBegin | ✅ | ❌ | ❌ | ❌ |
| ShippingComplete | ✅ | ❌ | ❌ | ❌ |
| CancelAccepted | ✅ | ❌ | ❌ | ❌ |
| ReturnAccepted | ✅ | ❌ | ❌ | ❌ |
| ExchangeAccepted | ✅ | ❌ | ❌ | ❌ |
| Refund | ✅ | ❌ | ❌ | ❌ |

> `?` = 개발자 문서에서 확인 필요

---

## 자동 설정 프리셋 적용 가능 여부

| 프리셋 | 필요 이벤트 | 카페24 | 샵바이 | 아임웹 | 기타 |
|--------|------------|:------:|:------:|:------:|:----:|
| 가입 유도 팝업 + 쿠폰 | (이벤트 불필요) | ✅ | ✅ | ✅ | ✅ |
| 장바구니 이탈 리마인드 | AddToCart | ✅ | ❌ | ? | ? |
| 최근 본 상품 추천 | ProductView | ✅ | ✅ | ? | ? |

---

## 시사점

1. **카페24가 가장 풍부한 연동 제공** - 대부분의 프리셋 구현 가능
2. **샵바이는 중간 수준** - 기본 프리셋 일부 가능
3. **아임웹/기타는 제한적** - 추가 확인 필요, GTM 등 별도 설정 필요할 수 있음
4. **빌더사별 프리셋 분기 필요** - 연동 수준에 따라 제공 가능한 프리셋이 다름
