# Search and results

## Scope
- Query entry, predictive suggestions, where refinement + filters go, result speed, results layout, long facet lists, zero results, forgiving input, known-item search.
- Open when designing/reviewing search box, predictive suggestions, results page, filter/facet panel, no-results state.

## Laws behind these patterns
|Law|Role here|
|---|---|
|../laws/hicks-law.md|decision time vs option count → suggestions, deferred refinement, facet ordering|
|../laws/working-memory.md|echoing query; counts beside filters|
|../laws/doherty-threshold.md|result speed|
|../laws/chunking.md|each result = separate chunk|
|../laws/proximity.md|gaps between results|
|../laws/uniform-connectedness.md|borders around special results|
|../laws/choice-overload.md|filters to shrink big sets|
|../laws/selective-attention.md|known-item search; matching search template|
|../laws/cognitive-load.md|linear scanning of long facet lists|

## Before the query

### What belongs on the search entry screen?
- When: search entry + any one-goal task (single-purpose entry).
- Do: nothing inviting extra decisions; search input autofocused, central, dominant.
- Avoid: advanced options, promotions, content on entry screen.
- Case: Google Search = reference case; landing page barely changed since 1998 launch. Speed has three sources: results easy to skim, quick delivery, nothing obstructing query.
- Hypothetical: city library catalogue opens on one focused field, cursor already in it; events, opening hours + advanced filters wait until query exists.

### One search box or several?
- Do: one universal search box tolerating typos, plurals + hyphens; curate best results for key queries.
- Avoid: several scoped boxes on one page → users pick wrong one + conclude content does not exist.
- Case: university library homepage split logistics + research-catalog searches into separate boxes = instance of several-scoped-boxes problem.
- Hypothetical: hospital intranet merges staff-directory box + policy-document box into one field; ward-name query returns both people + ward's procedures.

### Suggest terms while the person types?
- Do: list likely terms beneath field, refreshed each keystroke (predictive suggestions).
- Why: less typing + less thinking, since person can choose wanted term early (Hick's Law).
- Hypothetical: hardware-store search offers "cordless drill", "drill bits", "drill press" after a few letters; shopper taps right one instead of finishing word.

## Returning results

### How fast must results arrive?
- Do: speed = feature: results under 400 ms where possible → mind does not drift (Doherty Threshold). Results page may show retrieval time.
- Hypothetical: travel-booking site returns flight matches fast enough for traveller's eyes to stay on list, w/ small note of search time.

### Where do filters, sort and advanced search go?
- When: filters, sort, advanced search (deferring refinement).
- Do: on results page → extra decisions come only once query exists. Complexity where it helps, away from where it would add friction. Large result/catalog set (Choice Overload) → let people shrink set early w/ filters + search, before choice itself.
- Hypothetical: job board shows salary, location + contract filters beside results, not as pre-search form.

### How is the results page laid out?
- Do: at top, repeat query as typed, in plain view (echo query). Wide gaps between results (Law of Proximity) → each stands apart as own chunk. Inside each result, one repeated hierarchy. Result differing in kind from ordinary ones → frame it (Law of Uniform Connectedness): frame sets it off from results around it, lifts its priority + makes it read as one unit. Reference-material side card + definition heading only for queries calling for them.
- Avoid: borders everywhere: enclosure raises priority → reserve it for deserving items.
- Why: scanning results = many small judgments, one per item on page → people lose track of what they asked.
- Case (Google results page): online encyclopedia article on searched term = usual target of reference side card's link.
- Hypothetical: pharmacy product search repeats "results for: allergy tablets" above list, spaces each product apart w/ same name-price-dose order, boxes only pharmacist-recommended item.

### Long facet list: how to make values findable?
- When: one filter has many values (brands, locations, tags, accounts).
- Do: most used/recently used values first, w/ counts, then Show all opening in-facet type-ahead. Meaningful headings if natural grouping exists. Pin selected values at top as removable chips.
- Avoid: scrolling checkbox list dozens of values long w/o search; facet-list scroll position reset on each selection.
- Why: people not knowing exact label scan list linearly = scanning + finding load (Cognitive Load) → recency, frequency + in-facet search help more than alphabetical order.
- Limit: alphabetical order helps only people knowing exact label.
- Origin: search benefit of ordered lists from 1985 research, later extension, not part of original experiments behind Hick's Law.
- Hypothetical: expense-report vendor filter lists vendors this employee used most, w/ counts, then "Show all" w/ type-to-find box; chosen vendors sit at top as chips w/ remove mark.

## Zero results and known items

### What does a zero-results page offer?
- Do: never dead-end: repeat query; offer spelling correction/broader match (Postel's Law); name set-emptying filter + one-click removal; related content or route to human. Counts beside filter values → people avoid empty combinations (Working Memory).
- Avoid: bare No-results page = dead end; user cannot tell whether search failed or item missing (visibility-of-system-status + error-recovery heuristics).
- Why: blank no-results page = possible negative peak, + remembered ending if session stops there (Peak-End Rule, secondary reason; name both halves, peak + end).
- Hypothetical: council planning-permit search finds nothing for misspelled street → shows query, suggests correct spelling, says date filter emptied set w/ remove control, links to planning desk's contact page.

### Hunting a known item: how to match the search template?
- When: people hunt known item (command, setting, product, label).
- Do: known-item targets match user's mental image: same wording, icon + colour everywhere. If item's role must change → flag change explicitly + expect slips.
- Avoid: restyling/renaming recurring items; swapping targets.
- Why: w/ stable styling of targets + distractors, visual search becomes automatic w/ practice (Selective Attention).
- Hypothetical: banking app keeps "transfer" action's label, icon + colour same on every screen; when transfers move into new payments hub, one-time note points to new place.

## Related
- lists-options-and-choice.md: option counts, ordering + comparison once result set on screen.
- layout-grouping-and-hierarchy.md: grouping cues, spacing + containers behind scannable result chunks.
- feedback-loading-and-performance.md: response-time budgets, indicators + waits for returning results.
- errors-and-input-tolerance.md: tolerant input + recovery, for forgiving queries + zero results.
- ../checklists/usability-heuristics-map.md: heuristics named under zero results + laws behind each.
- ../laws/hicks-law.md: decision time vs option count; behind suggestions, deferred refinement, facet ordering.
- recommendations-and-personalization.md: humane bounds on algorithm-ranked results + steering controls.
- transparency-and-honesty.md: honest controls; explaining algorithm ordering what people see.
- ../laws/cognitive-load.md: scanning + finding load behind facet ordering.
