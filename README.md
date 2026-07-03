# Woovet Online Pet Hospital Platform — Case Study

> **Note:** This is a case study describing my role and contributions on a commercial product built for an employer (Harns Technology Pvt. Ltd.). Proprietary source code and client business data are not included — this repo documents architecture, decisions, and outcomes only.

## Overview

Woovet is a multi-clinic online pet hospital platform serving international veterinary clinics — appointment/records management, payments, and business dashboards for clinic staff and leadership.

**My role:** Software Development Engineer-II (Sep 2022 – Jan 2025), frontend/full-stack contributor and later frontend owner for the platform and its companion dashboards.

## Scale

| Metric | Detail |
|---|---|
| Routes mapped | 500+ |
| APIs integrated | 3,000+ |
| Clinics supported | Multiple, international |
| Payment gateways | Telr, Clover Connect (multi-regional) |
| Companion apps | Admin Dashboard, CEO Dashboard, React Native eCommerce app (Dubai-based client) |

## Tech Stack

React.js, Redux, TanStack Query (React Query), D3.js, Chart.js, Node.js, Express.js, MongoDB, React Native.

## What I Built

**Core platform** — Built and maintained the majority of the clinic-facing web application: routing architecture for 500+ distinct views, integration layer for 3,000+ backend APIs across appointment, records, billing, and inventory domains, and multilingual support for global clinic staff.

**Payments** — Integrated Telr and Clover Connect gateways to support secure, multi-regional transactions across the clinics served by the platform.

**Admin & CEO dashboards** — Designed and implemented two dashboards from requirements gathering through delivery: an operations dashboard for clinic admins and a metrics dashboard for leadership, using D3.js and Chart.js for dynamic, graph-based visualizations tailored to each audience's decision-making needs.

**Mobile (separate engagement)** — Led end-to-end development of a React Native eCommerce app for a Dubai-based client: translated Figma designs into mobile UI, implemented client- and server-side caching (Redux + TanStack Query) to cut load times, integrated Google Analytics, the Tamara payment gateway, and Android push notifications, and built pagination/caching for a catalog of thousands of products.

## Engineering Decisions

- **Caching strategy** — Combined Redux for client state with TanStack Query for server-state caching, reducing redundant API calls and improving perceived load time on data-heavy screens (dashboards, product catalogs).
- **Dashboard architecture** — Kept visualization logic (D3.js/Chart.js) decoupled from data-fetching so the same chart components could be reused across the Admin and CEO dashboards with different data shapes and access levels.
- **API integration at scale** — With 3,000+ APIs across the platform, structured the integration layer around consistent request/response contracts to keep 500+ routes maintainable by a small team.

## Outcome

Delivered 4 high-impact projects (platform, both dashboards, mobile app) within 2.5 years, supporting multiple international clinics in production with multilingual accessibility.

---
*For confidentiality, this write-up omits proprietary code, internal APIs, and client-identifying business data. Happy to discuss architecture and decisions in more depth in an interview.*
