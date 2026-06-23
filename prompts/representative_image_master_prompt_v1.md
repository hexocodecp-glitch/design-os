# Representative Image Master Prompt v1

대표이미지, 썸네일, 제품 메인 이미지, SNS 첫 장, 스마트스토어 대표이미지를 만들기 위한 공통 프롬프트 규칙이다.

---

## 1. Purpose

대표이미지는 고객이 가장 먼저 보는 이미지다.

대표이미지의 목적은 예쁜 이미지를 만드는 것이 아니라, 3초 안에 다음을 전달하는 것이다.

- 어떤 제품인가
- 누구를 위한 것인가
- 핵심 혜택은 무엇인가
- 왜 클릭해야 하는가
- 브랜드 신뢰감이 있는가

---

## 2. Core Principle

대표이미지는 클릭률과 첫인상을 결정한다.

따라서 대표이미지는 다음 기준을 따른다.

```text
제품 중심
핵심 메시지 중심
모바일 가독성 중심
플랫폼 규정 준수
브랜드 일관성 유지
원본 자산 보호
```

---

## 3. Asset Lock Rule

업로드된 원본 제품 이미지는 절대 변형하지 않는다.

금지:

- 제품 색상 변경
- 제품 형태 변경
- 제품 비율 변경
- 로고 변경
- 버튼 / 구조 / 패키지 변경
- 존재하지 않는 구성품 추가
- 실제 제품과 다른 재질 표현

허용:

- 배경 디자인
- 그림자 추가
- 조명 보정
- 그래픽 요소 추가
- 텍스트 배치
- CTA 배치
- 혜택 배지 추가

원칙:

> 제품은 원본 그대로 유지하고, 주변 디자인만 구성한다.

---

## 4. Representative Image Types

### 4.1 SmartStore Main Image

목적:

- 검색 결과에서 클릭 유도
- 제품 정체성 즉시 전달
- 과장 없이 신뢰감 확보

권장 구성:

- 제품 이미지 크게 배치
- 핵심 혜택 1개
- 짧은 보조 문구
- 깔끔한 배경
- 모바일에서 읽히는 큰 글자

주의:

- 너무 많은 문구 금지
- 복잡한 배경 금지
- 제품보다 모델이 커지는 구성 금지

---

### 4.2 Instagram Card News Cover

목적:

- 첫 장에서 멈춤 유도
- 저장 / 넘김 유도
- 문제 상황을 즉시 자극

권장 구성:

- 강한 후킹 문장
- 감정 또는 문제 상황
- 브랜드 톤에 맞는 이미지
- 카드뉴스 전체 톤과 통일

예시 구조:

```text
[고민/문제]
혼자서는 닿지 않던 등 뒤,
이제 직접 관리하세요
```

---

### 4.3 Detail Page Hero Image

목적:

- 상세페이지 첫 화면에서 USP 전달
- 이탈 방지
- 구매 흐름 시작

권장 구성:

- 제품 메인 비주얼
- 핵심 USP
- 1~2개 보조 근거
- 브랜드 신뢰 요소
- CTA 흐름

---

### 4.4 Blog Thumbnail

목적:

- 검색 결과 / 블로그 목록에서 클릭 유도
- 키워드와 주제 명확화

권장 구성:

- 검색 키워드 포함
- 문제 해결형 제목
- 단순한 배경
- 읽기 쉬운 글자

---

## 5. Prompt Template

아래 템플릿을 사용한다.

