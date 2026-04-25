# Project Instructions

## Product

This repo is for a Malaysian F&B shift marketplace app. Businesses post short shifts, and workers book suitable shifts. The app serves three core roles:

- Worker
- Business
- Admin

## Development Stack

- Use Expo, React Native, and TypeScript.
- Prefer Supabase for authentication, database, storage, and row-level security.
- Keep implementation mobile-first.
- Use simple, conventional app architecture unless a requested phase clearly needs more structure.

## Scope Discipline

- Build one phase at a time.
- Do not continue beyond the requested phase.
- Do not overbuild.
- Do not add a payment gateway until the payment phase.
- Do not add AI matching until the smart matching phase.
- If a requested change implies future-phase work, document the dependency and keep the current implementation within scope.

## Product Principles

- Keep the app clean, simple, mobile-first, and not congested.
- Core actions should take 3 taps or less where possible.
- Prioritize clarity over density.
- Optimize for real F&B shift workflows in Malaysia, including short-notice availability, business trust, worker reliability, and admin oversight.
- Make role boundaries explicit in UI, data access, and backend policies.

## Engineering Rules

- Use TypeScript types for domain models, API payloads, and screen props.
- Keep business rules close to the domain logic, not scattered through UI components.
- Use Supabase RLS for authorization, not just client-side checks.
- Avoid introducing new infrastructure unless the current phase needs it.
- Prefer boring, reliable implementation choices over clever abstractions.
- Add tests or focused verification for changes that affect booking, role access, shift state, or security.

## Review Expectations

Before considering work complete, check the reviewer checklist in `docs/reviewer-checklist.md` and confirm the phase stayed within scope.
