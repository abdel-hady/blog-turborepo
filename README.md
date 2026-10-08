# Blog Turborepo

A Turborepo monorepo for a blog application built with Next.js on the frontend. The workspace currently contains a single app, `apps/front`, which provides a modern blog experience with authentication, post management, comments, likes, and a Tailwind-based UI.

## Overview

This project is structured as a Turbo workspace to make it easier to scale into multiple apps or packages over time while keeping a single shared root configuration. The current implementation focuses on the frontend experience for a blog platform and communicates with a backend GraphQL API running at `http://localhost:8000`.

## Features

- Next.js 15 App Router frontend
- Turborepo-based monorepo structure
- Tailwind CSS + reusable UI components
- User authentication flows
- Google OAuth sign-in flow
- Blog post creation, editing, and deletion
- Post listing and post detail pages
- Comments and likes on blog posts
- JWT-based session handling
- Type-safe forms with Zod validation
- GraphQL integration for backend data access

## Tech Stack

- Next.js 15
- React 19
- TypeScript
- Tailwind CSS
- TurboRepo
- Supabase JS client
- TanStack React Query
- shadcn-style UI primitives
- Zod
- jose (JWT handling)

## Repository Structure

```text
blog-turborepo/
├── apps/
│   └── front/
│       ├── public/
│       ├── src/
│       ├── .eslintrc.json
│       ├── .gitignore
│       ├── components.json
│       ├── next.config.ts
│       ├── package.json
│       ├── postcss.config.mjs
│       ├── tailwind.config.ts
│       └── tsconfig.json
├── .gitignore
├── package.json
├── turbo.json
├── package-lock.json
└── README.md
