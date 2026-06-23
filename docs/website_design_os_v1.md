# Website Design OS v1

Website Design OS는 업무자동화 시스템 안에서 홈페이지 기획, Figma 디자인, 개발 전달, 운영 개선까지 관리하기 위한 웹사이트 제작 시스템이다.

이 문서는 태영님이 필요한 4개 웹사이트를 각각 독립적으로 설계하고 제작하기 위한 기준 문서다.

---

## 1. Core Purpose

홈페이지는 단순한 소개 페이지가 아니라 목적에 따라 구조가 달라져야 한다.

Website Design OS의 목적은 다음과 같다.

- 사이트별 목적 정의
- 타깃 고객 정의
- 페이지 구조 설계
- 섹션별 카피 작성
- Figma 와이어프레임 제작
- PC / Mobile 반응형 디자인
- 개발 전달용 가이드 생성
- 운영 후 개선 기록

---

## 2. Required Websites

현재 필요한 웹사이트는 총 4개다.

```text
1. Tattoo Shop Website
2. Ethermall Company Website
3. Ethermall Market Website
4. Personal Website
```

각 사이트는 목적이 다르므로 별도 프로젝트로 관리한다.

---

## 3. Website Project Structure

Recommended GitHub path:

```text
websites/
├─ tattoo_shop/
│  ├─ website_brief_v1.md
│  ├─ sitemap_v1.md
│  ├─ copy_v1.md
│  └─ figma_design_log_v1.md
├─ ethermall_company/
│  ├─ website_brief_v1.md
│  ├─ sitemap_v1.md
│  ├─ copy_v1.md
│  └─ figma_design_log_v1.md
├─ ethermall_market/
│  ├─ website_brief_v1.md
│  ├─ sitemap_v1.md
│  ├─ copy_v1.md
│  └─ figma_design_log_v1.md
└─ personal_homepage/
   ├─ website_brief_v1.md
   ├─ sitemap_v1.md
   ├─ copy_v1.md
   └─ figma_design_log_v1.md
```

---

## 4. Website Type A: Tattoo Shop Website

### Purpose

예약 전환과 포트폴리오 신뢰 형성이 핵심이다.

### Main Goals

- 타투샵 분위기 전달
- 아티스트 전문성 전달
- 작업 포트폴리오 제공
- 예약 문의 전환
- 위치와 상담 방식 안내

### Recommended Sections

```text
1. Hero / 첫 화면
2. Tattoo Style Introduction
3. Artist Profile
4. Portfolio Gallery
5. Work Process
6. Reservation Guide
7. Care Guide / 주의사항
8. Location / Contact
```

### Visual Direction

- Black / White 기반
- 강한 대비
- 작품 사진 중심
- 고급스럽고 전문적인 분위기
- 예약 버튼 명확하게 배치

---

## 5. Website Type B: Ethermall Company Website

### Purpose

이더몰마켓의 회사 및 브랜드 사업 역량을 소개하는 사이트다.

판매보다는 회사 신뢰, 사업 방향, 브랜드 운영 역량을 보여주는 것이 목적이다.

### Main Goals

- 회사 소개
- 브랜드 사업 소개
- 운영 브랜드 소개
- 상품 기획 / 소싱 역량 전달
- 온라인 판매 / 마케팅 역량 전달
- 협업, 입점, 제휴 문의 유도

### Recommended Sections

```text
1. Hero / 회사 비전
2. About Ethermall
3. Brand Business Overview
4. Operating Brands
5. Product Planning & Sourcing
6. Online Sales & Marketing Capability
7. Portfolio / Case Study
8. Partnership / Contact
```

### Visual Direction

- Corporate + Commerce hybrid
- 신뢰감 있는 레이아웃
- 밝고 깔끔한 배경
- 브랜드 카드형 구성
- 수치 / 프로세스 / 운영역량 시각화

### Key Message Draft

```text
브랜드를 만들고,
상품을 기획하고,
온라인에서 성장시키는 회사
```

---

## 6. Website Type C: Ethermall Market Website

### Purpose

이더몰마켓의 판매 사이트다.

상품 탐색, 구매, 리뷰, 이벤트, 카테고리 이동이 핵심이다.

### Main Goals

