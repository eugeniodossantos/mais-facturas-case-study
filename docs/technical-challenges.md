# Technical Challenges — +FACTURAS

## 1. Keeping frontend and backend contracts consistent

The platform combines a Next.js frontend with a Flask backend, so API contracts, authentication state and validation must remain aligned across two application layers.

**Approach:** keep business rules in the backend, use typed frontend integration where possible and validate production builds to catch interface mismatches early.

## 2. Point-of-sale operational flow

A POS interface must be faster and more focused than a general administration dashboard.

**Approach:** create a dedicated PDV experience with operator-oriented screens, activation controls and session-aware operational flows.

## 3. Role separation

Administrators, company users and POS operators do not need the same screens or permissions.

**Approach:** separate administrative and operational areas and apply role-aware access patterns across the application.

## 4. Reliable commercial data

Invoices, payments and POS activity require structured relationships and consistent reporting.

**Approach:** use PostgreSQL as the relational persistence layer and design reporting around the same authoritative commercial records.

## 5. Reporting across time periods

Business users need to compare activity across specific date ranges rather than rely only on static dashboard totals.

**Approach:** implement date-based filtering for reports and keep reporting queries aligned with business entities and permissions.

## 6. Iterative module growth

The system evolved through multiple functional phases, which can create regression risk when new modules affect existing flows.

**Approach:** validate each phase across frontend, backend and database boundaries, including type checking and production builds before moving to the next stage.
