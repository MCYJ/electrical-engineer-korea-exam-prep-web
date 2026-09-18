# 전기기사 필기·실기 문제풀이 marketing site context

## Identity and scope

- Service ID: `KOR-0029`
- Android package / iOS bundle: `app.mcyj.examprep.kor0029`
- Public repository: `MCYJ/electrical-engineer-korea-exam-prep-web`
- Production URL: `https://mcyj.github.io/electrical-engineer-korea-exam-prep-web/ko/`
- Scope is a public app-only marketing and useful exam-study site. The source service directory is read-only.

## Store state verified 2026-09-18

- Google Play exact package page returned HTTP 200.
- Apple public lookup returned one exact bundle match, track ID `6797294663`, version `1.0.1`, with a public App Store URL.
- Both Store badges are active only for those exact verified destinations.

## Official facts and boundaries

- Q-Net item code `1150`; qualification name `전기기사`; administering body 한국산업인력공단.
- Written: five subjects, 20 multiple-choice items and 30 minutes per subject, 100 items and 150 minutes total.
- Practical: Electrical Facility Design and Management, written-response type, 150 minutes.
- Passing: every written subject at least 40 and written average at least 60; practical at least 60.
- Current listed fees at verification: written KRW 19,400 and practical KRW 22,600. The site avoids checkout-sensitive price promises and directs candidates to Q-Net before payment.
- Q-Net instructs candidates to prepare with the latest Electrical Equipment Technical Standards and KEC announced before the exam date.
- Eligibility varies by education, prior qualification and experience; Q-Net self-check and document review control the individual decision.
- A written pass provides a two-year written-stage exemption from the announcement date.

## Product and design

- Korean primary locale with a useful English explanation for international readers; the Korean exam itself is not represented as English-delivered.
- Ten substantive guides per locale plus FAQ, privacy, terms, support and contact.
- Bright apricot and amber circuit-schematic visual system derived from the app's `soft_apricot` design family.
- Global typography uses `word-break: keep-all` and `overflow-wrap: break-word`; only long source/contact links use `overflow-wrap: anywhere`.
- Product claims are limited to the public listing: 500 independently authored questions, five mock exams, detailed explanations, on-device progress and no required RushLabs account.

## Build and QA

- `npm run build` generates static pages with canonical, hreflang, Open Graph, JSON-LD, sitemap, robots and a custom 404.
- `npm run check` verifies internal routes, metadata, output count, global keep-all, both exact Store identities and absence of stale Coming soon labels.
- GitHub Actions publishes `dist/` to GitHub Pages.

## Work log

- 2026-09-18: Created the bilingual site with current Q-Net facts and the apricot circuit-schematic visual direction. Production deployment evidence will be appended after publication.
