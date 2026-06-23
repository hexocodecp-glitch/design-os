# Brand Style Pack System v1

사진이나 제품 원본이 없는 상황에서도 브랜드 일관성을 유지하며 카드뉴스, 대표이미지, 블로그 이미지, 광고 배너, 상세페이지 섹션 이미지를 생성하기 위한 시스템이다.

---

## 1. Why This System Exists

모든 프로젝트에 제품 사진이나 실제 촬영 이미지가 있는 것은 아니다.

예:

- 정보성 카드뉴스
- 브랜드 스토리 콘텐츠
- 블로그 썸네일
- 인스타그램 교육형 콘텐츠
- 키노숲 같은 공간·경험 브랜드 콘텐츠
- 마케팅 정보 콘텐츠
- 캠페인 컨셉 이미지

이 경우 AI 이미지 생성만으로도 콘텐츠를 만들어야 한다.

하지만 사진이 없다고 아무 이미지나 만들면 브랜드 일관성이 무너진다.

따라서 브랜드별로 고정된 스타일 기준을 만들어야 한다.

---

## 2. Asset Mode

Design OS는 이미지 제작 방식을 두 가지 모드로 구분한다.

---

### Mode A. Product Asset Mode

실제 제품이 존재하고, 제품 이미지가 필요한 경우.

Examples:

- LANTONS Auto Shaker
- LANTONS Hair Brush
- GOODCARE Massage Gun
- GOODCARE Shower Brush

Rules:

- Original product asset required
- Product shape must not change
- Logo must not change
- Color must not change
- Proportion must not change
- Product must not be regenerated from scratch

Use when:

- Product detail page
- SmartStore representative image
- Product card news
- Product ad banner

---

### Mode B. Concept Asset Mode

제품 사진 없이 컨셉, 정보, 감성, 상황 이미지만으로 콘텐츠를 만드는 경우.

Examples:

- 키노숲 육아 정보 카드뉴스
- 브랜드 스토리 콘텐츠
- 인스타그램 알고리즘 카드뉴스
- 건강 정보 콘텐츠
- 블로그 썸네일
- 캠페인 컨셉 비주얼

Rules:

- No original product asset required
- Brand Style Pack must be used
- Do not invent false facilities, features, people, product specs, or certifications
- Use brand-consistent color, mood, lighting, layout, and typography
- If the content is about a real place, do not generate misleading space features unless verified

---

## 3. Brand Style Pack Structure

Each brand should have a Brand Style Pack.

Recommended path:

```text
brand_style_packs/
├─ goodcare/style_pack_v1.md
├─ lantons/style_pack_v1.md
└─ kinosoop/style_pack_v1.md
```

Each Style Pack includes:

- Brand position
- Mood keywords
- Visual keywords
- Color palette
- Typography direction
- Photography style
- Illustration style
- Layout style
- AI image generation style
- Forbidden style
- Platform-specific rules
- QA checklist

---

## 4. Brand Style Pack Template

```md
# [Brand Name] Brand Style Pack v1

## Brand Position

## Mood Keywords

## Visual Keywords

## Color Palette

## Typography Direction

## Photography Style

## Illustration / Graphic Style

## Layout Rule

## AI Image Generation Rule

## Forbidden Style

## Platform Rules

## QA Checklist
```

---

## 5. Concept Asset Generation Workflow

When there is no product photo, use this workflow.

```text
1. Identify brand
2. Load Brand Archive
3. Load Brand Style Pack
4. Define content objective
5. Define target audience
6. Define message
7. Define platform and size
8. Generate visual direction
9. Generate image
10. Add text in Figma
11. QA against Brand Style Pack
12. Save to Project Archive
```

---

## 6. Concept Image Prompt Framework

Use this framework for AI-generated concept images.

```text
Create a brand-consistent concept image for [BRAND].

Brand mood: [MOOD KEYWORDS]
Visual style: [VISUAL STYLE]
Color palette: [COLORS]
Lighting: [LIGHTING]
Composition: [LAYOUT]
Platform: [PLATFORM]
Size: [SIZE]

The image should communicate: [MESSAGE]
Target audience: [TARGET]

Do not include unverified product claims, fake logos, fake certifications, false facilities, or misleading details.
Keep the design consistent with the brand style pack.
Leave clean space for Korean text overlay.
```

---

## 7. Concept Asset Rules by Brand Type

### Product Brand

Even without a product image, the concept should stay close to the product category.

Example:

- wellness lifestyle
- self-care routine
- desk setup
- gym routine
- morning routine

Avoid:

- unrelated luxury objects
- unrealistic CGI products
- fake product packages

---

### Space Brand

For a real location or offline space, image generation must be careful.

Allowed:

- mood image
- symbolic image
- general atmosphere
- verified interior style

Avoid:

- fake facilities
- fake rooms
- fake exterior
- misleading attraction images
- outdoor concept if the brand is indoor

---

### Information Content Brand

For educational or informational card news, use simple metaphor visuals.

Allowed:

- abstract graphics
- icon system
- editorial images
- simple lifestyle scene

Avoid:

- cluttered infographic
- too many icons
- unrelated stock-like image

---

## 8. Figma Rule

For Concept Asset Mode, AI should usually generate the visual base only.

Final text should be added in Figma.

Reasons:

- Korean text accuracy
- Font control
- Layout consistency
- Easy revisions
- Reusable template creation

---

## 9. QA Checklist

Before using a concept image, check:

- Does it match the brand mood?
- Does it use the correct color family?
- Does it avoid false product or facility claims?
- Does it leave enough space for text?
- Does it match the platform size?
- Does it look like the same brand as previous content?
- Is it too generic or stock-like?
- Is it misleading?

---

## 10. Design OS Rule

> 제품 사진이 없을 때는 Asset Lock Rule이 아니라 Brand Style Pack Rule을 기준으로 생성한다.

> 사진이 없어도 브랜드 스타일은 있어야 한다.

---

## 11. Next Required Brand Style Packs

Priority:

1. LANTONS Brand Style Pack
2. GOODCARE Brand Style Pack
3. KINOSOOP Brand Style Pack

These style packs should be created before large-scale image generation.
