# Occam's Razor

## In one line
Parsimony as tie-breaker: fewest-assumption option wins, but only between rival hypotheses/design options w/ equal predictive power. Modern reading: entity added only when needed, never in surplus. Use when: deciding what to remove; choosing simpler vs more elaborate solution; running design critique; checking if parsimony = right argument to cite.
- Aliases: Ockham's razor; lex parsimoniae (law of parsimony). Class: effect/principle.
- Theme: Decisions. Matters most for: removing elements one by one; simplest solution as starting point; critique process.
- Core rules: drop elements w/o function; start = simplest solution; done-test = try one more cut: if anything can still go → keep editing; stop only once every attempted cut fails.

## Applies when / does not apply when
|Situation|Razor applies?|Note|
|---|---|---|
|options predict or serve equally well|yes: arbitrates only here|simpler wins only when options perform equally|
|simpler option performs worse|no|parsimony applies only when alternatives perform equally|
|provisional choice before evidence exists|yes|once data exists, data wins|
|removal would cost function|no|never remove at cost of function|
|deciding truth|no: razor does not call simplest explanation true|—|
|complexity people value|target = appropriate complexity, not minimum|keep valued complexity|
|jargon among insiders fluent in it|legitimate there|strip from general UI copy|
|simplicity vs clarity|clarity wins|never trade clarity for simplicity|

## Decision rules

### Start simple
- First attempt = simplest working thing; add nothing beyond it until need shows.
- Complexity never introduced beats complexity trimmed afterwards.
- Pick least powerful mechanism solving problem, e.g. simple form before wizard, static page before app.
- Rule of least power in code: native input types + required attributes before script validation; semantic elements before added roles.
- Keep interdependent parts per feature few.
- Test simpler design hypothesis first.
- Default to simpler design/model unless evidence favors complex one.
- Ask how simple something can get, not how much complexity it needs.

### Remove
1. Go through design element by element.
2. Overall function intact w/o element → remove it.
3. Audit every element strictly for its contribution: neither value nor meaning → delete; plainer form could also deliver it → use plainer form.
4. Judge every element by razor's aim: passes only if it blocks nothing (no barrier anywhere, path through content included) + backs up what content says. Payoff: people reach goal sooner.
5. Beware tidying controls out of view + flourishes meant to please: each may end up blocking. Hypothetical: rail-booking form folds passenger-count field into collapsed summary + plays jingle at every step; both may stand between traveller + ticket.
- Shrink test: strip interface away step by step; point immediately before content gets harder to find or its message stops landing well = right amount of UI.

### Know where to stop
- Cut functionality only where no significant penalty follows.
- Never remove at cost of function; never trade clarity for simplicity.
- Aim for appropriate complexity, not minimum: people value some complexity.
- Tesler's Law marks where cutting must stop.

### Measure both sides
- Fewer screens may mean denser screens or hidden modes → measure both sides when simplifying.
- Distrust preference surveys + feature checklists taken before use → measure satisfaction after real use; keep product focused.
- Analytics: drop-off more likely from slow page than from deep motivational problem.

### Run the critique
- Hold design critiques in repeated rounds: weak/unclear parts surface once designers must justify every choice.
- Ask explicitly in every review: what can we remove? (prompts editing stance vs additive bias)
- Before committing to appealing elaborate option, watch problem itself; such appeal flags missing information.

## Why it works

### Mechanism
- Each added element/assumption adds complexity + failure risk w/o any guarantee of value → fewer working parts preferable.
- Each added assumption/part = another chance of error; system w/ many essential components likely to fail somewhere even if each part reliable (1974 work on judgment under uncertainty). Failure odds rise w/ each added layer.
- Simpler models resist overfitting noise; fewer adjustable parameters → sharper predictions, easier to test + falsify (1991 analysis).
- Cutting complexity pays twice: people reach goal w/ less effort; design itself clearer + more forceful.
- Deliberate enrichment often backfires: people lose bearings + focus.
- Over-elaborating = slip of seasoned designers as well as beginners.
- Complexity bias makes complex ideas look smarter than simple ones.
- Additive bias: people systematically overlook subtractive changes + default to adding.
- Stakeholders often mistake simple result for low effort, though reaching it = hard work.

