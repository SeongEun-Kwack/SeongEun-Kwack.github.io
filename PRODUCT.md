# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

- **Primary:** 게임사 채용담당자와 리드 기획자. 게임 시스템·콘텐츠 기획 포지션 서류 검토 중에 들어온다. 짧은 시간 안에 지원자의 역량을 판단하고, 확신이 서면 기획서 원본을 직접 열어 품질을 확인한다.
- 부차적: PM/PO 관점의 검토자. OTT PM 경력은 운영·데이터·협업 역량의 근거로 읽힌다 (주 타깃은 아님).

## Product Purpose

곽성은(게임 기획자 & PM)의 개인 포트폴리오 허브. 경력 요약, 대표 이력, 기획서 원본 링크, 개인 프로토타입을 한곳에 모은다.

성공 기준:
1. **빠른 역량 파악**: 첫 화면에서 경력 축(게임 시스템·콘텐츠 기획 6년 + 라이브 운영 + PM)이 바로 읽힌다.
2. **기획서 원본 열람**: Document Hub에서 PDF·Google 문서·Figma 원본을 연다.
3. **이메일 연락**: 면접·제안 연락으로 이어진다.

## Positioning

"기획서 한 장에서 서비스 운영까지." 수집형 RPG 라이브 서비스(킹덤스토리)에서 경제/상점 밸런싱, 무한 PvE·PvP 설계, 유닛 밸런싱, 데이터 기반 이탈 보완을 직접 맡았고, 이후 OTT 플랫폼 PM으로 멀티 디바이스 런칭·인프라 비용 절감·정부 규제 대응을 주도했다. 기획 산출물과 운영 성과를 모두 원본으로 보여줄 수 있다는 점이 차별점이다.

## Operating Context

- 채용 서류 검토 흐름 안에서 열린다 (이력서·지원서 링크 → 사이트).
- 일부 문서는 외부 서비스(Google Docs/Slides, Figma)에 있고 로그인/권한 문제로 링크를 눌러야 원본 확인이 가능하다. 사이트는 미리보기 + 원본 링크 역할을 한다.
- 섹션 구성: INTRO(+스크린샷 뷰어) → PORTFOLIO VIEWER(Document Hub) → HIGHLIGHT(대표 이력) → RECENT(개인 작업) → 연락처.

## Capabilities and Constraints

- 현재 구현: GitHub Pages에 배포되는 정적 `index.html` / `style.css` / `script.js`. 빌드 도구·프레임워크 없음. (정적 유지 여부는 확정 제약으로 지정되지 않음, 변경 시 사용자 확인 필요.)
- 기능: 섞어서 보여주는 스크린샷 뷰어, Document Hub 탭(PDF 다운로드·외부 원본 링크), 이메일 복사 토스트.
- **한국어 우선**: 본문은 한국어. 영어는 라벨·섹션 태그 수준으로만.
- **성과 수치 유지**: 기존 수치만 사용하고 새 주장·수치를 추가하지 않는다.
- **역기획서 출처 표기**: 워프레임, 영화 '콘스탄틴' 등 타사 IP 기반 문서는 '(역) 역기획' / 팬 컨셉임을 명확히 표기한다.

## Brand Commitments

- 이름 표기: 곽성은 | Seongeun Kwack (로고 텍스트 `KWACK_SEONGEUN`).
- 직함: GAME PLANNER & PRODUCT OWNER / PROJECT MANAGER, 한국어로 "게임 기획자 & PM".
- 태그라인: "기획서 한 장에서 서비스 운영까지".
- 톤: 실행 중심, 간결, 사실 기반.

## Evidence on Hand

- `kwak_seongeun_resume.pdf`: 경력기술서 (소프트닉스, NT게임즈/위메이드커넥트, SJMNC 등 6년).
- `warframe_mod_system.pdf`, `warframe_mod_ui.pdf`: 워프레임 MOD 시스템 / Wireframe 역기획서 (Google 문서 원본 링크 있음).
- `KSE_concept_portfolio.pdf`: 보스 컨셉 기획서 (영화 '콘스탄틴' 테마, Figma 원본 링크 있음).
- `screenshots/shot-01~11`: 킹덤스토리(Unity2D), 러브레시피(Unity3D), OTT 기능(숏드·연령제한·자막), 한입만 줄래? 플레이 화면.
- `ue5_project.jpg` + YouTube: UE5(C++/Blueprint) FPS 프로토타입.
- `img_crosspuzzle.jpg`, `image_5edb7b.jpg`: 이전 작업 썸네일 (crosspuzzle 카드는 최근 커밋에서 제거됨).
- 확정 수치: AWS/ABR 최적화로 인프라 비용 68% 절감. 2025 영상물 자체등급분류 사업자 지정 (카카오·네이버와 함께 중소기업 최초 선정).
- 없음 (만들지 말 것): 추천사, 매출·DAU 등 미기재 지표, 수상 경력, 추가 고객사.

## Product Principles

1. **원본이 증거다.** 요약보다 기획서 원본으로 가는 경로가 짧고 분명해야 한다.
2. **게임 기획자가 먼저, PM은 확장.** 주 독자는 게임사이므로 게임 시스템·콘텐츠 기획 역량이 먼저 읽히고, PM 경력은 운영·데이터 역량의 근거로 받친다.
3. **30초 안에 판단 가능.** 경력 축, 대표 성과, 연락 수단이 스크롤 없이 혹은 최소 스크롤로 보인다.
4. **사실만 말한다.** 수치·주장은 기존 근거에 한정하고, 타사 IP는 출처를 밝힌다.
