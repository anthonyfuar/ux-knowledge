# Postel's Law (Robustness Principle)

## In one line
Strict on what goes out (sent / emitted), lenient on what comes in; plainly: own output strict + standard, varied input tolerated generously. Use when setting input parsing + validation tolerance, deciding where to stay strict (own output, inside system), checking layouts against difficult real data / any access method.
- Alias: Robustness Principle. Class: effect / principle.
- Theme: Complexity (group Complexity and robustness). Most affects: validation bounds + feedback, input parsing + normalization, accessibility across access methods.
- Core design rule: clear feedback + set bounds; within them accept varied input + normalize it when meaning clear.

## Applies when / does not apply when
|Lenient when|Strict when|
|---|---|
|input meaning unambiguous|meaning ambiguous: never accept silently|
|input within defined limits|interpreted value outside limits → clear feedback|
|clear feedback accompanies leniency|leniency would undermine output reliability / accessibility|
|at human interface|inside system + toward downstream systems: strict, explicit, validating|

Scope:
- Internal APIs, components + services in one product fall under it too: original principle already spanned program-to-program messaging, across network or inside one computer.
- Long tail of unusual inputs must not dictate design.

## Decision rules

### Building a robust application (in order)
1. Set, per context, what input counts as reasonable.
2. Clear feedback, above all when interpreted value outside those limits.
3. Accept many input forms, human needs first.
4. Convert input to system's format: application's job, not user's.

### Human face vs machine face
- Application has two faces: human-facing side tolerant + empathetic to varied input; machine-facing side treats input as potentially malicious, validates + normalizes before passing downstream.
- Mixing faces → database structure leaks into forms (strict formats imposed on people) or bad data enters systems.
- Meet whatever user does / enters w/ tolerance, flexibility + empathy.
- Plain feedback + input limits for user; input may arrive in many forms; system takes it in + converts to required form.
- If lenient parser turns free text into consequential value (amount / date triggering payment / booking) → read back to user before acting.
- Input leniency must not undermine output reliability or accessibility.

### Coverage
- Target common case (~95% of inputs parsed w/o friction); remaining 5% get respectful feedback loop.
- Validation failures = system shortcomings to design around, not user errors.
- Goal = accessible interface people can count on; means = designing for nearly every access method, capability level + input type.
- Resilience grows w/ each case foreseen + planned for.
- Pull extremes from real data, set limit covering nearly all content, fix outliers editorially.

### Citing
- Cite 1979/1980 origin + security-minded 1989 extension together.
- Many error-prevention fixes (idempotent submit, undo, soft delete, constraints) need no law → cite heuristic alone, not borrowed timing / motor law.

## Why it works

### Mechanism
- Robustness = absorb outside variation, keep own output predictable.
- Interpreting intent + normalizing messy input → fewer failures; consistent output + clear feedback build trust.

### Origin
- Began as TCP robustness principle, 1979-80, originally written for TCP.
- First written in 1979 IPv4 specification; used in January 1980 TCP specification.
- As TCP design guideline: deviation from specification tolerated on arrival if intent unambiguous, never on departure: program's transmissions match specification exactly.
- 1989 extension:
  - assume hostile hosts sending packets crafted for maximum damage;
  - accept unknown codes, possibly logging them, so protocols can evolve;
  - avoid sending legal but obscure features: they may expose receiver weaknesses;
  - cooperate to contain disruption from misbehaving hosts.

## Evidence
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Deviations from specification tolerated on arrival when intent unambiguous, never on departure: transmitted output matches specification exactly|networking engineering guideline + networking specifications (1979 IPv4, January 1980 TCP)|engineering guideline + specifications|lenient at human face, strict in own output|
|Non-conforming sender may work for years w/ lenient receivers, then fail against strict one; fault hard to trace + costly to fix|2001 critique|critique; recommended explicit consistency checks, even at some implementation cost|validate explicitly inside system|
|Principle's flexibility in onion-routing anonymity protocol could allow exploits compromising services' + clients' anonymity|2018 security analysis|security analysis|no leniency inside system|
|Robustness principle erodes robustness, security included, over time|2023 critique|argued|limit leniency; keep strict validation|
|Tolerating deviant input can hide defects|critique of robustness principle|can|set limits + give feedback|
|Input-handling leniency has security + maintenance costs|engineering critiques + 2018 security analysis|evidence against unlimited leniency|bounded leniency only|
|Archive of list-item titles: shortest 8 characters, longest over 320, only a handful above 80; team designed for 80-character maximum + edited the few outliers; edited titles better|2018 practitioner case, audit of client's full archive|single practitioner case|pull extremes from real data; limit covering nearly all; fix outliers editorially|

## Misreadings and limits
- Wrong: accepting ambiguous input silently → Right: lenient only when meaning unambiguous; set limits + give feedback.
- Wrong: applying Postel's Law leniency inside system too → Right: liberal at human face, strict + validating toward downstream systems; internal leniency hides defects + can invite exploitation.
- Wrong: reading good ratings of polished prototype as usability proof, or trusting demo filled w/ ideal content → Right: review w/ messy real content, sparse data + low-end devices.
- Wrong: letting long tail of unusual inputs shape design → Right: target common case (~95%), respectful feedback loop for rest.
- Limit: tolerating deviant input can hide defects.
- Limit: input leniency must not undermine output reliability or accessibility.

