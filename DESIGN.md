---
name: 곽성은 포트폴리오 Hub
description: 기획서 한 장에서 서비스 운영까지 — 게임 기획자 & PM 포트폴리오
colors:
  signal-red: "#e5484d"
  signal-red-deep: "#c93a3e"
  signal-red-strong: "#b0302f"
  ink: "#0a0a0a"
  graphite: "#6b6b6b"
  paper: "#fafafa"
  sheet: "#ffffff"
  grid-line: "#e6e6e6"
  crosshair: "#c2c2c2"
typography:
  display:
    fontFamily: "IBM Plex Sans, Inter, sans-serif"
    fontSize: "clamp(2.4rem, 5vw, 4.2rem)"
    fontWeight: 600
    lineHeight: 1.08
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "IBM Plex Sans, Inter, sans-serif"
    fontSize: "clamp(1.6rem, 2.8vw, 2.3rem)"
    fontWeight: 600
    lineHeight: 1.15
    letterSpacing: "-0.01em"
  title:
    fontFamily: "IBM Plex Sans, Inter, sans-serif"
    fontSize: "1.15rem"
    fontWeight: 600
    letterSpacing: "-0.01em"
  body:
    fontFamily: "IBM Plex Sans, Inter, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "JetBrains Mono, IBM Plex Mono, ui-monospace, monospace"
    fontSize: "0.75rem"
    fontWeight: 500
    letterSpacing: "0.04em"
rounded:
  none: "0px"
spacing:
  xs: "8px"
  sm: "16px"
  unit: "24px"
  card: "32px"
  section-sm: "64px"
  section: "96px"
components:
  button-primary:
    backgroundColor: "{colors.signal-red-deep}"
    textColor: "{colors.sheet}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "0 28px"
    height: "48px"
  button-primary-hover:
    backgroundColor: "{colors.signal-red-strong}"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "0 28px"
    height: "48px"
  button-outline-hover:
    textColor: "{colors.signal-red}"
  card:
    backgroundColor: "{colors.sheet}"
    rounded: "{rounded.none}"
    padding: "{spacing.card}"
  tag:
    backgroundColor: "transparent"
    textColor: "{colors.graphite}"
    rounded: "{rounded.none}"
    padding: "5px 10px"
  nav-cta:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
    padding: "7px 14px"
  nav-cta-hover:
    backgroundColor: "{colors.signal-red-strong}"
    textColor: "{colors.sheet}"
---

# Design System: 곽성은 포트폴리오 Hub

## Overview

**Creative North Star: "The Planner's Grid Notebook"**

이 사이트는 기획자의 모눈 노트를 펼쳐 놓은 모양이다. 24px 점 격자가 종이 전체에 깔려 있고, 그 위에 흰 시트(카드)를 핀으로 꽂듯 올린다. 모서리마다 작은 십자 마커가 있다. 모노스페이스 인덱스(`[01]`, `// INTRO`)는 노트 여백의 메모 번호처럼 읽히고, 구조와 순서가 곧 사고 과정의 증거가 된다.

밀도는 중간이다. 섹션 사이 여백은 넉넉하게(96px), 섹션 안의 정보는 촘촘하게 정리한다. 장식은 격자, 십자 마커, 인덱스 라벨 세 가지뿐이다. 색은 거의 무채색이고, 강조색 하나(Signal Red)가 "여기를 보라"는 표시 역할만 한다. 컴포넌트는 단단하고 확신 있게: 각진 모서리, 1px 선, 그림자 없음, hover에서는 빨간 선으로 분명하게 반응한다.

실제 스타일은 `index.html` 인라인 `<style>`에 있다. 루트의 `style.css`와 `script.js`는 이 페이지에 연결되지 않은 별도 자료이므로 디자인 근거로 쓰지 않는다.

**Key Characteristics:**
- 24px 점 격자 배경과 최대 1200px 폭의 좌우 세로선 프레임
- 카드 네 모서리의 십자 마커. hover 시 테두리와 함께 빨간색으로 바뀜
- 모노스페이스 대문자 라벨로 인덱스, 기간, 태그, 내비게이션 표시
- 모서리 0px, 그림자 없음, 1px 선으로만 구조 표현
- 강조색은 Signal Red 하나

