---
version: 1
slug: "index-html"
primary_target: "index.html"
related_targets: []
---

# Surface: 알바 머니 미터 main app (index.html)

Mode: Operate. Audience: anyone paid hourly (students, work-study, office workers, freelancers), phone glance and desktop tab about equally. Task: see what my time is earning now, what's next (shift, payday, goal), keep the schedule accurate, compare with friends. Constraints: single static index.html, no build; Firebase friend-ranking logic and data shape unchanged; calculation logic unchanged; localStorage key unchanged.

## Direction contract

THESIS: A calm everyday-money app where the live amount and "what's next" are the only loud things; it refuses the gamified sticker-card dashboard (offset shadows, gradients, emoji icons, display type on every number) that the current build ships.

OWN-WORLD: Warm tinted ground, white soft-cornered cards (~20px radius, no borders, no offset shadows), one deep green action colour used only on pressable things and the live/progress mark, warm greys for text, line icons drawn as small inline SVG, one humanist Korean sans (Gothic A1) at a real type scale; tabular figures for all money.

STORY: The visitor sees today's money moving (or, off-shift, when they next start and what this week made), knows payday and goal at a glance, and finds records, friends and settings in a bottom tab bar. Setup is a 3-step sheet that ends with the total counting up.

FIRST VIEWPORT: Top: app name left, status pill right. Hero card: period segmented control (오늘/이번 주/이번 달/전체) directly above a large ticking amount, rate line, and a thin shift bar ("퇴근까지 n분"); off-shift the hero leads with 다음 출근. Below: two half cards (다음 월급날 D-day + amount; 목표 ring + %). Bottom tab bar: 홈 · 기록 · 친구 · 설정. On desktop the same column widens into two columns (hero + side cards), tab bar stays bottom-centered.

FORM: digital-design-canon-warm-consumer-app-surface (dealt challenger, user-chosen over the assigned banknote direction), rank: challenger. seed: 9b3ef960953b6884

Signature move: the goal ring, a single green arc that fills as savings reach the goal, with the live amount ticking beside it; motion is a soft press feedback, no bounce on entry.

FINISH: unreviewed and undocumented is unfinished; this build ends with the finish review, the verdict, DESIGN.md, and every shipping raster carrying its provenance