- 상품 판매
- 카테고리 탐색
- 베스트 상품 노출
- 신상품 노출
- 브랜드별 상품 탐색
- 이벤트 / 기획전 운영
- 리뷰 신뢰 형성

### Recommended Sections

```text
1. Main Banner
2. Category Navigation
3. Best Products
4. New Products
5. Brand Collection
6. Event / Promotion
7. Review Section
8. Product Detail Pages
9. Cart / Checkout Flow
```

### Visual Direction

- Clean commerce UI
- 상품 카드 중심
- 검색 / 필터 / 카테고리 중요
- 모바일 쇼핑 최적화
- 장바구니 / 구매 버튼 명확하게

---

## 7. Website Type D: Personal Website

### Purpose

태영님의 개인 브랜딩과 포트폴리오를 보여주는 사이트다.

### Possible Positioning

- 사진가
- 디자이너
- 브랜드 운영자
- 자동화 시스템 기획자
- 콘텐츠 제작자

### Main Goals

- 개인 소개
- 전문 분야 소개
- 프로젝트 포트폴리오
- 작업 철학 전달
- 문의 / 협업 연결
- GitHub / Figma / SNS 연결

### Recommended Sections

```text
1. Hero / Personal Identity
2. About
3. Expertise
4. Projects
5. Portfolio Gallery
6. Design OS / Automation Work
7. Contact
```

### Visual Direction

- 개인의 사진/작업물 중심
- 미니멀하고 신뢰감 있는 레이아웃
- 포트폴리오가 돋보이는 구성
- 너무 복잡하지 않은 구조

---

## 8. Figma Production Workflow

각 홈페이지는 Figma에서 다음 순서로 제작한다.

```text
1. Website Brief 작성
2. Sitemap 작성
3. Section Copy 작성
4. PC Wireframe 제작
5. Mobile Wireframe 제작
6. Visual Design 제작
7. Component / Style 정리
8. Prototype 연결
9. QA
10. 개발 전달용 Export
```

---

## 9. Standard Figma File Naming

```text
Tattoo_Shop_Website_v1
Ethermall_Company_Website_v1
Ethermall_Market_Website_v1
Personal_Homepage_v1
```

---

## 10. Website Design QA Checklist

공통 검수 항목:

- 사이트 목적이 명확한가?
- 첫 화면에서 누구를 위한 사이트인지 알 수 있는가?
- CTA가 명확한가?
- PC와 모바일 구조가 분리되어 있는가?
- 섹션 흐름이 자연스러운가?
- 텍스트가 너무 많은가?
- 브랜드/개인/회사 톤이 일관적인가?
- 개발자가 구현하기 쉬운 구조인가?
- 이미지와 카피가 실제 내용과 맞는가?
- 허위 정보나 과장 표현이 없는가?

---

## 11. Recommended Priority

현재 우선순위는 다음과 같이 잡는다.

```text
1. Ethermall Company Website
2. Ethermall Market Website
3. Personal Website
4. Tattoo Shop Website
```

이유:

- 회사 소개 사이트가 먼저 있어야 사업의 기준이 잡힌다.
- 판매 사이트는 회사/브랜드 구조가 정리된 뒤 제작하는 것이 효율적이다.
- 개인 홈페이지는 포트폴리오와 자동화 시스템 소개를 연결할 수 있다.
- 타투샵 홈페이지는 별도의 브랜드 톤과 사진 자료가 필요하다.

---

## 12. Connection to Business Automation System

Website Design OS는 업무자동화 시스템의 다음 영역과 연결된다.

```text
업무자동화 시스템
├─ 브랜드 관리
├─ 상품 관리
├─ 콘텐츠 관리
├─ 디자인 자동화
├─ 판매 관리
├─ 고객 문의 관리
├─ 포트폴리오 관리
└─ 성과 분석
```

각 홈페이지 프로젝트는 Project Archive에 기록한다.

---

## 13. Next Action

가장 먼저 제작할 Figma 테스트 화면은 다음을 추천한다.

```text
Ethermall Company Website
PC Main Hero Section
1440 x 1024
```

이 화면을 먼저 만들면 회사/브랜드사업 소개 사이트의 전체 방향을 빠르게 확인할 수 있다.
