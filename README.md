# react_practice

TMDB API를 사용해서 영화 데이터를 보여주는 **React + Vite 연습 프로젝트**입니다.

## Stack

- React (Functional Components + Hooks)
- Vite (빌드 툴)
- Tailwind CSS
- ESLint
- TMDB API

## Features

현재 구현된 기능:

- 인기 영화 목록 불러오기
- 로딩 스피너 표시
- 검색 입력 UI
- 검색 결과 표시
- 검색어 기반 영화 결과 업데이트
- 검색어 카운트 저장 (Appwrite 연동 기능)
- 인기 검색어 기반 트렌딩 영화 표시

## Project Structure

```
.
|-- public/
|-- src/
|   |-- components/
|   |   |-- Search.jsx
|   |   |-- Spinner.jsx
|   |   `-- MovieCard.jsx
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

### 1. 설치

```
npm install
```

### 2. 환경 변수 설정

`.env.example` 파일을 참고해서 `.env` 파일을 루트에 생성하고, 아래 값을 채웁니다:

```
VITE_TMDB_API_KEY=your_tmdb_read_access_token
```

⚠️ 주의:

- 이 값은 **TMDB Read Access Token (Bearer token)** 입니다.
- `.env`는 로컬 전용 파일이며 **Git에 커밋하지 않습니다**.

### 3. 실행

```
npm run dev
```

브라우저에서 기본 개발 서버 주소(`localhost:5173` 등)를 열어 앱을 확인합니다.

## Scripts

```
npm run dev      # 개발 서버 실행
npm run build    # 프로덕션 빌드
npm run preview  # 프로덕션 빌드 미리보기
npm run lint     # 코드 린트
```

## Notes

- `MovieCard` 컴포넌트는 영화 제목, 평점, 언어, 개봉연도 등을 표시합니다.
- API 호출 실패 시 에러 메시지를 표시합니다.
- 검색 결과가 없거나 에러가 발생하면 사용자에게 안내 텍스트가 표시됩니다.

## Source

- This code is based on the following references:
  - Video: https://www.youtube.com/watch?v=dCLhUialKPQ
  - Repository: https://github.com/adrianhajdin/react-movies
