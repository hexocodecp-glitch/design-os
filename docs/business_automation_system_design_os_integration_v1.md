# Business Automation System x Design OS Integration v1

업무자동화 시스템 안에 Design OS 기능을 포함하기 위한 통합 설계 문서다.

이 문서는 Design OS를 별도 디자인 도구가 아니라 전체 업무자동화 시스템의 디자인·콘텐츠·브랜드·자산 관리 모듈로 연결하기 위해 작성한다.

---

## 1. Core Decision

Design OS는 독립 시스템으로만 운영하지 않는다.

업무자동화 시스템 안에 다음 모듈로 포함한다.

```text
업무자동화 시스템
└─ 디자인·콘텐츠 자동화 모듈
   └─ Design OS
```

즉, Design OS는 전체 자동화 프로그램의 하위 핵심 기능이다.

---

## 2. Design OS가 들어가는 위치

업무자동화 시스템 안에서 Design OS는 다음 업무를 담당한다.

- 브랜드 아카이브
- 제품 아카이브
- 제품 마스터팩
- 브랜드 스타일팩
- 카드뉴스 기획
- 상세페이지 기획
- 대표이미지 기획
- 광고 이미지 기획
- 블로그/SNS 이미지 기획
- 제품 사진 관리
- 이미지 업로드 분류
- AI 이미지 생성 기준
- Figma 텍스트/레이아웃 제작 기준
- QA 검수
- 성과 학습 기록

---

## 3. 전체 업무자동화 시스템 안의 연결 구조

```text
업무자동화 시스템
├─ 상품/제품 관리
│  └─ Product Archive / Product Master Pack 연결
├─ 브랜드 관리
│  └─ Brand Archive / Brand Style Pack 연결
├─ 디자인 자동화
│  └─ 대표이미지 / 카드뉴스 / 상세페이지 / 배너 제작
├─ 콘텐츠 자동화
│  └─ 블로그 / SNS / 정보성 콘텐츠 / 캠페인 기획
├─ 마케팅 자동화
│  └─ 광고 소재 / CTA / 후킹 카피 / 전환 구조
├─ 고객반응 관리
│  └─ Customer Voice Archive / 리뷰 / 문의 / 댓글 분석
├─ 경쟁사 분석
│  └─ Competitor Archive / 상세페이지 / 광고 / 가격 / USP 분석
├─ 자산 관리
│  └─ Asset Library / 이미지 업로드 / 분류 / 선택 규칙
├─ QA 관리
│  └─ Asset Lock Rule / Brand Style Check / 과장광고 검수
└─ 학습 관리
   └─ Winning Library / Failure Library / Learning System
```

---

## 4. Design OS 주요 기능의 업무자동화 시스템 반영

### 4.1 Brand Archive

업무자동화 시스템에서 브랜드별 기준 정보를 저장한다.

연결 업무:

- 브랜드 관리
- 콘텐츠 제작
- 디자인 제작
- 광고 제작
- 상세페이지 제작

---

### 4.2 Brand Style Pack

제품 사진 없이 AI 이미지 생성만으로 콘텐츠를 만들 때 브랜드 일관성을 유지한다.

연결 업무:

- 정보성 카드뉴스
- 브랜드 스토리 콘텐츠
- 블로그 썸네일
- 캠페인 이미지
- 키노숲 같은 공간/경험 브랜드 콘텐츠

핵심 규칙:

> 사진이 없어도 브랜드 스타일은 있어야 한다.

---

### 4.3 Product Archive

제품별 판매 논리와 정보를 저장한다.

연결 업무:

- 상품 기획
- 상세페이지 제작
- 대표이미지 제작
- 광고 소재 제작
- FAQ 제작

---

### 4.4 Product Master Pack

반복 제작이 필요한 제품을 고정 자산으로 만든다.

연결 업무:

- 카드뉴스 반복 제작
- 상세페이지 반복 제작
- 대표이미지 제작
- 광고 배너 제작
- 제품별 프롬프트 자동화

예시:

```text
products/lantons/auto_shaker/product_master_pack_v1.md
```

---

### 4.5 Asset Upload & Selection Rule

제품 사진, 상세페이지 캡처, 라이프스타일컷, 리뷰 이미지 등을 업로드하고 자동 분류하는 기준이다.

업무자동화 시스템 안에서는 자산 관리 모듈에 포함한다.

핵심 규칙:

> 이미지는 처음부터 완벽하게 분류하지 않아도 된다. 단, 브랜드별 / 제품별 폴더는 구분한다.

예시:

```text
assets/
├─ lantons/
│  ├─ auto_shaker/
│  │  ├─ raw_uploads/
│  │  ├─ product_photos/
│  │  ├─ lifestyle_photos/
│  │  ├─ detail_page_screenshots/
│  │  └─ selected_for_cardnews/
```

---

