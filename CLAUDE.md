# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 언어 및 커뮤니케이션 규칙
- **기본 응답 언어**: 한국어
- **코드 주석**: 한국어로 작성
- **커밋 메시지**: 한국어로 작성
- **문서화**: 한국어로 작성
- **변수명/함수명**: 영어 (코드 표준 준수)

## 프로젝트 개요

HTML, CSS, JavaScript, Tailwind CSS를 사용한 정적 개발자 웹 이력서 사이트. 빌드 도구 없이 CDN 기반으로 동작하는 단일 페이지 웹사이트.

## 기술 스택

- **HTML5** - 시맨틱 마크업
- **CSS3** - 커스텀 스타일 및 애니메이션
- **JavaScript (ES6+)** - 인터랙션 로직 (바닐라 JS)
- **Tailwind CSS (CDN)** - 유틸리티 기반 스타일링

## 개발 환경

별도의 빌드/번들링 과정 없음. `index.html`을 브라우저에서 직접 열거나 로컬 서버로 실행.

```bash
# 로컬 서버 실행 (Live Server 등)
npx serve .
```

## 코드 컨벤션

- Tailwind CSS 클래스를 우선 사용하고, 커스텀 CSS는 `css/style.css`에 최소한으로 작성
- JavaScript는 `js/main.js`에 작성하며 모듈 없이 단일 파일로 유지
- 반응형 디자인: 모바일 퍼스트 (Tailwind 기본 → `md:` → `lg:` 순서)
- 다크모드: Tailwind `dark:` 변형 클래스 활용
