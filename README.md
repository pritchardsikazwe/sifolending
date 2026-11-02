# SifoLending

Independent Sifonet application for Zambia. Currency: ZMW.

This initial repository foundation is demo-only. Production authentication, persistence, permissions, audit events, compliance workflows and deployment are not yet implemented.

## Planned modules

- Borrowers & KYC
- Loan Products
- Applications
- Credit Assessment
- Approvals
- Guarantors & Collateral
- Disbursements
- Repayments
- Arrears & Collections
- Restructuring
- Portfolio Reports
- Settings

## Security baseline

- Company and branch isolation enforced server-side.
- Role-based access and audit trails.
- Secrets remain server-side.
- No live financial records in demo state.