### Terms
|Term|Meaning|
|---|---|
|Razor|term's two senses: removal (premises an explanation can do w/o) / separation (two conclusions resembling each other)|
|Anti-razors|add factor when existing ones insufficient; do not reduce entities to point of inadequacy|
|Rule of least power|use least powerful adequate language or tool|
|Feature fatigue|feature-rich products win before use + lose after use|
|Constraint on theory-building|keep basic elements as few as possible w/o giving up adequate coverage of any single observation|

### Supporting maxims (prompts for editing, not evidence)
- Design maxim: solution needing less design = better.
- Literary aphorism: work becomes flawless once cutting finds no more candidates, not once addition ideas run out.
- Both = practitioner + literary aphorisms.

### Origin
- Credited to medieval thinker: heavy user, not inventor.
- Earlier parsimony forms predate razor: thinkers from antiquity through 13th century favored demonstrations from fewer postulates.
- Famous "entities" wording appeared 1639; label "Ockham's razor" 1649, centuries after razor's namesake.
- Later uptake: life sciences (medicine + biology), mathematics of uncertainty (statistics + probability theory) + scientific practice broadly.
- Support for preferring explanation w/ fewest assumptions = philosophical principle, not empirical study.

## Evidence
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Preferring explanation w/ fewest assumptions|philosophical principle|not empirical study|use as rule for provisional choices|
|No comparison had evidence balance favoring complexity|review of 32 papers, 97 comparisons of simple vs complex economic forecasting methods|review; economic forecasting domain|default to simpler unless evidence favors complex|
|Complex methods raised forecast error by 27% on average|review's 25 papers w/ quantitative comparisons|on average|—|
|Before use, people weighted capability over usability; after use, usability drove satisfaction, simpler version satisfied more, + most rejected high-feature model|2005 consumer experiments on feature fatigue|experiments|measure satisfaction after real use, not pre-use surveys|
|People systematically overlook subtractive changes + default to adding (additive bias)|2021 research|—|ask "what can we remove?" in every review|
|System w/ many essential components likely to fail somewhere even if each part reliable|1974 work on judgment under uncertainty|likely|fewer interdependent parts|
|Simpler models resist overfitting; sharper, more testable predictions|1991 analysis|analysis|test simpler hypothesis first|
|Guesses tend to come out narrower + more elaborate than needed, though hidden rule admits any rising triple|1960 rule-discovery task (2-4-6 task)|illustration of complexity bias|observe before elaborating|
|Most participants, after seeing 1 sample triple + free to test more sequences, settled on rule more elaborate than true one (any 3 numbers in rising order)|1989 reasoning experiment reusing 2-4-6 task|paper concludes students chose testing strategies sensibly per task; abstract: undergraduates used disconfirmation strategy when only evaluating hypotheses + counterfactual-inference strategy when also generating them, balancing task's logical requirements vs outcome desirability|cite for task-sensitive reasoning; demonstration only as complexity-bias illustration|

## Misreadings and limits
- Wrong: cutting elements until function breaks → Right: remove only what can go while full function remains.
- Wrong: preferring simpler option even though it performs worse → Right: parsimony applies only when alternatives perform equally.
- Wrong: razor argues for cutting for its own sake → Right: it presumes competing options perform equally + argues for fewest parts still working fully.
- Wrong: simplest explanation = true → Right: razor does not say so.
- Wrong: citing 1989 rule-discovery study as proof of complexity bias → Right: it shows task-sensitive reasoning; use it only to illustrate task; date 2-4-6 task itself to 1960.
- Wrong: quoting popular slogan form of theory-building constraint (keep things as simple as they can be, but no simpler) as verified quotation → Right: slogan's source unverified; paraphrase constraint (as few basic elements as possible w/o giving up adequate coverage of any single observation), do not quote slogan.
- Wrong: treating supporting maxims as evidence → Right: they = editing prompts.
- Limit: simplicity can move instead of shrinking: economy of practical expression distinct from economy of grammar + vocabulary; simplifying one can complicate its counterpart.
- Limit: fewer screens may mean denser screens or hidden modes.
- Limit: what counts as "simplest" subjective + prone to confirmation bias.
- Limit: parsimony wrongly invoked against phenomena later proven real: meteorites, continental drift, atoms.
- Limit: target = appropriate complexity, not minimum; people value some complexity.

