# Hospital Appointment API

Prisma ORM & PostgreSQL implementation for Hospital Appointment API domain.

## Overview
- Introspected relational PostgreSQL schema using Prisma.
- Cleaned schema: PascalCase models (`Patient`, `Doctor`, `Appointment`), camelCase fields with `@map`, relation field naming, preserved `@db.Date` and `@db.Timestamp(6)`.
- Full CRUD operations implemented for `Patient`, `Doctor`, and `Appointment` models using `@prisma/adapter-pg`.
- Relational operations using `connect` and nested `include`.
- Database seeding with `prisma db seed` and end-to-end test verification script.

## Test Output
```
 ── Patients ──────────────────────────
Created: Test Patient 3
Found: Test Patient
Updated phone: 8888888888
Search results: 1

 ── Doctors ───────────────────────────
Created: Dr. Test 3
General Medicine doctors: 1

 ── Appointments ──────────────────────
Booked: 3 for Test Patient
Full fetch: Test Patient with Dr. Test
Doctor schedule: 1 appointment(s)
Status updated to: cancelled

 ── Cleanup ───────────────────────────
Test data cleaned up.
```
