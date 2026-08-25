# LeadRoute

> Outbound lead operations dashboard for verification, approvals, sequencing, and inbox workflows.

LeadRoute is a React + Vite + TypeScript frontend focused on prospect intake, approval review, sequence automation, and operational monitoring. The app is organized around a sidebar-driven dashboard, route-based screens, and product workflows for outbound lead operations.

![React](https://img.shields.io/badge/React-19.2.8-61DAFB?logo=react&logoColor=111)
![TypeScript](https://img.shields.io/badge/TypeScript-5.7.0-3178C6?logo=typescript&logoColor=fff)
![Vite](https://img.shields.io/badge/Vite-5.4.10-646CFF?logo=vite&logoColor=fff)
![MUI](https://img.shields.io/badge/MUI-5.14.20-007FFF?logo=material-ui&logoColor=fff)
![Redux Toolkit](https://img.shields.io/badge/Redux_Toolkit-2.2.7-764ABC?logo=redux&logoColor=fff)
![React Router](https://img.shields.io/badge/React_Router-6.20.0-CA4245?logo=reactrouter&logoColor=fff)
![ESLint](https://img.shields.io/badge/ESLint-9.39.5-4B32C3?logo=eslint&logoColor=fff)
![Prettier](https://img.shields.io/badge/Prettier-3.9.5-F7B93E?logo=prettier&logoColor=111)

---

## Overview

This project currently implements the frontend experience for LeadRoute, including shared navigation, dashboard metrics, verification queues, approvals, campaign management, message inbox flows, and settings screens. The UI uses demo data and a structured service/state layer so it can be connected to a backend later.

### Included product areas

- Dashboard and KPI cards
- Verification queue
- Approvals and audit trail
- Campaigns and templates
- Sequence builder and active sequences
- Connected inboxes and inbox hub
- Performance monitoring
- Settings screen

---

## Tech stack

| Area                 | Stack                               |
| -------------------- | ----------------------------------- |
| Frontend             | React 19                            |
| Language             | TypeScript                          |
| Build tool           | Vite                                |
| UI library           | MUI                                 |
| State management     | Redux Toolkit + React Redux         |
| Routing              | React Router DOM                    |
| Styling              | SCSS modules + MUI styling          |
| Visualization        | Recharts                            |
| Form validation      | React Hook Form + Zod               |
| API client           | Axios                               |
| Icons                | Lucide React                        |
| Testing              | Vitest, Testing Library, jsdom, MSW |
| Linting / formatting | ESLint + Prettier                   |

---

## Project structure

```text
leadroute/
├── public/
├── src/
│   ├── api/
│   │   ├── client/
│   │   ├── services/
│   │   ├── authSession.ts
│   │   ├── errorHandler.ts
│   │   └── apiResponse.ts
│   ├── components/
│   │   └── common/
│   ├── config/
│   ├── constants/
│   ├── features/
│   │   └── LeadRoute/
│   │       ├── data/
│   │       ├── screens/
│   │       ├── LeadRouteApp.tsx
│   │       ├── LeadRouteLayout.tsx
│   │       └── LeadRouteApp.module.scss
│   ├── hooks/
│   ├── providers/
│   ├── redux/
│   ├── routes/
│   ├── styles/
│   ├── types/
│   ├── utils/
│   ├── App.tsx
│   ├── main.tsx
│   └── setupTests.ts
├── env/
├── eslint.config.js
├── index.html
├── package.json
├── tsconfig.json
├── tsconfig.app.json
├── tsconfig.node.json
├── vite.config.ts
├── README.md
└── public/
```

### Main folders

- src/features/LeadRoute: app shell and screen implementations
- src/routes: app route configuration
- src/constants: nav and route constants
- src/api: client, services, and error handling
- src/components/common: reusable UI primitives
- src/redux: state slices, reducers, and store setup
- src/styles: theme and shared styling

---

## Screens and routes

Current screens in the app:

- Dashboard
- Verification Queue
- Approvals
- Audit Log
- Performance
- Campaigns
- Sequence Builder
- Templates
- Active Sequences
- Connected Inboxes
- Inbox Hub
- Settings

Routes are defined in src/routes/AppRoutes.tsx and default to the dashboard from the home page.

---

## Local setup

### Prerequisites

- Node.js 18+
- npm

### Install

```bash
npm install
```

### Run dev server

```bash
npm run dev
```

### Build production bundle

```bash
npm run build
```

### Preview build

```bash
npm run preview
```

---

## Available scripts

```bash
npm run dev
npm run dev:development
npm run dev:qa
npm run dev:production
npm run build
npm run build:development
npm run build:qa
npm run build:production
npm run preview
npm run lint
npm run typecheck
npm run test
npm run test:run
npm run test:coverage
npm run format
npm run format:check
```

---

## Project status

This is a frontend-focused prototype with:

- working app shell and layout
- route-based navigation
- MUI-driven screens and modal flows
- demo data for prospects, integrations, campaigns, and audit events
- Redux and API scaffolding for future backend integration

It is a product UI demo rather than a full backend-connected application.

---

## Notes

- The project name and app branding are aligned to LeadRoute.
- The codebase was previously carrying old PeopleFlow references in a few places, and those have been cleaned up.
- The app is still designed to be extended with real authentication, backend services, and persisted data flows.

---

## License

This project is currently unlicensed unless otherwise specified by your organization or team.
