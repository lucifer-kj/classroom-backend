# Classroom Backend

[![CodeRabbit Pull Request Reviews](https://img.shields.io/coderabbit/prs/github/lucifer-kj/classroom-backend?utm_source=oss&utm_medium=github&utm_campaign=lucifer-kj%2Fclassroom-backend&labelColor=171717&color=FF570A&link=https%3A%2F%2Fcoderabbit.ai&label=CodeRabbit+Reviews)](https://coderabbit.ai)

Backend service for the Classroom management system, built with TypeScript, Node.js, Express, Neon Postgres, and Drizzle ORM.

## Tech Stack

- **Runtime & Language**: Node.js, TypeScript
- **Framework**: Express
- **Database**: Neon Serverless PostgreSQL
- **ORM & Migrations**: Drizzle ORM, Drizzle Kit
- **Package Manager**: pnpm

## Getting Started

### Prerequisites

- Node.js (v20+ recommended)
- [pnpm](https://pnpm.io/) (`corepack enable pnpm`)

### Setup

1. **Install dependencies:**
   ```bash
   pnpm install
   ```

2. **Environment Variables:**
   Copy `.env.example` or update `.env` with your Neon connection string:
   ```env
   DATABASE_URL="postgresql://[user]:[password]@[neon_hostname]/[dbname]?sslmode=require&channel_binding=require"
   ```

3. **Database Migrations:**
   ```bash
   pnpm run db:generate   # Generate SQL migrations from schema
   pnpm run db:migrate    # Apply migrations to database
   ```

4. **Run Development Server:**
   ```bash
   pnpm run dev
   ```
