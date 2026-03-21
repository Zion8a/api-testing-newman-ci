![API Smoke](https://github.com/Zion8a/api-testing-newman-ci/actions/workflows/api-smoke.yml/badge.svg)

# API Smoke Tests (Postman + Newman + GitHub Actions)

This repo demonstrates how I design and automate API smoke tests using Postman, run them locally with Newman, and execute them in CI with GitHub Actions including test reports as artifacts.

## What this repo demonstrates
- API smoke suite versioned in Git (Postman Collection v2.1 JSON)
- Environment-driven configuration (`baseUrl`, dynamic `bookingId`)
- Newman CLI execution with reports (HTML + JUnit XML)
- GitHub Actions CI that uploads reports as artifacts (`newman-reports`)

## Tech
- Postman Collection (v2.1)
- Newman (CLI)
- GitHub Actions (CI)
- Reporters: htmlextra (HTML), junitfull (JUnit XML)

## Run locally
```bash
npm ci
npm run api:smoke