#프로젝트 컨벤션 (Project Conventions)

##기술 스택 (Tech Stack)

- 프레임워크: Astro
- 스타일링: Tailwind CSS
- UI 컴포넌트: HTML/Astro 컴포넌트 (복잡한 클라이언트 측 상태 관리가 필요한 경우에만 React/Preact 사용)
- 배포: Vercel

##스타일링 및 디자인 시스템 (Tailwind)

- Cursor 작업 지침: 즉시 브랜드 색상이 반영되도록 Tailwind 설정과 CSS 변수를 업데이트하십시오. 이때 대비 수치가 웹 접근성 표준을 충족하는지 확인하십시오.

##컴포넌트 구조 (Component Structure)

- Astro의 컴포넌트 구조(src/components/)를 따릅니다.
- AstroWind 기본값에서 크게 벗어나는 커스텀 UI 또는 Human-tec 전용 컴포넌트에는 명확한 접두사를 붙여 구분하십시오.
- 컴포넌트는 모듈식으로 유지하십시오 (예: HeaderLogo, HeaderLinks, LanguageSelector, LoginButton 등으로 분리).

##요청된 구조적 변경 사항 (우선순위) 1.**공지 바 (Announcement Bar)**: 베이스 레이아웃에서 <Announcement /> 컴포넌트를 완전히 제거하십시오.2.2.**언어 드롭다운 (Language Dropdown)**: 헤더의 RSS/Wi-Fi 아이콘을 드롭다운 컴포넌트로 교체하십시오. [ 한국어, English, 日本語 ]를 지원해야 합니다. 3.**로그인/관리자 버튼**: 헤더에 있는 기존 AstroWind의 'Download' CTA 버튼을 'Login' 버튼으로 교체하십시오.

##콘텐츠 마이그레이션 (Human-tec)
**(매우 중요) 위의 AstroWind 템플릿은 이미 본 프로젝트 폴더에 이식 완료 된 상태**

- 가능한 경우 제품, 서비스, 뉴스 등의 콘텐츠는 Astro의 콘텐츠 컬렉션(src/content/)을 통해 관리하십시오.
- 페이지 코딩을 시작하기 전, 기존 Human-tec의 주요 카테고리를 새로운 AstroWind 내비게이션 구조에 맞게 매핑하십시오.
