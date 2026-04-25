# Product Rules

## Product Definition

The product is a Malaysian F&B shift marketplace app where businesses post short shifts and workers book suitable shifts.

## Core Roles

- Worker: Finds, reviews, books, and completes suitable F&B shifts.
- Business: Posts shifts, manages applicants or bookings, and tracks shift fulfillment.
- Admin: Oversees platform quality, user issues, disputes, and operational controls.

## Core Experience Principles

- The app must be clean, simple, mobile-first, and not congested.
- Core actions should take 3 taps or less where possible.
- Each screen should have one primary job.
- Prefer clear lists, filters, status labels, and direct actions over dense dashboards.
- Avoid adding secondary workflows unless they are required by the current phase.

## Marketplace Rules

- Workers should only see shifts that are relevant and bookable for their role and status.
- Businesses should only manage shifts they own.
- Admins may view and moderate platform-wide data when required by the phase.
- Shift status must be explicit and consistent, such as draft, open, booked, completed, cancelled, or disputed when those states are in scope.
- Booking rules must prevent double-booking and invalid state transitions.

## Malaysian F&B Context

- Design for short shifts, part-time work, and operational urgency.
- Use local-friendly assumptions for currency, date, time, location, and contact patterns.
- Keep language direct and easy to scan for busy workers and business operators.
- Do not assume payment, payroll, tax, or compliance features exist until those phases are requested.

## Phase Boundaries

- Build one phase at a time.
- Do not continue beyond the requested phase.
- Do not overbuild placeholder flows for future phases.
- Do not add payment gateway logic until the payment phase.
- Do not add AI matching until the smart matching phase.
- Future features may be noted in docs or TODOs only when they clarify a current decision.

## Success Criteria

A phase is successful when the requested user workflow works simply, role access is correct, data is reliable, and the implementation does not introduce future-phase features.