## Check questions
[A] = answerable from artifact itself (screen, prototype, spec). [P] = needs evidence about process or research.
- [A] Clear feedback + limits, varied input accepted + normalized? Look for: rigid formats; rejection of unambiguous input; silent failures.
- [A] Consequential interpreted inputs read back to user before acting? Look for: lenient parser silently turning free text into amount / date triggering payment or booking.
- [A] Strict, validating system behind forgiving surface? Look for: database structure leaking into form rules; unvalidated input passed downstream.
- [A] Output consistent, reliable + accessible? Look for: input leniency leaking into unpredictable output.
- [P] (Aesthetic-Usability, Postel's Law) Layout tested w/ extreme content, not only ideal placeholders? Look for: short names + studio photos in mockups; unchecked longest + shortest real values, missing images, larger fonts, long translations, right-to-left scripts.
- [A] (Postel's Law for any access method, Fitts's Law) Every action reachable + operable by keyboard, logical order, visible focus indicator? Look for: hover-only menus; focus traps; invisible focus.
- [A] (Postel's Law, Cognitive Load) Every control exposes its name + state to assistive technology? Look for: icon-only buttons w/o accessible name.
- [A] (Postel's Law, Von Restorff Effect) Layout holds at 200% text size, w/ platform text scaling (Dynamic Type, Android font scale) + reduced motion on? Look for: clipped labels; fixed-height buttons; motion w/ no off switch.
- In usability review checklist these questions sit under theme Systems and behavior.

## Symptoms → fixes
|Symptom|Likely cause (laws)|Fix|
|---|---|---|
|Strict input format rejects valid entries|Postel's Law|within bounds + w/ explanation, accept varied formats + normalize|
|Layout breaks w/ real content|Aesthetic-Usability, Postel's Law|design + review w/ longest, shortest + missing real values, larger fonts + long translations|
|Strict formats imposed on people in forms|database structure leaking into forms (two faces mixed)|tolerant human face; application does conversion|
|Bad data reaches downstream systems|leniency applied inside system (two faces mixed)|validate + normalize on machine face before passing downstream|
|Free-text entry triggers wrong payment or booking|lenient parser acting w/o read-back|read interpreted value back before acting|

## Hypothetical examples
- Hypothetical: same meaning, different strings → money-transfer form: person may write amount w/ currency sign, spaces between thousands or comma as decimal mark; to person all one amount, to code different strings → form normalizes them to one amount.
- Hypothetical: people tolerant, form rigid → post-office clerk accepts address w/ house number before or after street name; online change-of-address form rejects every order but its own → fix accepts both orders + normalizes.
- Hypothetical: strict out, lenient in → library-catalogue service accepts loosely formatted records from many partner libraries but always exports in one strict standard format to shared union catalogue.
- Hypothetical: read-back → banking chatbot hears "pay the electrician the usual amount next Friday" + shows interpreted payee, amount + date for confirmation before scheduling anything.

## Humane bound
- Bounded by Resilient: abuse taken as given.
- Bounded by Inclusive: any input, access method + capability level.
- Turned against people: leniency inside system hides defects + can invite exploitation (2018 onion-routing anonymity analysis).
- Turned against people: ambiguous input accepted silently.
- Further reading: errors, input tolerance + edge cases patterns; inclusive + accessible design patterns (accessibility floors: zoom, motion, readable text, semantics; common devices behind access-method, text-scaling + low-end-device checks).

## Related
- ../principles/resilient.md: humane principle bounding Postel's Law; abuse taken as given.
- ../principles/inclusive.md: humane principle bounding Postel's Law; any input, access method + capability level.
- ../patterns/errors-and-input-tolerance.md: applies Postel's Law; further reading on humane bound.
- ../patterns/inclusive-and-accessible-design.md: accessibility floors + devices behind access-method, text-scaling + low-end-device checks.
- ../checklists/usability-review.md: Postel's Law questions sit under theme Systems and behavior.
- ../checklists/usability-heuristics-map.md: heuristic "Error prevention" (related laws: Postel's Law, Fitts's Law for spacing of destructive targets, Working Memory); classic usability heuristics date from 1990, revised 1994; many error-prevention fixes need heuristic alone.
- teslers-law.md: same theme (Complexity).
- cognitive-load.md: shares question on name + state exposed to assistive technology.
- jakobs-law.md: expectations people bring from products they already use.
- aesthetic-usability-effect.md: shares difficult-data question, layout-breaks-with-real-content fix + polished-prototype misreading.
- fittss-law.md: shares keyboard-reachable question; named together w/ Postel's Law under "Error prevention" heuristic.
- ../guides/laws-and-principles-crosswalk.md: names humane principle bounding Postel's Law.
- ../patterns/forms-and-data-entry.md: applies Postel's Law.