## Check questions
[A] = answerable from artifact itself (screen, prototype, spec).
- [A] (Occam's Razor) Can any element go w/o losing function? Look for: elements w/ no meaning or value.
- Could any remaining interface go w/o content getting harder to find or its message landing less well?
- Competing options perform equally? If not → razor does not decide.
- Data already exists? If yes → data wins over razor.
- After simplifying: screens denser or modes hidden?
- Did review ask: what can we remove?

## Symptoms → fixes
|Symptom|Likely cause|Fix|
|---|---|---|
|Elements w/ no meaning or value on screen|additive bias; enrichment added w/o need|remove element by element while function intact|
|People get lost + lose focus on enrichment-padded screens (decorative flourishes, controls tucked out of sight)|additions blocking path through content|question + cut them; support content's message|
|Team drawn to elaborate solution|complexity bias; missing information|observe problem first; test simpler hypothesis first|
|Simplified flow now has dense screens or hidden modes|simplicity moved, not shrunk|measure both sides; aim for appropriate complexity|
|Feature-rich version wins pre-use survey|feature fatigue|measure satisfaction after real use; keep product focused|
|Drop-off blamed on deep motivation|elaborate explanation chosen first|check for slow page first|
|Flow cut until step protecting people gone|removing at cost of function|restore step; scale confirmation to severity|

## Hypothetical examples
- Hypothetical: valued complexity → home-audio app keeps many-band manual equalizer next to one-tap presets, because some owners enjoy tuning sound by hand.
- Hypothetical: least power first → clinic collects new patient's contact details w/ one plain form using native date + phone inputs, not multi-screen wizard w/ custom validation scripts.
- Hypothetical: humane stop → payroll tool trims approval flow but keeps review screen before salaries go out, because this pause = where mistakes get caught.

## Humane bound
- Bounded by Intentional: friction on purpose, w/ confirmation effort scaled to severity.
- Law itself records no abuse case; its pitfall = removing at cost of function.
- Misuse: removing steps for conversion, incl. step where deliberation, learning or ownership happens.
- Misuse: one-tap irreversible actions, removing pause protecting against impulse, accident + regret.
- Further reading: friction, undo + deliberate pauses (designing for meaning-building effort); convenience + friction evidence.

## Related
- ../principles/intentional.md: humane principle bounding it; friction on purpose, confirmation scaled to severity.
- ../patterns/friction-undo-and-confirmation.md: humane bounds on removing steps (confirmation graded by consequence, undo windows, speed bumps); meaning-building effort.
- ../evidence/convenience-and-friction.md: evidence for humane bound.
- teslers-law.md: marks where cutting must stop.
- hicks-law.md: shares heuristic "Aesthetic and minimalist design".
- cognitive-bias.md: linked via complexity bias + additive bias.
- ../methods/cutting-to-essentials.md: step list for simplifying design w/o losing function.
- ../methods/design-critique.md: running critiques where designers justify each decision.
- ../checklists/usability-heuristics-map.md: "Aesthetic and minimalist design" → Aesthetic-Usability Effect, Occam's Razor, Cognitive Load + Hick's Law; classic heuristics 1990, revised 1994.
- ../guides/laws-and-principles-crosswalk.md: maps humane principle bounding it.
- ../patterns/navigation-and-menus.md: applies it.
- ../patterns/complexity-management.md: applies it.
- ../patterns/first-impressions-and-aesthetics.md: applies it.
