# react_practice

TMDB API를 사용해 인기 영화를 불러오는 간단한 React + Vite 연습 프로젝트입니다.

현재 구현된 범위는 기본 영화 목록 조회와 검색창 UI까지입니다. 검색 입력값 상태는 연결되어 있지만, 실제 검색 API 호출 로직은 아직 붙어 있지 않습니다.

## Stack

- React 19
- Vite
- Tailwind CSS 4
- ESLint
- TMDB API

## Features

- TMDB 인기 영화 목록 조회
- 로딩 상태 표시
- 에러 메시지 처리
- 반응형 UI 레이아웃
- 검색 입력 UI

## Project Structure

```bash
.
|-- public/
|-- src/
|   |-- components/
|   |-- App.jsx
|   |-- App.css
|   |-- index.css
|   `-- main.jsx
|-- .env.example
|-- .gitignore
|-- package.json
`-- vite.config.js
```

## Getting Started

### 1. Install

```bash
npm install
```

### 2. Set environment variables

`.env.example`을 참고해서 `.env` 파일을 채운 뒤 실행합니다.

```env
VITE_TMDB_API_KEY=your_tmdb_read_access_token
```

주의:

- 이 값은 TMDB v3 API Key가 아니라 `TMDB Read Access Token` Bearer 토큰 기준입니다.
- `.env`는 로컬 전용 파일이고 Git에는 포함되지 않습니다.

### 3. Run locally

```bash
npm run dev
```

브라우저에서 기본 개발 서버 주소를 열면 됩니다.

## Scripts

```bash
npm run dev
npm run build
npm run preview
npm run lint
```

## Notes

- 현재 영화 카드는 제목만 렌더링합니다.
- 검색창은 UI만 준비되어 있고 실제 검색 기능은 미구현 상태입니다.
- TMDB 토큰이 없거나 잘못되면 영화 목록을 불러오지 못합니다.
