# vibereview-web

VibeReview 메인 대시보드 웹앱. 팀 분석, 개인 통계, 데일리 스크럼, API 키 관리 등 핵심 사용자 인터페이스.

## Tech Stack

- **Framework:** Next.js 15 + Turbopack + React 19
- **Styling:** Tailwind CSS v3 + Radix UI
- **State:** Zustand + TanStack Query
- **Charts:** Recharts
- **Animation:** Framer Motion
- **Auth:** Supabase Auth (SSR + Auth Helpers)

## Getting Started

```bash
# 의존성 설치
pnpm install

# 환경 변수 설정
cp .env.example .env.local
# NEXT_PUBLIC_SUPABASE_URL, NEXT_PUBLIC_SUPABASE_ANON_KEY 등 입력

# 개발 서버 실행 (Turbopack)
pnpm dev
```

## Scripts

| Command | Description |
|---|---|
| `pnpm dev` | 개발 서버 (Turbopack, localhost:3000) |
| `pnpm build` | 프로덕션 빌드 |
| `pnpm start` | 프로덕션 실행 |
| `pnpm lint` | ESLint 검사 |

## Routes

| Route | Description |
|---|---|
| `/dashboard` | 팀 분석 대시보드 |
| `/my-dashboard` | 개인 통계 |
| `/team` | 팀 관리 |
| `/daily-scrum` | 데일리 스크럼 |
| `/api-keys` | API 키 관리 |
| `/settings` | 사용자/팀 설정 |
| `/getting-started` | 온보딩 가이드 |
| `/guest` | 게스트 접근 (비인증) |

## Environment Variables

```env
NEXT_PUBLIC_SUPABASE_URL=https://your-project.supabase.co
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-anon-key
NEXT_PUBLIC_API_BASE_URL=http://localhost:3001
```

## Related Projects

- [vibereview-api](https://github.com/ijg0341/vibereview-api) - REST API
- [vibereview-uploader](https://github.com/ijg0341/vibereview-uploader) - CLI 업로더
