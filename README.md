# FixedFunding

> A student-funding and accommodation administration platform concept focused on reconciling allowances, supporting evidence and payment workflows.

## Problem

Student funding workflows can become difficult to audit when accommodation records, invoices, allowances and supporting evidence live across disconnected processes. FixedFunding explores a software workflow for making those records easier to track and reconcile.

## What the application is

FixedFunding is a React + TypeScript application with a Vite build pipeline. The codebase contains application screens, seeded demonstration data and deployment configuration for Netlify. The repository is structured as an application rather than a static mock-up, with domain-oriented UI flows and data handling in the `app/` project.

## Technology

- React 19
- TypeScript
- Vite
- React Router
- Tailwind CSS
- Radix UI components
- React Hook Form + Zod
- Recharts
- Firebase integration
- Netlify deployment configuration

## Architecture at a glance

```text
User
 │
 ▼
React application
 ├── routed screens
 ├── reusable UI components
 ├── forms + validation
 ├── charts / reporting
 └── application data + service integrations
        │
        ├── Firebase
        └── Netlify deployment
```

The project also includes `generateSeed.js` for generating demonstration data and `netlify.toml` for deployment configuration.

## Repository structure

```text
.
├── app/              # React + TypeScript application
├── generateSeed.js   # demonstration-data generation
├── netlify.toml      # Netlify configuration
└── package-lock.json
```

## Run locally

```bash
git clone https://github.com/Just4Skii/FixedFunding.git
cd FixedFunding/app
npm install
npm run dev
```

For a production build:

```bash
npm run build
npm run preview
```

Linting:

```bash
npm run lint
```

## Engineering focus

This project is useful as a portfolio example because it combines a business workflow with a modern typed frontend, form validation, routing, reporting visualisations and deployment configuration. The domain is intentionally grounded in a real administrative problem rather than a generic tutorial application.

## Portfolio note

This is a demonstration/project implementation. Any funding, payment or student data shown in the application should be treated as sample data rather than real financial records.
