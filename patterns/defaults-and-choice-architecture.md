# Defaults and choice architecture

## Scope + principles behind these patterns
- Use for: humane patterns on defaults · opt-in · equal-weight decline · symmetric exit · limiting choices · sharing on person's behalf.
- Applies when: designing/reviewing any preselected option, consent/permission prompt, configurator, cancellation or sharing flow.
- Principles underneath:
  - ../principles/intentional.md: honest defaults, withheld defaults, limited choices, deliberate sharing. Named first on more default patterns than any other principle.
  - ../principles/empowering.md: equal-weight decline, symmetric exit, curation, withheld defaults, deliberate sharing.
  - ../principles/transparent.md: opt-in.
  - ../principles/respectful.md: sequencing + limiting choices.
  - ../principles/resilient.md: personal settings override group + automated actions.

### What should a preselected option be?
- When: any preselected option; rules apply since most people never change default.
- Do:
  - Default = honest, beneficial suggestion (Intentional): favours privacy, calm, safety or savings.
  - Default = recommendation you'd defend aloud.
  - Default earns place only if person lacks knowledge/time for own preference + has reason to trust setter.
  - If either condition fails (person has knowledge + time, or no reason to trust setter) → ask, don't preselect.
  - Pick value you most want people to end at, not merely value better than zero.
- Avoid: defaults chosen to raise data collection/session length, e.g. notifications on, autoplay on, sharing public.
- Why: experts + audiences w/ no grounds to trust setter see preselection as nudge. Default = both ceiling + floor on people's final choice.
- Evidence:
  - Workplace savings: default contribution rate moved from nothing to modest figure → more people saved, but fewer saved more than new default.
  - Classic research: opt-out enrolment roughly doubled organ-donor consent.
  - Retirement plans w/ modest default contribution raise participation.
- Hypothetical: energy-supplier sign-up preselects lowest-cost tariff household qualifies for + one-line reason supplier would state aloud.

### Identity, consent, money, relationships: preselect or not?
- When: identity, consent, money or relationship decisions, where active choice matters.
- Do: withhold default → neutral choice, no preselection, visible trade-offs.
- Avoid: pre-ticked consent boxes; "we assume you agree" banners.
- Why: Intentional + Empowering: active choice matters here.
- Hypothetical: pension form asks for beneficiary if member dies; no name prefilled; each option shows household impact.

### Collecting, sharing or personalising on data: opt-in or opt-out?
- When: collecting, sharing or personalising on data.
- Do: opt-in, not opt-out. Start w/ nothing collected; ask for data in context, benefit stated clearly; withdrawing consent as easy as giving it.
- Avoid: quietly switching permission from "while using" to "always" + waiting to see if people object.
- Why: Transparent.
- Case: ride-hailing company quietly switched setting from "while using" to "always"; reversed within a year.
- Hypothetical: home-energy monitor keeps readings on device; asks to upload only when person opens "compare w/ similar homes", stating what comparison gives.

### Multi-step configuration or checkout: how many choices, in which order?
- When: multi-step configuration or checkout.
- Do: fewer options; few-option attributes before many-option ones; remember preferences + offer "same as last time".
- Avoid: front-loading long, complex choice so people give up + accept preselection; re-asking configuration every visit.
- Why: Intentional + Respectful.
- Evidence: well-known study: six-jam display outsold twenty-four-jam display (see ../laws/choice-overload.md for when overload occurs).
- Hypothetical: rail-ticket flow asks one-way vs return + class first, then lists many departure times; returning traveller sees "same as last time" for seat preference.

### People struggle to choose from a large catalog: curate how?
- When: people struggle to choose.
- Do: short, explained shortlist + one-tap access to full unpersonalised catalog.
- Avoid: home screen of algorithmic rows w/ no index.
- Why: Empowering. Choice tax = burden of having to choose; curation should cut it w/o hiding full catalog.
- Evidence: 2023 survey: a fifth of streaming viewers gave up choosing entirely.
- Hypothetical: university course catalog opens on "suggested for your major" list, each w/ reason, next to "all courses A–Z".

### Prompt w/ an accept path: how visible is the No?
- When: any prompt w/ accept path.
- Do: decline, skip + email-only options get accept's size, contrast + position; every prompt has obvious escape.
- Avoid: tiny grey "no"; mandatory phone-number path hiding email path; install wall w/ no way to dismiss.
- Why: Empowering (equal-weight No).
- Hypothetical: banking app's paperless-statements prompt shows "keep paper" button matching "go paperless" in size, contrast + position.

### Cancel, unsubscribe, delete account: how hard to leave?
- When: cancellation, unsubscribing, account deletion.
- Do: leaving as fast, as available online + as discoverable as joining. One honest confirmation (what person keeps/loses) → let person go.
- Avoid: phone-only cancellation; multi-screen retention gauntlets; guilt copy on exit; making people retype email "so we can remove you".
- Why: Empowering (symmetric exit).
- Case: lingerie subscription simplified cancellation → refunds rose 30% + subscriptions fell 15%, revealing how much revenue cancellation friction had extracted.
- Hypothetical: gym membership joined online cancels online from same account page: one screen states remaining visits + end date, then confirms.

### Activity could be auto-published: share on the person's behalf?
- When: platform could auto-publish person's activity, memberships, listening or reading.
- Do: never act on person's behalf w/o deliberate share → conscious per-item decision before sharing anything.
- Avoid: auto-publishing activity.
- Why: Intentional + Empowering.
- Case: large network rolled back "frictionless sharing" of third-party app activity after people felt loss of control.
- Hypothetical: e-reader asks after each book whether to add it to shelf friends can see; nothing added unless reader says yes per book.

### Groups, admins, tags or automation attach content to a person: whose setting wins?
- When: groups, admins, tags or automation can attach content to person.
- Do: individual privacy choices beat group defaults; person's approval required before being tagged/listed.
- Avoid: precedence rules letting group/admin actions override personal settings.
- Why: Resilient.
- Case: precedence rules outed student when group admin added her to chorus group, overriding her carefully configured privacy settings.
- Hypothetical: workplace chat needs employee's approval before manager can add them to channel listed in public directory.

## Related
- ../principles/intentional.md: named first on more default patterns than any other principle; honest + withheld defaults.
- ../principles/empowering.md: equal-weight decline, symmetric exit, curation, deliberate sharing.
- ../principles/transparent.md: opt-in.
- ../principles/respectful.md: sequencing + limiting choices.
- ../principles/resilient.md: personal settings override group + automated actions.
- lists-options-and-choice.md: usability side: option counts, ordering, comparison + pricing tiers.
- ../laws/choice-overload.md: usability law on large option sets; jam study + when overload occurs.
- ../evidence/decision-fatigue-and-choice.md: evidence on defaults, choice overload + decision quality.
- ../ethics/deceptive-patterns.md: taxonomy: each deceptive pattern, how it works + honest alternative.
- ../ethics/influence-vs-manipulation.md: test whether persuasive lever serves or exploits person.
- privacy-data-and-security.md: consent, data minimisation, access + deletion.
- friction-undo-and-confirmation.md: confirmation graded by consequence; friction serving person.
- complexity-management.md: system absorbing decisions via defaults user can still change.
