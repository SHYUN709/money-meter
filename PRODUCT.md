# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Anyone paid by the hour in Korea: university students in part-time jobs (알바) and work-study (근로장학생), and also office workers and freelancers paid hourly. They use it alone to see what their time is earning, and in small friend groups to compare earnings. They open it about equally on a phone (a quick glance during or between shifts) and on a computer (left open in a tab, e.g. in a work-study office).

## Product Purpose

Turns an hourly wage and a work schedule into money that visibly accumulates, second by second, during working hours. It answers "how much have I earned today / this week / this month / so far", "how much lands on the next payday, and when", and "how close am I to my goal". Success is that the user trusts the number and feels their work adding up.

## Positioning

The amount is computed live from the user's own schedule and real exceptions (days off, changed hours, entered hours), so it moves only while they are actually working, and it speaks Korean hourly-work reality: the 최저시급, a monthly payday for the previous month's work, and the 근로장학생 hour cap as a goal mode.

## Operating Context

- Set up once: wage, start date, payday (day of month), weekly schedule (several blocks per day for breaks), then occasional date exceptions.
- Daily: glance at the live amount and status (working / resting, next shift), payday D-day, goal progress.
- Social: a friend group joined by invite code or link; friends' earnings are recomputed on each screen from their shared wage and schedule.
- Single static `index.html` with no build step, deployed on Vercel from GitHub `main` (also usable as a local file or on GitHub Pages).

## Capabilities and Constraints

- Periods: today, this week, this month, all time. Monthly settlement list with month-end projection.
- Goal modes: target amount (named goal) or hour cap (with optional end date).
- Payday: D-day, amount for the previous month's work, countdown.
- Secondary features, kept but moved behind the core (user decision 2026-11-02): levels/XP, achievement badges, "what this buys" conversions (치킨, 아메리카노, 국밥, 삼각김밥), sound effects, coin effects.
- Friend ranking via Firebase (anonymous auth, Firestore `groups/{code}/members/{uid}`). Only nickname, wage, start date, schedule, exceptions, mode and cap are shared; amounts are computed client-side. Firebase logic and data shape must not change in visual work.
- Amounts are pre-tax. Personal records are stored in the browser (localStorage).
- Undecided: 주휴수당 (weekly holiday allowance) calculation is requested but not built yet.

## Brand Commitments

- Name: 알바 머니 미터. Korean UI, friendly 해요체 voice.
- Level titles ladder (신입 알바 → … → 알바의 신) and the piggy bank as the goal object exist today; whether they stay visually is a design decision, but the features stay.

## Evidence on Hand

- No testimonials, user counts, or press. Do not invent any.
- Real content: the 2026 최저시급 (10,320원) hint, item prices used for conversions.

## Product Principles

1. The number must be trustworthy: show how it was computed (pre-tax, schedule-based) and never silently change what the user entered.
2. The live amount and what is next (shift, payday, goal) come first; everything else is secondary and stays out of the way.
3. Calm over noise: reward progress without competing for attention.
4. Works for any hourly worker, not only students.
5. Equally good on a phone glance and a desktop tab.

## Accessibility & Inclusion

Keyboard reachable controls, visible focus, WCAG AA contrast in light and dark modes, 44px touch targets, respect `prefers-reduced-motion`, and no meaning carried by emoji or colour alone.
