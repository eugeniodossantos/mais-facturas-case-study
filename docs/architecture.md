# Architecture — +FACTURAS

## Overview

+FACTURAS uses a conventional multi-tier web architecture that separates the user interface, backend business logic and relational persistence layer.

```text
Browser
  |
  v
Next.js 16 + TypeScript
  |
  v
Flask Backend / API
  |
  v
PostgreSQL
```

## Application responsibilities

### Frontend — Next.js + TypeScript

- Authentication UI
- Dashboards
- Invoice flows
- POS / PDV interfaces
- Reports
- Administrative screens
- Payment-management interfaces

### Backend — Flask

- Authentication / authorization handling
- Business rules
- Invoice operations
- POS operations
- Payment workflows
- Administrative actions
- Reporting data
- Database access

### Database — PostgreSQL

The relational database persists commercial and operational data and supports structured relationships between companies, users, customers, invoices, payments and point-of-sale activity.

## Architectural priorities

- Clear separation between frontend and backend responsibilities.
- Centralized business rules in the backend.
- Relational consistency for invoicing and payments.
- Different operational areas for administrators and business users.
- Ability to evolve modules without exposing production implementation in the public portfolio.

## Security boundary

This repository intentionally excludes authentication secrets, production endpoints, database connection details, payment credentials and client data.