### 4.6 Asset Mode System

이미지 제작 방식을 두 가지 모드로 구분한다.

#### Mode A. Product Asset Mode

제품 사진이 있는 경우.

사용 예:

- 랜턴스 자동쉐이커
- 굿케어 마사지건
- 랜턴스 헤어브러시

핵심:

- 제품 원본 보호
- 로고 변경 금지
- 형태 변경 금지
- 색상 변경 금지

---

#### Mode B. Concept Asset Mode

제품 사진 없이 AI 이미지 생성만으로 만드는 경우.

사용 예:

- 키노숲 정보성 카드뉴스
- 브랜드 스토리 콘텐츠
- 블로그 썸네일
- 마케팅 정보 콘텐츠

핵심:

- Brand Style Pack 기준 생성
- 허위 시설/기능/인증 생성 금지
- 브랜드 무드와 컬러 유지

---

### 4.7 Figma Text/Layout Workflow

AI 이미지 생성 시 한국어 텍스트 오류를 줄이기 위해 최종 텍스트와 레이아웃은 Figma에서 처리한다.

업무자동화 시스템에서 Figma는 다음 단계에 연결된다.

```text
AI 시각 자료 생성
↓
Figma 텍스트 레이아웃
↓
모바일 가독성 QA
↓
최종 이미지 Export
```

---

### 4.8 QA Engine

제품형 이미지와 컨셉형 이미지를 모두 검수한다.

검수 항목:

- 제품 원본이 유지되었는가?
- 로고가 바뀌지 않았는가?
- 제품 색상/비율이 유지되었는가?
- 스펙과 수치가 정확한가?
- 과장 광고가 없는가?
- 브랜드 스타일팩과 일치하는가?
- 실제 장소나 시설을 허위로 묘사하지 않았는가?
- 모바일에서 읽히는가?

---

## 5. 업무자동화 시스템 내 Design OS 운영 흐름

```text
브랜드 선택
↓
제품 선택 또는 콘텐츠 주제 선택
↓
Brand Archive 확인
↓
Brand Style Pack 확인
↓
Product Archive 확인
↓
Product Master Pack 확인
↓
Asset Mode 결정
↓
Product Asset Mode 또는 Concept Asset Mode 적용
↓
기획서 생성
↓
카피 생성
↓
이미지 생성 또는 자산 선택
↓
Figma 텍스트/레이아웃
↓
QA 검수
↓
최종 결과물 저장
↓
Project Archive 기록
↓
성과 학습 업데이트
```

---

## 6. 업무자동화 시스템에 추가되어야 할 신규 기능

### 6.1 브랜드 스타일팩 관리 기능

브랜드별 Style Pack을 생성, 수정, 적용할 수 있어야 한다.

필요 데이터:

- 브랜드명
- 무드 키워드
- 컬러
- 폰트
- 이미지 스타일
- 금지 스타일
- 플랫폼 규칙

---

### 6.2 제품 마스터팩 관리 기능

제품별 반복 제작 기준을 저장한다.

필요 데이터:

- 제품명
- USP
- 스펙
- 고객 문제
- 고객 언어
- 제품 보존 규칙
- 카드뉴스 구조
- 이미지 생성 규칙

---

### 6.3 자산 업로드 및 자동 분류 기능

사용자가 이미지를 구분 없이 올려도 AI가 분류할 수 있어야 한다.

단, 최소한 브랜드/제품 폴더는 구분한다.

자동 분류 기준:

- Hero image
- Product photo
- Lifestyle photo
- Detail page screenshot
- Review capture
- Competitor reference
- Selected for card news

---

### 6.4 이미지 제작 모드 선택 기능

작업 시작 시 다음 중 하나를 선택한다.

```text
Product Asset Mode
Concept Asset Mode
```

---

### 6.5 프로젝트 아카이브 자동 저장 기능

완료된 작업은 자동으로 Project Archive에 저장한다.

저장 항목:

- 프로젝트 ID
- 브랜드
- 제품
- 플랫폼
- 기획서
- 카피
- 사용 자산
- 최종 결과물
- QA 결과
- 학습 내용

---

## 7. 현재 GitHub에 반영된 관련 문서

```text
docs/DesignOS_Master_v1.md
docs/brand_style_pack_system_v1.md
docs/asset_upload_and_selection_rule_v1.md
products/lantons/auto_shaker/product_master_pack_v1.md
projects/lantons/auto_shaker/cardnews_001/project_brief_v1.md
```

---

## 8. Next Step

업무자동화 시스템 전체 Master 문서를 별도로 생성하고, 그 안에 Design OS를 공식 하위 모듈로 추가해야 한다.

Recommended next file:

```text
docs/business_automation_master_v1.md
```

이 문서는 전체 팀 구조, 업무 흐름, 각 자동화 모듈과 Design OS의 연결 관계를 정의한다.