## Colors

종이 위 연필 선 같은 무채색 팔레트에 신호용 빨강 한 가지를 쓴다.

### Primary
- **Signal Red** (`signal-red`): 주목 지점을 알리는 유일한 강조색. 주요 버튼 배경, 활성 탭 밑줄, 인덱스 숫자(`[01]`), 기간 표기, eyebrow 라벨, hover 시 테두리·십자 마커·링크.
- **Signal Red Deep** (`signal-red-deep`, CSS `--accent-text`): 빨간 **텍스트**와 흰 글자를 얹는 빨간 면(주요 버튼). 흰 바탕·Paper 위 4.5:1 이상.
- **Signal Red Strong** (`signal-red-strong`, CSS `--accent-strong`): 주요 버튼·nav CTA hover 배경.

### Neutral
- **Ink** (`ink`): 제목과 본문 텍스트, 외곽선 버튼 테두리, 토스트 배경.
- **Graphite** (`graphite`): 보조 설명, 내비게이션 기본 상태, 태그 텍스트, 캡션.
- **Paper** (`paper`): 페이지 바탕. 반투명(92%)으로 sticky 내비 배경에도 쓰임.
- **Sheet** (`sheet`): 카드, 스탯 셀, 인덱스 배지 등 종이 위에 올린 시트.
- **Grid Line** (`grid-line`): 점 격자, 프레임 세로선, 섹션 구분선, 카드·태그 테두리.
- **Crosshair** (`crosshair`): 십자 마커 기본색, eyebrow 앞 `//`, 리스트 대시(`—`).

