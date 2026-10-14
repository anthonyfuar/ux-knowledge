# Object-oriented UX (objects before screens)

## Use when
- Structuring product before any screens drawn: map objects in user's mental model, their content, nesting + rank; 6 steps.
- Named approach dates from 2015.
- Premise: users think in real-world things, not interface verbs.

## Steps
1. **Core objects = nouns recurring in brief.** Drop abstract outcomes. Collection words (library, catalog, calendar, map) name object views, not objects themselves.
2. **Infer hidden objects from verbs** + record each object's states.
3. **Split each object's core content from its metadata.** Metadata = anything users sort / filter object by.
4. **Nest objects**: what sits inside what → relationships + contextual navigation between them.
5. **Force-rank each object's elements**, no ties. Rank → size, color / disclosure level; not necessarily screen position.
6. **Start layout as single ranked column**, even for desktop software. Why: mobile-first design forces prioritization.

## Decision rules
- If candidate object = abstract outcome → drop from object list.
- If noun = collection word → model as view of some object, not as object.
- If verb recurs in brief → find hidden object it implies + record its states.
- If two elements tie in rank → force choice; ties not allowed.
- If top-ranked element not at screen top → fine; rank may show as size, color / disclosure instead.

## Evidence
|Finding|Study (year, kind, sample)|Strength + caveat|Design consequence|
|---|---|---|---|
|Responsive election-night build organized around three objects: states, races, state-race results|news site, 2012; one practitioner case|only evidence; no controlled measures of method's effect exist|treat method as structuring aid, not proven performance gain|

## Limits
- Object map = first draft only.
- No controlled measures of object-oriented UX's effect.

## Hypothetical examples
- Hypothetical (things vs verbs): people planning trip think in flights, hotels, bookings; not in "sort", "refine" / "toggle view".
- Hypothetical (hidden object from verb): in city repair-request portal, "report a pothole" implies hidden repair-request object w/ states e.g. submitted, scheduled, fixed.

## Related
- ../laws/mental-model.md: objects drawn from user's mental model.
- ../patterns/navigation-and-menus.md: step 4 nesting feeds navigation ordering, grouping + depth.
- [Content layout, grouping and visual hierarchy](../patterns/layout-grouping-and-hierarchy.md): turns step 5 ranks into size, color / disclosure via emphasis + reading order.
- ../patterns/search-and-results.md: filters + results layout built on step 3 metadata.
- [Mapping memory demands in a flow](mapping-memory-demands.md): builds information architecture from users' own categories via card sorting + tree testing.
- [Stating and citing evidence accurately](../evidence/stating-evidence.md): quoting evidence accurately; here single practitioner case.
- ../principles/surface-to-principle-map.md: humane principles each product surface touches first + where to start.
