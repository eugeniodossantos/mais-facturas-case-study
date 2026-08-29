# +FACTURAS — Invoicing & POS Platform Case Study

Technical case study of a business invoicing and point-of-sale platform developed with **Next.js, TypeScript, Flask and PostgreSQL**.

> **Project type:** Third-party / client project.  
> **Role:** Full-Stack Developer.

## Project overview

+FACTURAS is a business-management solution focused on invoicing, point-of-sale operations, payments, reporting and administrative control. The system combines a modern web frontend with a backend API and relational database to support day-to-day commercial operations.

## Business problems addressed

- Centralize invoicing and commercial operations.
- Provide a structured point-of-sale workflow for operators.
- Improve visibility over payments and transactions.
- Give administrators operational and financial reporting tools.
- Separate administrative and operational responsibilities.
- Maintain business information in a structured relational data model.
- Support controlled growth from invoicing into broader commercial operations.

## Main capabilities

- Authentication and role-based areas
- Customer / company dashboards
- Invoicing workflows
- Point of Sale (POS / PDV)
- POS activation and operator workflows
- Session / operational controls
- Payment management
- Administrative payment review
- Reporting with date filters
- Business dashboards
- Company and user administration

## Technology stack

| Layer | Technology |
|---|---|
| Frontend | Next.js 16 + TypeScript |
| Backend / API | Flask |
| Database | PostgreSQL |
| Architecture | Web client + backend API + relational database |
| Version control | Git / GitHub |

## Architecture

```text
Users / Operators / Admin
          |
          v
 Next.js Web Application
          |
          v
      Flask API
          |
          v
     PostgreSQL
          |
  -------------------
  |        |        |
Invoices Payments  POS
Reports  Companies Users
```

See [`docs/architecture.md`](docs/architecture.md).

## Data model

This public case study documents only conceptual data domains. The production schema, migrations, credentials and client data are not published.

Conceptual domains include companies, users, customers, invoices, invoice items, products/services, payments, POS configuration, operator sessions and reporting data.

See [`docs/database.md`](docs/database.md).

## My role

I worked as the developer of the system, contributing across frontend, backend, database integration, business workflows, debugging, validation and the evolution of the administrative and POS modules.

## Development timeline

The platform has been developed iteratively in multiple functional phases. The exact commercial timeline is not publicly disclosed in this repository.

## Screenshots

Approved public/demo screenshots will be maintained in [`assets/screenshots/`](assets/screenshots/).

## Source code policy

This repository is a **portfolio case study only**. It does not contain the production source code, credentials, database dumps, real customer information or private business logic.

## Ownership

+FACTURAS is **not owned by the developer and is not presented as a Logos Sistemas S.U. product**. This repository documents development work performed by Eugénio Fernandes dos Santos for professional portfolio purposes. All client/project ownership rights remain with their respective owner(s).

---

**Developer:** Eugénio Fernandes dos Santos  
**GitHub:** https://github.com/eugeniodossantos
