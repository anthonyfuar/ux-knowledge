# Recommendations, ranking and personalization

## Scope
- Algorithm-ranked feeds, recommenders + personalization: steering controls, explanations, rabbit holes, sensitive states + inferred attributes, news pacing, prompted social acts, time cost.
- Open when designing/reviewing anything ranked, recommended or tailored per person.

## Principles behind these patterns
|Principle|What it governs here|
|---|---|
|../principles/empowering.md|ranking controls handed over; less decision load w/o hidden options; question as filter; contrary views w/ context|
|../principles/transparent.md|explained recommendations; prompted social acts disclosed|
|../principles/resilient.md|countering rabbit hole; sensitive-state guardrails; inferred sensitive attributes kept out; news pacing|
|../principles/intentional.md|approval separated from following; info kept out of friendship metaphor|
|../principles/respectful.md|prompted social acts disclosed; recognizing people, not only targeting them|
|../principles/finite.md|news pacing; time personalization consumes bounded|

## Steering and explaining the ranking

### Which levers do people get over the ranking?
- When: any ranked feed/recommender.
- Do: let people switch chronological/ranked order; offer following-only view; let people mute topics/sources; let them tune/reset model + choose which signals it uses.
- Avoid: opaque ranking w/ no user-facing levers.
- Why: Empowering (handing over ranking controls).
- Hypothetical: recipe-sharing app: cook can mute "desserts" topic, untick "recipes I saved" as ranking signal, reset suggestions from settings.

### Narrow the options without hiding them?
- When: algorithm narrows what people see or answers on person's behalf.
- Do: keep alternatives discoverable; provide show-me-everything/unpersonalized view; let people override narrowing.
- Avoid: taking agency away: system picks unasked + every alternative stays out of sight, never seen.
- Why: Empowering. ../laws/choice-overload.md = law behind narrowing options; bounded here by keeping alternatives discoverable.
- Hypothetical: job board's "best matches for you" shortlist keeps visible "see all openings" link + lists applied filters, each removable.

### Explain why this is recommended?
- When: anything labelled for you/recommended.
- Do: why-am-I-seeing-this affordance; show which signals (location, history, interests) influenced it; let people adjust them.
- Avoid: unexplained recommendation rows; silent profiling.
- Why: Transparent.
- Hypothetical: hardware-store app labels suggested drill-bit set "because you bought this drill" + lets shopper switch off purchase history as signal.

### Is the question itself the filter?
- When: people reach info via search box, prompt, suggested-query list or generated answer.
- Do: show which terms produced result; offer reformulation someone knowing subject would use; make rerunning query w/ different framing one tap.
- Avoid: suggestion lists only elaborating phrasing already typed → narrow search w/ every accepted suggestion.
- Why: Empowering. Words someone supplies = first + strongest filter on info they receive. Loaded vs neutral phrasings of one subject return different worlds of results. Query-framing skill varies enormously between people.
- Evidence: study of school students searching contested topic: students ending up sealed off = those whose existing view shaped terms they typed; search skill mattered more than ranking.
- Misreading: Wrong: people found what they asked for → results neutral. Right: finding what one asked for = not proof of neutral results.
- Usability of query entry, suggestions + results: search-and-results.md; this pattern bounds it.
- Hypothetical: university library's research assistant, after student types "why remote work fails", highlights which of those words each source matched + offers labour researcher's phrasing as one-tap rerun.

## Escalation, sensitive states and news

### How to keep ranking from becoming a rabbit hole?
- Do: add diversity + serendipity; monitor drift toward extreme content + interrupt it; weight momentary impulses less than long-run interests.
- Avoid: ranking for raw engagement → structurally amplifies anger, fear + us-versus-them material.
- Why: Resilient. Optimizing purely for predicted engagement rewards escalation + sameness (rabbit hole).
- Case: feed team shifted ranking toward long-term interests after feed's role in ethnic violence became clear.
- Evidence on ranking's effects on belief + discourse: ../evidence/filter-bubbles-and-polarization.md.
- Hypothetical: home-repair video app notices viewer's queue narrowing to ever riskier wiring stunts → mixes in other topics viewer followed for months + interrupts run w/ choice of new directions.

### Sensitive state signalled: what guardrails?
- When: person signals interest in self-harm, eating disorders, depression or similar.
- Do: dampen recommendation feedback loop; diversify content; cap recommendation depth; surface support resources; assume person possibly young.
- Avoid: engagement alone deciding what distressed person sees next.
- Why: Resilient. Distress inside conversation: ai-and-automated-features.md.
- Evidence: 2023 human-rights report: short-video feed answered minor's curiosity about mental health w/ steadily bleaker suggestions, drifting toward content glamorizing self-injury.
- Caveat: 2023 report gives no figure for how quickly feed drifted → cite it w/o one.
- Hypothetical: music-streaming app, after listener repeatedly searches songs about self-harm, stops chaining similar tracks, mixes in other genres listener plays, shows support line, applies these limits assuming listener possibly teen.

