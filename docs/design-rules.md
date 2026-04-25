# Design Rules

## Design Direction

The app must feel clean, simple, mobile-first, and not congested. It is an operational marketplace for Malaysian F&B shifts, so the design should be practical, fast, and calm.

## Mobile-First Rules

- Design for small mobile screens first.
- Keep screens focused and easy to scan.
- Put the primary action where the user's thumb can reach it comfortably.
- Use clear hierarchy: title, key details, primary action, secondary details.
- Avoid dense dashboards, multi-column layouts, and crowded cards on mobile.

## Interaction Rules

- Core actions should take 3 taps or less where possible.
- One screen should usually have one primary action.
- Use direct actions for booking, posting, editing, cancelling, and approving.
- Confirm destructive or high-impact actions.
- Avoid long setup flows unless the current phase requires them.

## Visual Rules

- Use generous spacing without wasting screen space.
- Prefer readable lists and compact detail sections over decorative layouts.
- Keep cards simple and purposeful.
- Use status labels consistently for shift and booking states.
- Use color to support meaning, not as the only way to communicate state.
- Keep typography readable for outdoor, on-shift, and quick-glance use.

## Form Rules

- Keep forms short and grouped by task.
- Ask only for information needed in the current phase.
- Use sensible defaults for Malaysian F&B shift posting, such as date, time, location, pay, and role.
- Validate fields inline and explain errors plainly.
- Avoid optional fields that do not affect the current workflow.

## Role Experience

- Worker screens should emphasize finding, understanding, and booking suitable shifts quickly.
- Business screens should emphasize posting shifts and seeing fulfillment status clearly.
- Admin screens should emphasize oversight, exception handling, and safe moderation.
- The active role should always be obvious from available actions and navigation.

## Content Rules

- Use plain, direct language.
- Keep labels short.
- Avoid marketing copy inside operational flows.
- Use local-friendly terms for pay, dates, times, and locations.
- Show the most decision-relevant shift details before secondary information.

## Anti-Patterns

- Do not create congested dashboards.
- Do not hide primary actions behind deep menus.
- Do not require unnecessary onboarding before a user can understand the app.
- Do not add payment UI before the payment phase.
- Do not add AI matching UI before the smart matching phase.
- Do not add decorative complexity that slows down core shift workflows.
