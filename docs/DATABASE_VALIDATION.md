# Database validation plan — SifoLending

Status: schema draft only; not applied to any database.

## Required before production
- Apply migrations to a disposable Supabase/PostgreSQL project first.
- Verify two-company isolation for borrowers, applications, loans, and transactions.
- Add company/branch ownership checks for all related records.
- Test repayment allocation across principal, interest, fees, and penalties; loan principal is not revenue.
- Ensure loan disbursement/repayment are atomic, idempotent, and ledger-backed.
- Verify role separation between application, assessment, approval, disbursement, and collection.
- Confirm audit events are append-only and capture actor, action, and record identity.
- Review RLS policy recursion, SECURITY DEFINER function ownership/search_path, and privilege grants.
- Add automated SQL migration tests before marking this PR ready.