### Which inferred attributes stay out of ranking?
- When: any recommender learning from behaviour; applies hardest for minors.
- Do: write down inferred attributes barred from ranking, retrieval, ad targeting + lookalike building. Bar: mental-health interest, body image + weight, sexuality + gender identity, religion, immigration status, political leaning, any proxy for mood/emotional state. Audit model's feature list against exclusion list at every model change. For minors: hold behavioural profile only for short stated window, auto-expiring; offer control wiping profile + restarting model.
- Avoid: profile built in someone's teens following them into adulthood.
- Misreading: Wrong: data called purpose-bound → problem solved. Right: not whole answer while every inferred trait stays available to ranker.
- Why: Resilient. Evidence on tracking, inference + data misuse: ../evidence/personalization-and-surveillance.md.
- Hypothetical: homework-help app for school pupils deletes each pupil's behaviour-based profile at end of period stated at sign-up; release checklist blocks any model update whose feature list includes barred trait such as inferred religion.

### How to pace breaking news?
- When: ranking news, alerts or trending material, above all where minors in audience.
- Do: news edition w/ beginning + end; repetition of same distressing event held to stated cadence, not re-delivered hourly; delay amplification of fast-moving claim until corroborated + cap forwarding meanwhile; label claims still developing/disputed; correction as prominent + far-reaching as original claim; let people mute topic or single story, not only source.
- Avoid: endless alert stream keeping disaster permanently in front of fourteen-year-old; ranking claim upward because outrage travels fastest; correction reaching only fraction of error's audience.
- Why: Resilient + Finite (pacing breaking news, slowing amplification of unverified claims).
- Hypothetical: regional news app keeps fast-spreading dam-failure claim out of trending list until officials confirm, tags story "developing"; when early report proves wrong, sends correction to every reader of first version.

## Perspectives and social signals

### Showing contrary views: with what context?
- When: surfacing opposing opinions to widen people's perspectives.
- Do: give contrary views designed context: who speaks + what norms apply; remind person of own limited vantage point; pair ranking changes w/ explanations of how feed works.
- Avoid: raw, unlabelled contradictions dropped into feed + expecting open-mindedness.
- Why: Empowering. Abrupt, context-free contrary views breed rigidity rather than openness.
- Hypothetical: book-review site, when showing critical review of reader's favourite novel, labels reviewer long-time crime-fiction critic, notes site's review rules, + adds line noting reader's own ratings shape what they usually see.

### Approval or following?
- When: only way to receive source = public like.
- Do: follow-quietly option; reactions expressing curiosity/ambivalence, not only approval; news gets distinct context w/ own vocabulary + ideally editorial curation.
- Avoid: modelling news outlets as friends + every interaction as affirmation.
- Why: Intentional (approval separated from following; info kept out of friendship metaphor).
- Hypothetical: professional-network app: member can follow industry newsletter w/o public endorsement on profile; "curious" + "unsure" reactions beside "agree".

### Prompted social act: whose voice is it?
- When: product suggests that one person tag, endorse, invite, follow or congratulate another w/ single tap.
- Do: design from what other person will believe; let person's decline stick; when wording/occasion came from system → say so, do not send it in person's voice.
- Avoid: suggestion engine quietly setting rate of putting people under obligation while presenting each prompted act as friend acting freely.
- Why: Transparent + Respectful. Unmarked prompted gesture reads as deliberate choice + carries deliberate choice's social debt, though in fact one-tap answer to suggestion → product, not people, decides how often to stake anyone's social standing.
- Measure: count of social-act prompts = figure team owns + reviews.
- Hypothetical: alumni-network app suggesting congratulations on classmate's new job marks resulting message "suggested by the app" + stops suggesting it once member declines.

## Time and relationship

### What time does personalization cost?
- When: tailoring saves seconds of searching but consumes hours of watching.
- Measure: net time personalization saves.
- Do: natural stopping points when personalized feed starts consuming time rather than saving it.
- Avoid: for-you page tuned only for session length.
- Why: Finite. Stopping points, infinite scroll + autoplay: feeds-scrolling-and-pacing.md.
- Hypothetical: language-learning app compares study time its personalized lesson picks save vs time spent in its suggested-video tab; adds "that's today's set" break once video tab takes more time than it saves.

### Recognize people or target them?
- When: deciding where personalization effort goes.
- Do: invest in relationship touchpoints (post-purchase how-to, feedback requests, check-ins) over deeper behavioural targeting; personalize convenience while keeping information architecture + pricing consistent for everyone.
- Avoid: following someone around web w/ product they already bought; individualized pricing.
- Why: Respectful.
- Hypothetical: furniture retailer shows every visitor same menu layout + prices, but remembers returning customer's delivery address + room measurements to speed next order.

## Related
- ai-and-automated-features.md: generated answers, sources + uncertainty, distress inside conversation, fairness of models ranking people.
- feeds-scrolling-and-pacing.md: stopping points, infinite scroll + autoplay in ranked feeds.
- transparency-and-honesty.md: explaining algorithm + honest controls.
- privacy-data-and-security.md: data minimisation, consent + tracking behind personalization.
- search-and-results.md: usability of query entry, suggestions + results, bounded by question-as-filter.
- ../laws/choice-overload.md: law behind narrowing options; bounded here by discoverable alternatives.
- ../evidence/filter-bubbles-and-polarization.md: evidence on ranking's effects on belief + discourse.
- ../evidence/personalization-and-surveillance.md: evidence on tracking, inference + data misuse.
