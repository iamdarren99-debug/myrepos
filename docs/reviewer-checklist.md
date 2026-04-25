# Reviewer Checklist

Use this checklist for every feature, fix, or phase review.

## Scope

- Did this phase stay within the requested scope?
- Did the implementation avoid future-phase work?
- Did it avoid adding payment gateway behavior before the payment phase?
- Did it avoid adding AI matching before the smart matching phase?
- Is any new abstraction justified by current needs?

## UX Simplicity

- Is the app clean, simple, mobile-first, and not congested?
- Can core actions be completed in 3 taps or less where possible?
- Is each screen focused on one primary job?
- Are labels, status messages, and calls to action easy to understand?
- Are empty, loading, success, and error states clear?

## Mobile-First Layout

- Does the layout work well on small mobile screens first?
- Are touch targets large enough and comfortably spaced?
- Is important information visible without crowding the screen?
- Does the UI avoid desktop-first density?
- Are forms short, grouped logically, and easy to complete on a phone?

## Role-Based Access

- Are Worker, Business, and Admin permissions clearly separated?
- Can workers only access worker-appropriate actions and data?
- Can businesses only manage their own shifts and business data?
- Can admins access moderation or oversight tools only where intended?
- Are role checks enforced on the backend, not only in the UI?

## Data Correctness

- Are shift, booking, user, and business records created and updated correctly?
- Are state transitions valid and consistent?
- Are double bookings, stale shift states, and race conditions handled where relevant?
- Are dates, times, locations, and Malaysian currency values represented consistently?
- Are required fields validated before data is saved?

## Security

- Are Supabase RLS policies used for protected data?
- Is sensitive data hidden from unauthorized roles?
- Are uploads, storage paths, and public/private access rules safe where relevant?
- Are client inputs validated before trusted operations?
- Are secrets kept out of the client and repo?

## Edge Cases

- What happens when a shift is cancelled, full, expired, or already booked?
- What happens when a user has no role, an incomplete profile, or a suspended account?
- What happens with slow network, offline behavior, or failed Supabase requests?
- Are duplicate taps, retries, and refreshes handled safely?
- Are empty lists and first-use states polished?

## Feature Creep

- Did the change introduce workflows not requested in the phase?
- Did it add settings, dashboards, analytics, payments, messaging, AI, or admin tooling without being asked?
- Are placeholders limited to what is necessary for navigation or current functionality?
- Could any added complexity be removed without hurting the requested phase?

## Final Review

- Does the implementation match `AGENTS.md`, `docs/product-rules.md`, and `docs/design-rules.md`?
- Has the reviewer checked the app as each affected role?
- Has the reviewer verified the main happy path and at least the most likely failure path?
- Are remaining risks, assumptions, or deferred features documented clearly?
