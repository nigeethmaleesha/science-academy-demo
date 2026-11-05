# Pradeep Science Academy — Student Platform Demo

An interactive student-facing frontend demonstration for Grades 6–11 Science tuition. This is not a working production payment, login or content access system.

## What's included

- Home page with custom brand, AI-generated variations based on the supplied tutor photos
- 14 class combinations: Grades 6–9 Theory/Paper; Grades 10–11 Theory/Paper/Revision
- Grade filtering, class search and class detail/material previews
- Free/paid demo lesson library and unlock/payment navigation
- Three sample five-question Science MCQ exams with ten-minute timer, grading and answer review
- Demo student login, dashboard and payment history
- Bank-slip form demonstration: only filename and a pending entry are saved to browser localStorage; the file is NOT uploaded to a server
- Online gateway disabled until real integrations are available

## Run locally

Open `index.html` directly in a browser, or run a local static web server from this folder:

```bash
npx serve .
```

## Deploy to Vercel

1. Put the contents of this folder (not the enclosing ZIP) in a GitHub repository.
2. On Vercel, choose Add New → Project → Import that Git repository.
3. Framework Preset: Other (static HTML/CSS/JS). Root Directory: repository root.
4. Build Command: blank; Output Directory: blank/default.
5. Deploy. Vercel will provide a `*.vercel.app` URL.

The site uses hash routes (`#/classes`, `#/exams`) so static Vercel hosting works without routing rewrites.

## Important

- This is an interactive design prototype. Sample prices, lesson titles, examination questions and payment statuses are demonstration content only. Confirm all fees and details with the tutor before launch.
- Do not upload real payment slips or enter actual banking information into this prototype.
- Actual secure login, payment verification, student/parent accounts, teacher uploads, access control and video protection require the backend phase.
- AI images should be checked and approved by the tutor before public marketing use.

## Recommended full-stack evolution

Next.js + TypeScript, PostgreSQL + Prisma, object storage for resources, verified payment gateway with webhooks, private video streaming with signed playback tokens, and server-side role-based access controls. The demo's data can be migrated into real database models.
