# Asset Upload and Selection Rule v1

Design OS에서 이미지 자료를 업로드하고, AI가 자동 분류하여 카드뉴스·상세페이지·광고 제작에 활용하기 위한 기본 규칙이다.

---

## 1. Core Principle

이미지는 처음부터 완벽하게 정리해서 올릴 필요는 없다.

다만 정확도를 높이기 위해 최소한 제품별 폴더는 분리한다.

Recommended Minimum Structure:

```text
LANTONS/
├─ Auto_Shaker
├─ Hair_Brush
└─ Other_Products
```

---

## 2. Why Product-Level Folder Separation Matters

구분 없이 모든 제품 이미지를 섞으면 AI가 제품을 혼동할 가능성이 높아진다.

예:

- LANTONS 자동쉐이커
- LANTONS 헤어브러시
- GOODCARE 마사지건
- 키노숲 공간 사진

이 이미지들이 섞이면 카드뉴스 제작 시 잘못된 제품을 선택할 수 있다.

따라서 최소 기준은 다음과 같다.

> 브랜드별 폴더 + 제품별 폴더는 반드시 분리한다.

---

## 3. Recommended Folder Structure

```text
assets/
├─ lantons/
│  ├─ auto_shaker/
│  │  ├─ raw_uploads/
│  │  ├─ product_photos/
│  │  ├─ lifestyle_photos/
│  │  ├─ detail_page_screenshots/
│  │  ├─ review_captures/
│  │  └─ selected_for_cardnews/
│  └─ hair_brush/
│     ├─ raw_uploads/
│     ├─ product_photos/
│     └─ lifestyle_photos/
├─ goodcare/
└─ kinosoop/
```

---

## 4. Upload Rule

처음 업로드할 때는 세부 분류 없이 넣어도 된다.

Allowed:

```text
assets/lantons/auto_shaker/raw_uploads/
```

이후 AI가 다음 기준으로 분류한다.

- Hero image
- Front product image
- 45-degree product image
- Color lineup
- Mixing image
- Cleaning image
- Lifestyle image
- Office scene
- Gym scene
- Car cup holder scene
- Bag storage scene
- Detail page screenshot
- Review capture
- Competitor reference

---

## 5. Optional File Naming Rule

정확도를 더 높이고 싶다면 아래 파일명 규칙을 사용한다.

```text
AS_HERO_001.png
AS_FRONT_001.png
AS_45DEG_001.png
AS_COLOR_001.png
AS_MIXING_001.png
AS_CLEANING_001.png
AS_LIFESTYLE_001.png
AS_OFFICE_001.png
AS_CAR_001.png
AS_BAG_001.png
AS_DETAIL_001.png
AS_REVIEW_001.png
```

AS = Auto Shaker

---

## 6. AI Selection Priority

카드뉴스 제작 시 AI는 다음 순서로 이미지를 선택한다.

1. 제품 원본 정확도가 높은 이미지
2. 로고와 형태가 잘 보이는 이미지
3. 카드 메시지와 맞는 이미지
4. 배경이 깔끔한 이미지
5. 텍스트를 얹기 쉬운 여백이 있는 이미지
6. 브랜드 톤과 맞는 이미지

---

## 7. Card News Asset Selection Rule

Instagram carousel card news uses one image per card.

Do not create one collage containing 10 cards.

Recommended:

```text
card_01.png
card_02.png
card_03.png
card_04.png
card_05.png
card_06.png
card_07.png
card_08.png
card_09.png
card_10.png
```

Each card should be:

- 1080 x 1350px
- 4:5 ratio
- one message
- one visual focus
- one emotion

---

## 8. Product Preservation Rule

When using product photos, never alter:

- Product shape
- Logo
- Color
- Proportion
- Material
- Button position
- Cap structure
- Printed text
- Package shape

AI may only change:

- Background
- Lighting
- Shadow
- Graphic elements
- Text layer
- CTA
- Composition around the product

---

## 9. When AI Can Generate Missing Images

If the following images are missing, AI may generate the background or lifestyle scene.

Allowed AI generation:

- Gym lifestyle background
- Office desk scene
- Car cup holder background
- Bag storage scene
- Cafe lifestyle scene
- Morning routine scene

Important:

> The product itself should use the original product asset whenever possible.

---

## 10. Recommended Workflow

1. User uploads all product-related images into the product folder.
2. AI classifies them into asset types.
3. AI selects the best images for card news.
4. AI creates a product master pack.
5. AI creates a card news storyboard.
6. AI generates or prepares card backgrounds.
7. Text is finalized in Figma.
8. Final outputs are saved to Project Archive.

---

## 11. Design OS Rule

> 자료는 완벽하게 정리해서 시작하지 않아도 된다. 단, 제품별 폴더만 구분하면 AI가 이후 분류하고 선택할 수 있다.

