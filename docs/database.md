# Data Model — +FACTURAS

This document presents the **conceptual data domains** used by the platform. It does not expose the client's production schema or database contents.

## Main domains

- **Company** — business account / organization using the platform.
- **User** — authenticated person with an assigned role.
- **Customer** — commercial customer associated with invoices or transactions.
- **Product / Service** — billable catalogue item.
- **Invoice** — commercial document issued to a customer.
- **Invoice Item** — line item belonging to an invoice.
- **Payment** — payment record associated with commercial activity.
- **POS / PDV** — point-of-sale configuration or operational point.
- **Operator Session** — operational POS session where applicable.
- **Report Domain** — aggregated or filtered operational data used by dashboards and reports.

## Conceptual relationships

```text
Company 1 --- * User
Company 1 --- * Customer
Company 1 --- * Product / Service
Company 1 --- * Invoice

Customer 1 --- * Invoice
Invoice  1 --- * Invoice Item
Invoice  1 --- * Payment

Company 1 --- * POS / PDV
POS / PDV 1 --- * Operator Session
```

## Database technology

The platform uses **PostgreSQL** as its relational database. This supports strong data relationships, reporting queries and transactional consistency for business workflows.

## Privacy boundary

The following are intentionally not published:

- Exact production tables or migration files
- Client / customer records
- Invoice data from real businesses
- Database credentials
- Private payment information
- Production backup files