```text
[역할]
당신은 20년차 이커머스 대표이미지 디자이너입니다.
스마트스토어, 인스타그램, 상세페이지, 블로그 썸네일의 클릭률과 전환율을 고려하여 대표이미지를 설계합니다.

[목표]
아래 제품/브랜드의 대표이미지를 기획하고 생성 프롬프트를 작성합니다.
목표는 예쁜 이미지가 아니라 3초 안에 제품의 핵심 가치를 전달하고 클릭을 유도하는 것입니다.

[브랜드]
- 브랜드명:
- 브랜드 톤:
- 컬러:
- 금지 톤:

[제품]
- 제품명:
- 카테고리:
- 핵심 USP:
- 고객 문제:
- 타깃 고객:
- 주요 혜택:

[플랫폼]
- 사용 위치: 스마트스토어 / 인스타그램 / 상세페이지 / 블로그 / 광고
- 권장 비율:
- 필수 문구:
- 금지 문구:

[원본 자산 보호]
업로드된 제품 이미지는 형태, 색상, 비율, 로고, 구조를 절대 변경하지 마세요.
제품은 원본 그대로 유지하고 배경, 조명, 그림자, 그래픽, 텍스트만 구성하세요.

[디자인 방향]
- 스타일:
- 배경:
- 조명:
- 그래픽:
- 텍스트 계층:
- CTA:

[출력]
1. 대표이미지 목적
2. 핵심 메시지
3. 레이아웃 구성
4. 텍스트 문구
5. 이미지 생성 프롬프트
6. 금지 요소
7. QA 체크리스트
```

---

## 6. Image Generation Prompt Structure

이미지 생성 프롬프트는 다음 구조를 따른다.

```text
Create a high-converting ecommerce representative image for [PRODUCT].
Use the uploaded product image as the exact original product asset.
Do not alter the product shape, color, logo, proportion, structure, material, or details.
Keep the product visually identical to the original asset.

Design a [STYLE] background with [LIGHTING], [SHADOW], and [GRAPHIC ELEMENTS].
The image should communicate [CORE BENEFIT] within 3 seconds.
Place the product as the main hero object.
Use clean composition, strong visual hierarchy, and mobile-friendly spacing.
Leave clear space for Korean headline text.

Mood: [MOOD]
Color palette: [COLORS]
Platform: [PLATFORM]
Aspect ratio: [RATIO]

Do not create a new product.
Do not redesign the product.
Do not add unverified features.
Do not include distorted text.
```

---

## 7. Copy Rules

대표이미지 문구는 짧아야 한다.

권장:

- 8~16자 메인 카피
- 1개 핵심 혜택
- 숫자는 검증된 경우에만 사용
- 모바일에서 한눈에 읽히는 문장

금지:

- 긴 문장
- 3개 이상 혜택 나열
- 검증되지 않은 수치
- 의료적 효과 단정
- 과장 광고

---

## 8. Layout Rules

대표이미지 레이아웃 우선순위:

1. 제품
2. 핵심 카피
3. 혜택 배지
4. 보조 정보
5. 브랜드 요소

제품은 항상 명확히 보여야 한다.

텍스트가 제품을 가리면 안 된다.

---

## 9. Platform Size Guide

기본 권장 비율:

- 스마트스토어 대표이미지: 1:1
- 인스타그램 카드뉴스 커버: 1:1 또는 4:5
- 상세페이지 히어로: 870px width 기준 세로형
- 블로그 썸네일: 16:9 또는 1:1
- 광고 배너: 플랫폼별 별도 적용

---

## 10. QA Checklist

생성 후 반드시 확인한다.

- 제품 원본이 변형되지 않았는가?
- 색상과 비율이 유지되었는가?
- 로고가 바뀌지 않았는가?
- 핵심 메시지가 3초 안에 보이는가?
- 모바일에서 글자가 읽히는가?
- 문구가 너무 많지 않은가?
- 플랫폼 규정에 맞는가?
- 브랜드 톤과 맞는가?
- 검증되지 않은 기능이나 수치가 없는가?
- 클릭하고 싶은 이유가 있는가?

---

## 11. Archive Rule

대표이미지를 만들 때마다 다음 정보를 Project Archive에 저장한다.

- 대표이미지 목적
- 플랫폼
- 사용 제품
- 사용 원본 자산
- 핵심 카피
- 최종 프롬프트
- 결과 이미지
- QA 결과
- 성과 데이터
- 개선점
