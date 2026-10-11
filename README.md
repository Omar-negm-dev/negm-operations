# Negm Operations

A browser-based inventory operations prototype for a business with multiple company-owned warehouses and online/local sales channels.

## Run locally

Open `index.html` in a browser, or serve this directory with `python -m http.server 8000` and visit `http://localhost:8000`.

## Features

- Warehouse creation and deletion (deletion is blocked while stock remains assigned)
- Inventory by SKU, quantity, and warehouse
- Demonstration auto-assignment rules for Amazon versus local fulfilment
- Role-specific demo views for owner, online staff, and local staff
- Sales recording and a simple activity log
- Local browser persistence via `localStorage`

## Important limitations

**This is a reconstructed prototype, not an export of the previously deployed site.** Demo role selection is not authentication and can be bypassed. Do not enter real company or personal data. It has no server, secure accounts, Amazon Vendor Central API integration, audit-grade transaction storage, or multi-user synchronization. The Amazon channel is only an internal label. Before production use, add a backend, server-side role-based authorization, properly hashed credentials, durable database storage, transactional stock changes, audit logs, and official integration credentials secured on the server.

## Suggested next steps

1. Add backend API and relational database.
2. Introduce authentication and server-side authorization.
3. Implement reorder rules, inventory transfers, and warehouse allocation settings.
4. Build supported Amazon Vendor Central workflows with appropriate authorization and reconciliation.
5. Add automated tests and deployment configuration.