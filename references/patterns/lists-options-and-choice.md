# Lists, options and choice

## Scope + laws behind these patterns
- Use for: option-set usability patterns: how many to show · how to sequence + order · side-by-side comparison · pricing tiers · first numbers + frames · action placement by frequency.
- Applies when: designing/reviewing option lists, plan pickers, catalogs, comparison tables, price displays or feature placement.
- Laws underneath: ../laws/hicks-law.md, ../laws/choice-overload.md, ../laws/serial-position-effect.md, ../laws/pareto-principle.md, ../laws/cognitive-bias.md, ../laws/millers-law.md.

### Many options compete: cut, sequence or feature?
- When: many options compete, especially where response time matters.
- Do: cut option count. Sequence options across steps. At any one time lead w/ item mattering most, like featured product.
- Avoid: over-reducing options into meaningless abstraction. Believing more choice satisfies more people (myth).
- Why: Choice Overload hurts twice: overall experience feels worse + decisions slower + worse. ../laws/choice-overload.md, ../laws/hicks-law.md.
- Hypothetical: pension-fund portal asks risk level first, then shows only funds within it, one fund highlighted per step.

### Catalog must be large but each purchase is one item?
- When: large catalog required but each purchase = one item (go wide to browse, narrow to decide).
- Do: separate category choice from item choice. At decision point narrow set: curated sets, clearly dominant recommended pick, concise comparison text. Set must stay large → no artificial time pressure.
- Avoid: whole assortment at item-choice step. Options added for curious minority at majority's cost.
- Why: assortment breadth draws people in; images in broad assortment make browsing feel faster + suggest variety.
- Evidence: 2000 grocery-store field study: 24-jam display stopped more shoppers, 6-jam display sold far more.
- Limit: gift finders + flows for choosing on someone else's behalf tolerate larger option sets.
- Hypothetical: tile retailer site: wide photo grid of styles to browse; style picked → short curated set, one tile marked "recommended for wet rooms".

### Options must be weighed side by side?
- When: decision truly hinges on judging alternatives against each other, e.g. competing products/price levels.
- Do: related options adjacent. Carry option details into comparison tables → system holds what memory cannot.
- Steps: 1. Map what users must carry mentally at each step. 2. Store it for them: aligned tables, shortlists/carts, persistent selections, pre-computed differences.
- Avoid: making users remember attributes across screens. Making users mentally combine >2-3 interacting variables.
- Limit: even w/ all data on screen, it can exceed limit on how many relations people can grasp at once.
- Why: ../laws/millers-law.md.
- Hypothetical: mortgage comparison: rate, fees + term in one aligned table, monthly-cost difference between offers pre-computed.

### Comparing plans, tiers or specs?
- When: pricing tiers, plan pickers, spec comparison tables (compare against user's criteria).
- Do: frame comparison against user's stated criteria. Mark task-relevant differences, e.g. "matters for you" tag. Drop options worse on every attribute unless they meet real need.
- Avoid: decoy effect = deliberately weak middle/anchor tier pushing people toward higher-margin plan (manipulation). Distinction bias = spec tables making trivial differences look decisive.
- Why: ../laws/choice-overload.md, ../laws/cognitive-bias.md; manipulation tests in ../ethics/influence-vs-manipulation.md.
- Hypothetical: broadband plan picker asks household needs (upload speed for home work, no fixed contract) + tags those rows "matters for you"; plan slower + pricier than another on every line dropped.

### Which number and frame to show first?
- When: prices, suggested donations, default tips/quantities, risk + consent statements.
- Do: show most honest relevant reference value first. Keep unrelated figures away from decisions. Consequential choices (health, money, privacy) → both frames, e.g. 95% succeed + 5% fail, plus base rates. Independent judgments (reviews, estimates) → collect user's own value before showing system's suggestion. Show price + intended audience per offer, e.g. serves 100 people or 100,000.
- Avoid: struck-through reference prices or first amounts shown only to inflate spending. Prominent steep-discount displays.
- Why: something always anchors numeric judgment. Price shows most concretely what offer amounts to + whom it serves; no price → visitors conclude offer not for them. Internal reference price = ~weighted blend of highest + most recent prices person has seen.
- Evidence: one study: steep discounts can permanently erode demand, because low price stays salient.
- Hypothetical: charity donation form suggests amount donors most often give + what it funds, not pre-filled high amount next to struck-through "usual" figure.

### Framing options for people who decide w/ shortcuts?
- When: framing options (users decide w/ heuristics).
- Do: expect heuristics + biases to shape choices.
- Limit: knowing about bias → catch it more often, in users, stakeholders + yourself; bias itself stays.
- Term: confirmation bias (classic) = prior belief steers what people look for, how they read it + what they remember, toward confirming belief.
- Why: ../laws/cognitive-bias.md.
- Hypothetical: team reviewing plan-page test notices they quote only feedback favoring tier they already preferred.

### Which options, features or issues to polish first?
- When: prioritizing options, features or issues to polish (invest in the vital few).
- Do: find small share of inputs driving most outcomes. Effort where most users benefit.
- Limit: 80/20 split = approximate; holds in many, not all, systems.
- Why: ../laws/pareto-principle.md.
- Hypothetical: public-library app team ranks support requests by volume → polishes renewals + holds before rare inter-library loan settings.

### Where does each action go?
- When: placing actions + features (Pareto Principle applied to feature availability).
- Do: few most-needed actions at point of use. Rarer actions in one predictable secondary place.
- Symptom: action hunt = same action might sit on page, in detail view, in one of several overflow menus or in global navigation.
- Avoid: judging design by click count alone; predictable click costs less than search.
- Why: ../laws/pareto-principle.md.
- Hypothetical: payroll tool puts "approve timesheet" on each row; "export audit log" only in one settings menu.

## Related
- ../laws/choice-overload.md: law behind reducing, curating + narrowing option sets, w/ limits + evidence.
- ../laws/hicks-law.md: decision time vs option count; when it applies to lists + when not.
- navigation-and-menus.md: ordering, grouping, depth + visibility when options = navigation.
- search-and-results.md: search + filters shrinking big sets before choosing.
- defaults-and-choice-architecture.md: humane bounds on defaults, opt-in, equal-weight decline.
- ../ethics/influence-vs-manipulation.md: tests whether framing, anchor or tier lever serves person or exploits them.
- ../ethics/deceptive-patterns.md: named deceptive patterns + honest alternative to each.
- ../evidence/decision-fatigue-and-choice.md: evidence on defaults, choice overload, decision quality.
