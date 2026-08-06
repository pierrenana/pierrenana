## Pierre Nana

**I design and build mobile applications for iOS and Android — from the idea to the app being downloadable on the App Store and Google Play.**

The whole thing, by one person: the app itself, the API and database it runs on, the deployment pipeline, and the store submissions — signing, certificates, review. A lot of React Native work stops at the build. Mine stops when it runs on someone's phone.

Freelance developer, based in Marseille, France. Fully remote. I work in French and English.

---

## Kelenz — my own product, live on both stores

A social network for athletes. LinkedIn ignores performance, Instagram ignores the record — Kelenz puts both in one profile: sport, positions, season stats, trophies, club history, with a full social layer on top.

I'm a competitive athlete myself, and I had nowhere to exist online as one. I built what was missing, on iOS, Android and the web.

[App Store](https://apps.apple.com/us/app/kelenz/id6758309487) · [Google Play](https://play.google.com/store/apps/details?id=com.kelenz.app) · [kelenz.com](https://kelenz.com)

Product design, architecture and development — three platforms, one person, three separately deployed repositories behind a single API.

| | |
|---|---|
| **Mobile** — iOS + Android | React Native, Expo SDK 56, expo-router, TanStack Query, Zustand, i18next |
| **Web** — public pages, shareable profiles, admin back-office | Next.js 15 (App Router), React 19, Tailwind v4, next-intl |
| **API** — business logic, real time, media | NestJS 11, PostgreSQL (Neon), Drizzle ORM, native WebSocket |

Verified in the codebase, not estimated:

- ~100,000 lines of strict TypeScript · ~1,900 commits · 188 test files (unit, integration, end-to-end against a real database)
- 29 controllers · ~100 API endpoints · 35 tables · 25 hand-written SQL migrations · 70 mobile routes
- 83 sports · 3 profile types · FR/EN everywhere, down to push notifications and transactional emails

### Three things worth naming

**A full backend migration, with no downtime.** From a serverless architecture (Supabase Edge Functions, Deno, ~70 functions) to a NestJS monolith on Postgres — while mobile and web clients stayed in production the whole way. What I was after: end-to-end typing, real integration tests, an explicit domain, and a predictable bill.

**Removing a product, not only adding to one.** Kelenz shipped with a B2B vertical for clubs — dashboard, teams, matches, Stripe subscriptions. Pivoting to consumer meant taking all of it out: schema, endpoints, screens, translations, with no regression on what stayed. Deleting code is the part nobody practises.

**Real time that degrades properly.** An authenticated WebSocket gateway feeds messaging and notifications while the app is in the foreground; Expo push takes over in the background. Reconnecting invalidates the cache rather than replaying events — simple, and hard to get wrong.

---

## What I work with

**Mobile** — React Native, Expo, expo-router, TypeScript (strict, everywhere)
**API** — NestJS, Node.js, PostgreSQL, Drizzle ORM, WebSocket, REST
**Shipping** — App Store and Google Play submissions, signing, certificates, review, CI/CD
**Infrastructure** — Railway, Neon, Cloudflare R2, GitHub Actions, Sentry, PostHog

I write React Native, and I go down into native when a project calls for it — a native module, an Xcode or Gradle build that won't cooperate, an SDK with no JS binding. If you need genuinely native Swift or Kotlin work, I'll tell you so rather than sell you cross-platform.

---

## Why there's no public code here

Kelenz is my product, and client work belongs to my clients. So there are no repositories to browse on this profile — the two store listings above are the artifact. I'd rather say that plainly than open three empty repos.

---

## Working together

Building an app from scratch, taking over an existing one, or getting a React Native project all the way through release.

- Fully remote, France and international
- French and English, meetings included
- Epitech Grande École programme, MSc, 2020–2025 · 4 years of professional experience

[Malt](https://www.malt.fr/profile/pierrenana) · [LinkedIn](https://www.linkedin.com/in/pierrenana/)