### Named Rules
**The Readable Red Rule.** 밝은 Signal Red(#e5484d)는 선·테두리·십자 마커·밑줄·포커스 링 등 비텍스트 요소에만 쓴다. 글자색이나 흰 글자 뒤 배경에는 Signal Red Deep을 쓴다.

**The One Signal Rule.** 빨강은 하나만, 표시 용도로만 쓴다. 넓은 면에 칠하는 건 주요 버튼과 nav CTA hover뿐이다. 두 번째 강조색을 들이지 않는다.

**The Pencil Grey Rule.** 구조선은 모두 `grid-line` 한 단계로 통일한다. 선의 위계는 색 농도가 아니라 두께로 만든다 (기본 1px, 활성 탭 2px, 토스트 3px).

## Typography

**Display Font:** IBM Plex Sans (with Inter, sans-serif)
**Body Font:** IBM Plex Sans (with Inter, sans-serif)
**Label/Mono Font:** JetBrains Mono (with IBM Plex Mono, ui-monospace)

**Character:** 엔지니어링 문서 느낌의 산세리프에 코드 에디터 느낌의 모노를 짝지었다. 본문은 사람이, 라벨은 시스템이 쓴 것처럼 보인다.

IBM Plex Sans는 한글 글리프가 없어서, 한국어 본문과 제목은 시스템 산세리프(맑은 고딕, Apple SD Gothic Neo 등)로 렌더링된다. 한국어가 주 콘텐츠이므로 실제로 보이는 한글 서체는 OS에 따라 달라진다.

### Hierarchy
- **Display** (600, clamp 2.4–4.2rem, 1.08): 히어로 직함("게임 기획자 & PM") 전용.
- **Headline** (600, clamp 1.6–2.3rem, 1.15): 섹션 제목 (Document Hub, 최근/대표 이력, 최근 작업).
- **Title** (600, 1.15rem): 카드 제목, 문서 뷰어 제목.
- **Body** (400, 16px, 1.6): 본문. 히어로 소개는 1.05rem·56ch, 문서 설명은 0.9rem·60ch, 경력 리스트는 0.92rem·1.55.
- **Label** (500, 0.68–0.8rem, 0.02–0.04em, 대문자): eyebrow, 내비게이션, 버튼, 탭, 태그, 기간, 캡션, 스탯 라벨. 스탯 숫자는 같은 모노체로 1.6rem·600·Signal Red.

### Named Rules
**The Margin Note Rule.** 인덱스, 기간, 분류, 동작 이름처럼 시스템이 매기는 정보는 모노 대문자로 쓴다. 문장과 설명은 산세리프로 쓴다. 이 둘을 섞지 않는다.

## Layout

- **프레임:** 최대 1200px 중앙 컬럼. 좌우를 `grid-line` 1px 세로선으로 닫아 노트 한 장의 경계를 만든다. 안쪽 여백은 24px.
- **배경:** `body` 전체에 24px 간격의 1px 점 격자 (radial-gradient).
- **리듬:** 기본 단위 24px. 그리드 gap 24px, 카드 패딩 32px, 섹션 패딩 96px(작은 섹션 64px). 섹션 사이는 위쪽 1px 구분선.
- **그리드:** 히어로는 1.1fr / 0.9fr 2열. 경력·최근 작업은 1fr / 1fr 2열. 스탯은 1px 간격의 2열 셀 그리드.
- **반응형:** 1024px 이하에서 히어로 1열, 임베드 높이 축소. 768px 이하에서 경력·최근 그리드 1열, 내비는 CTA만 남김. 640px 이하에서 푸터 좌측 정렬, 임베드 400px.
- **Sticky 내비:** 높이 64px, 92% 불투명 Paper + 6px blur, 하단 1px 선.

## Elevation & Depth

평면 시스템이다. 깊이는 그림자가 아니라 "격자 종이 위에 올린 흰 시트"라는 색 차이(Paper → Sheet)와 1px 테두리로만 표현한다. 스크린샷 뷰어도 프레임 없이 격자 위에 바로 놓인다.

예외는 토스트 하나다. 화면 위에 잠깐 떠 있는 알림이라 약한 그림자(`0 4px 16px rgba(0,0,0,0.15)`)를 쓴다.

### Named Rules
**The Flat Sheet Rule.** 콘텐츠 표면에는 그림자를 쓰지 않는다. 레이어가 필요하면 Sheet 배경과 `grid-line` 테두리로 분리한다. 그림자는 일시적으로 떠 있는 요소(토스트)에만 허용한다.

## Shapes

모든 모서리는 직각(0px)이다. 둥근 모서리는 어디에도 없다. 형태 언어는 세 가지다.
- **1px 직선 테두리**: 카드, 태그, 버튼, 임베드 프레임.
- **십자 마커**: 카드 각 모서리 바깥 6px 지점에 12×12px 십자. 제도 용지의 재단 표시처럼 시트의 위치를 알려준다.
- **텍스트 기호**: `//` (eyebrow 접두), `[01]` (인덱스 괄호), `—` (리스트 불릿), `↗ ↓` (외부 링크·다운로드).

## Components

### Buttons
단단하고 확신 있게. 높이 48px의 직각 블록에 모노 대문자 라벨을 넣는다.
- **Shape:** 직각 (0px), 1px 테두리.
- **Primary:** Signal Red Deep 배경 + 흰 텍스트, 좌우 28px. 페이지당 1–2개만 (예: "라이브 문서 열람하기").
- **Hover:** 배경이 Signal Red Strong으로 바뀜, 160ms ease-out.
- **Focus:** 모든 링크·버튼·탭에 2px Signal Red 외곽선, 2px 간격, 직각.
- **Outline:** 투명 배경 + Ink 테두리·텍스트. hover 시 테두리와 텍스트가 Signal Red로 바뀜. 문서 액션("PDF 다운로드 ↓", "구글 문서 원본 ↗")에 쓰며, 이때는 38px 높이·0.7rem의 compact 변형.
- **Group:** 버튼 간격 16px, 줄바꿈 허용.

### Chips (Tags)
- **Style:** 투명 배경, `grid-line` 1px 테두리, Graphite 모노 대문자 0.68rem, 패딩 5px 10px, 간격 8px.
- **State:** hover 시 테두리·텍스트가 Signal Red로 바뀜. 선택 상태는 없음 (분류 표시 전용).

### Cards / Containers (Blueprint Card)
- **Corner Style:** 직각 + 네 모서리 십자 마커.
- **Background:** Sheet.
- **Shadow Strategy:** 없음 (Flat Sheet Rule).
- **Border:** `grid-line` 1px. hover 시 테두리와 십자 마커가 함께 Signal Red로 바뀜 (160ms).
- **Internal Padding:** 32px.
- 카드 안 미디어(16:9)는 hover 시 1.02배 확대 (300ms).

### Navigation
- **Style:** 왼쪽에 모노 로고 `KWACK_SEONGEUN.` (마침표만 Signal Red), 오른쪽에 `[01] INTRO` 형식의 모노 대문자 0.72rem 링크(간격 28px).
- **States:** 기본 Graphite, hover Signal Red. CTA("EMAIL ✉")는 Ink 1px 테두리 박스이고, hover 시 Signal Red로 채워지며 텍스트는 흰색.
- **Mobile (≤768px):** 섹션 링크를 숨기고 CTA만 남긴다.

### Document Tabs
- **Style:** 모노 대문자 0.72rem 텍스트 탭, 배경 없음. 탭 바 아래 `grid-line` 1px. 인덱스 `[01]`은 Signal Red.
- **States:** 기본 Graphite, hover Ink, 활성 Ink + Signal Red 2px 밑줄.
- 탭 아래에는 제목/설명/액션 헤더와 임베드 프레임(1px 테두리, 640 → 480 → 400px)이 온다.

### Screenshot Viewer (Signature)
프레임 없이 격자 위에 바로 놓인 자동 슬라이드쇼. 11장을 장당 5초씩 크로스페이드하며(55초 주기) hover 시 멈춘다. 왼쪽 위에 모노 인덱스 배지(Sheet 배경 + 1px 테두리), 아래에 `[07] 캡션` 형식의 모노 캡션이 붙는다. reduced-motion에서는 첫 장만 고정해서 보여준다.

### Career Entry
모노 Signal Red 기간(`2024.12 — 2026.04`) → Title 회사명 → Graphite 역할 → `—` 불릿 리스트 → 태그 그룹. 리스트 항목의 세부 설명은 `//` 접두로 한 줄 내려 쓴다.

### Toast
화면 오른쪽 아래 24px. Ink 배경, 흰 모노 0.78rem, 왼쪽에 3px Signal Red 띠. 아래에서 12px 올라오며 200ms에 나타난다.

## Do's and Don'ts

### Do:
- **Do** 새 섹션은 `// EYEBROW` → Headline → Graphite 설명 순서로 시작하고, 섹션 사이에는 1px `grid-line` 구분선과 96px 여백을 둔다.
- **Do** 모든 인덱스와 순번을 `[01]` 모노 형식으로 쓰고, 숫자는 Signal Red로 칠한다.
- **Do** 새 카드는 Blueprint Card(Sheet 배경, 1px 테두리, 십자 마커 4개, 32px 패딩)로 만들고 hover 반응을 똑같이 맞춘다.
- **Do** 모든 상태 전환은 160ms ease-out으로 맞춘다 (등장 효과 320ms, 토스트 200ms).
- **Do** 외부 링크에는 `↗`, 다운로드에는 `↓` 기호를 라벨 끝에 붙인다.
- **Do** 새 모션에는 `prefers-reduced-motion` 대응을 함께 넣는다.

### Don't:
- **Don't** 모서리를 둥글게 만들지 않는다. 모든 표면과 컨트롤은 0px이다.
- **Don't** 콘텐츠 카드나 버튼에 그림자를 넣지 않는다.
- **Don't** Signal Red 외에 두 번째 강조색이나 그라데이션을 들이지 않는다.
- **Don't** 설명 문장을 모노체로, 인덱스·라벨을 산세리프로 쓰지 않는다 (Margin Note Rule).
- **Don't** 연결되지 않은 `style.css`의 값(검정·흰색 반전 변수, `#a40000` 계열)을 이 시스템의 토큰으로 가져오지 않는다.
