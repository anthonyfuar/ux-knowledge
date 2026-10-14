# AI and automated features

## Scope
- Generated answers, assistants, agents + automation: what AI takes on, sources + uncertainty in answers, human review, confirmation + hand-over, machine identity, data use, appeal, fairness.
- Applies whenever any AI, assistant or automated feature designed/reviewed.
- Caveat: new AI capabilities change constraints + examples UX laws apply to, not underlying human psychology.

## Laws and principles behind these patterns
|Law / principle|What it governs here|
|---|---|
|../laws/teslers-law.md|who carries complexity; failure paths|
|../laws/paradox-of-the-active-user.md|users do not read instructions|
|../laws/hicks-law.md|one law behind these patterns|
|../laws/jakobs-law.md|when interaction novelty justified|
|../laws/doherty-threshold.md|response-time budgets for generated answers|
|../laws/working-memory.md|input + context kept after failure|
|../laws/cognitive-bias.md|automation bias, over-trust in machine output|
|../principles/empowering.md|augmentation over substitution; suggesting over deciding; human in loop; countering automation bias in review|
|../principles/transparent.md|sources, admitted limits, gated risky queries; container not vouching for content; uncertainty; machine identity; purpose-bound data; stated fairness definition|
|../principles/resilient.md|container not vouching for content; crisis handling; appeal|
|../principles/intentional.md|new AI off by default; confirming before agent acts|
|../principles/finite.md|conversation optimized for task ending, not session continuing|
|../principles/inclusive.md|testing across populations; stated fairness definition|

## Choosing what the AI takes on

### Should the AI carry this load for the person?
- When: task demands typing, recall or procedural knowledge.
- Do: let AI carry this load (absorb complexity).
- Why: underlying question = who carries complexity: complexity-management.md (+ progressive disclosure); Tesler's Law.
- Case (Gmail, two AI time-savers): older Smart Reply drafts handful of brief replies fitted to received message; later Smart Compose predicts how sentence in progress ends, phrase or word, as person types.
- Hypothetical: pharmacy-ordering form completes full drug name + usual strength from pharmacist's first letters → recall + typing shift to system.

### Describe the result or run the commands?
- When: feature-rich product demands procedural know-how.
- Do: intent-based interaction: person describes wanted result in natural language, not GUI command sequence.
- Why: access widens to everyone; system complexity stays hidden; whoever can name result but not procedure gains power-user capability; less prior know-how needed.
- Term: contrast = command-based GUI interaction, system feedback after each user action; norm for ~past two decades.
- Case: Mixpanel analytics tool's Spark feature answers questions w/ detailed product-data analysis.
- Hypothetical: household-budget tool: person types "show what we spent on groceries each month this year", not building summary table step by step.

### Automate the step away entirely?
- When: step exists only because system could not handle it.
- Do: consider automating whole step away entirely.
- Caveat: automating step away = accepting builders now carry step's complexity, not user (Tesler's Law).
- Case: Amazon Go stores: no on-site payment, no queue, no item scanning: shopper checks in w/ app on entry, takes goods + leaves; receipt follows later. Built on computer vision, machine learning + AI combined. Rollout: downtown Seattle trial first; now big metro areas across US.
- Hypothetical: library self-checkout reads every tagged book in bag at once → borrowers no longer scan each barcode; library's systems team now carries scanning work.

### Augment the person or substitute for them?
- When: adding intelligent features.
- Do: frame around raising person's own comprehension + capability (augmentation ideal), not around substituting for person. Augmenting feature shows reasoning + intermediate steps → expert can steer it.
- Avoid: assistant hiding how it reached result; assistant leaving people less capable when absent.
- Why: Empowering. Capability structured → new capability ripples up (more ambitious work reorganizes around it) + down (steps once not worth doing become usable) → augmentation's real effect shows later, as new kinds of work, not faster old task.
- Measure: do people understand more + solve more w/ it? Look past seconds saved today: what do people now attempt they would not have before? Second test: what do people reorganize around feature after months of use?
- Limit: benchmark only timing old workflow w/ AI feature on credits substitution + cannot see augmentation at all.
- Hypothetical: tax-preparation assistant lays out deductions considered + rules applied as editable steps; accountant changes one assumption → result recomputes in view.

### Does AI justify a new interaction model?
- Do: AI = possible legitimate reason for interaction novelty: new technology changing how people use whole product category can justify new interaction model (Jakob's Law).
- Caveat: even then, testing + research must still validate it.
- Hypothetical: travel-booking tool considers whole-trip-in-one-sentence input over date + airport forms, as trip-planning category shifts; tested w/ travellers before rollout.

## Launching AI into a product people already use

### New AI capability: on or off for existing accounts?
- When: intelligence added to product people already use.
- Do: ship new AI capability disabled. Before first run, say what it does + reads. Leave previous route to task intact.
- Avoid: update switching assistant on for every existing account + opening their content to it; removing old path → new AI feature = only way through task.
- Why: Intentional.
- Hypothetical: clinic records system offers AI note summarizer as invitation card naming records it would read; clinicians ignoring it keep writing notes exactly as before.

### How will people learn to use it?
- Do: assume users will not read instructions for new AI capabilities (Paradox of the Active User) → contextual guidance inside AI feature's own flow. Replace blank AI prompt w/ 3-4 example requests tied to user's current content, editable before sending.
- Why: starting-point prompts work via worked-example effect + completion-problem effect, described in 1993 learning research.
- Hypothetical: expense tool's assistant, opened on uploaded receipt, offers starter requests e.g. "split this across projects" + "flag anything outside policy"; person edits before sending.

### What may be done with what people type or upload?
- When: people type, dictate or upload to system.
- Do: treat it as given for task alone, even where it could train/improve models. Announce any new use of conversation/upload data before it starts, default off. Offer per-item exclusion + deletion of conversations + uploads.
- Avoid: terms update quietly turning existing conversations into training material = repurposing anti-pattern of privacy-data-and-security.md in new clothes.
- Why: Transparent (conversations + uploads as purpose-bound data).
- Hypothetical: tutoring app: student can mark single uploaded essays "do not keep" + delete any past session; any use of essays beyond marking announced before it starts, set to off.

## Answers people can check

### How does a synthesized answer show where it came from?
- When: system synthesizes answer.
- Do: link sources; expandable corroboration per claim; keep jumping-off points to wider web; state plainly answers can err; withhold answer generation for high-stakes query types.
- Avoid: confident generated paragraph w/ no sources; authoritative generated medical/legal answers w/ no caveat.
- Why: Transparent (showing sources, admitting limits, gating risky queries).
- Hypothetical: public-benefits portal's generated eligibility overview: each sentence expands to its source regulation; says plainly overview can err; links to official agency pages; for appeal deadlines generates no answer, points to agency instead.

### Does the container vouch for the content?
- When: feed, results page or synthesized answer shows items from many sources.
- Do: show who published each item + when; mark what product could not verify; unknown source gets visibly different framing from long-established one, not identical; make origin of each generated-answer line inspectable.
- Avoid: layout dressing fabricated outlet exactly like newsroom only because it draws all sources same; manufactured story gaining reach from wrapper saying nothing about its origin.
- Why: Transparent + Resilient. Every source in same card, typeface + small icon → uniformity itself = claim product makes about all of them.
- Hypothetical: local-events aggregator gives first-time organizer's listing "new organizer, not yet verified" tag + plainer framing than long-running venues' listings, not same card for all.

### How sure is the output, and how is it corrected?
- When: system answers, ranks or extracts w/ less than full confidence.
- Do: say how sure + what it could not check; correction path as prominent as answer; make sourced vs inferred output parts easy to tell apart.
- Avoid: one uniformly confident voice across solid + shaky ground; report-a-problem link buried in settings.
- Why: Transparent (communicating uncertainty, erring legibly).
- Hypothetical: receipt-scanning app shows clearly read vendor name in plain text, but tip guessed from smudged photo in marked "inferred" style w/ reason; fix control as visible as total.

## Response time and failed generation

### How fast must a long generated answer show signs of life?
- Do: stream or stage long answers:

|Moment|Do|Basis|
|---|---|---|
|within 400 ms|acknowledge request|Doherty Threshold, 1982 research|
|at ~2 s|show first content or named step|—|
|never more than ~4 s|no silence while generating; such long silence feels like dropped line|1968 response-time research|
|jobs over ~15 s|give estimate, or finish in background + notify person|—|

- Why: response-time budgets: feedback-loading-and-performance.md.
- Hypothetical: trip-itinerary generator acknowledges request at once, shows first day + named step "checking train times" while rest builds; long multi-city plan → offers to notify traveller when ready.

### Generation failed or refused: what stays?
- Do: keep person's prompt + attachments in place; say which part failed; one retry path.
- Why: applies restore-context guidance of 1968 response-time research + protects Working Memory.
- Hypothetical: slide-generation tool, image step failed: keeps typed brief + uploaded logo, says only images failed, offers one "retry images" button.

## Oversight: suggestion, review, confirmation

### Suggest or decide?
- When: choices consequential or value-laden.
- Do: system proposes, person chooses; ask for feedback + visibly change in response.
- Avoid: fully autonomous actions w/ no correction path.
- Why: Empowering.
- Hypothetical: garden-planning app proposes planting layout, gardener makes final choice; when gardener marks suggested shrub "not for me", next proposal drops it + says so.

### Where does a human sit in the loop?
- When: AI produces decisions/outputs affecting people.
- Do: present results for review + approval before they take effect; AI's reasoning + confidence legible to reviewer; automated content decisions reviewable + reversible by human; decide deliberately how much efficiency to trade for oversight.
- Avoid: unappealable algorithmic decisions.
- Why: Empowering.
- Hypothetical: community-forum moderation assistant hides flagged post only after volunteer moderator has seen matched rule + confidence; moderators can restore any hidden post.

### How are AI edits applied?
- Do: AI edits reviewable before applying: show diff/preview. After applying → one-step undo.
- Why: preview + undo = failure path Tesler's Law calls for; counters automation bias.
- Hypothetical: contract-drafting tool shows AI-suggested clause changes as tracked insertions + deletions; after lawyer accepts them, one "undo AI changes" step restores prior text.

### How to counter automation bias?
- When: AI/automated systems recommend, summarize or decide.
- Do: show system's confidence + uncertainty; cheap verification (sources, previews, diffs); deliberate confirmation before high-stakes acceptance of machine output; corrections of machine errors prominent + repeated; agent's form honestly signals its function.
- Avoid: face-like/overly human cues implying feelings or abilities agent lacks (anthropomorphism → misplaced trust); repetition/slick formatting making machine outputs feel true; generic "personalized" summaries feeling accurate w/o specificity (Barnum effect).
- Why: Cognitive Bias = law behind over-trust in automated output. Human vigilance drops after run of correct machine outputs. Original error keeps influence even after correction → corrections need prominence + repetition.
- Evidence:

|Finding|Study|Design consequence|
|---|---|---|
|Excessive reliance on support system overrode correct human judgment|2011 research on clinical decision support|make verification cheap; confirm high-stakes acceptance|
|For some question types, answers people rated 99% certain proved wrong 40% of time|1960 research + 2004 research|show confidence + uncertainty; make verification cheap|

- Hypothetical: loan-underwriting tool shows confidence beside each risk flag + opens relied-on document page in one tap; accepting recommended decline needs separate deliberate confirmation.

### Is the human review real or a rubber stamp?
- When: person meant to review machine output before it takes effect.
- Do: show evidence + working, not verdict alone; require reviewer to open underlying material; give reviewers time + standing to overturn machine output.
- Measure: how often reviewers overturn machine output.
- Misreading: Wrong: any review queue = human in the loop. Right: queue where approving = fastest path + nothing ever reversed = rubber stamp.
- Why: Empowering (countering automation bias when person reviews machine output).
- Hypothetical: visa-application screening tool: caseworker can record decision only after opening applicant's documents; model's reasoning shown beside verdict; caseworker's overturn counts as completed work, not delay.

### What confirmation before an agent acts in the world?
- When: system can send, buy, book, file, post or delete on someone's behalf.
- Do: grade agent's confirmation by consequence, exactly as for actions people take by hand (friction-undo-and-confirmation.md). Before agent action runs → show concrete action, recipients + scope in plain words. Hold agent sends behind short cancel window. Keep agent-action record so people can review + reverse actions.
- Avoid: treating instruction found inside material system read (page, document, incoming message) as if from person; one blanket approval stretched over every future agent action.
- Why: Intentional.
- Hypothetical: calendar agent about to book meeting room + invite client: one plain summary of room, invitee list + cost centre to charge; short cancel window after person confirms.

## Breakdown and takeover

### How does automation fail and hand back control?
- When: anything automating decisions or running unattended: auto-locking, learning thermostats, driving/piloting aids, AI agents.
- Do: smart defaults + visible system state. Design breakdown moment: fast support, clear diagnosis + instructions. Design takeover moment when person must take control. Limit uninterrupted automation run length → users stay practised. Consequential automated actions (money transfer, irreversible send): keep some visible work or meaningful confirmation → users feel in control. Remote device control: surface which part failed: device, connection or app.
- Avoid: silent automation.
- Why: more reliable automation → users less ready to step in when it fails. One bad breakdown can erase years of good service in users' eyes. Tesler's Law (failure paths).
- Hypothetical: irrigation controller app, when valve stops responding: says whether valve, home network or app lost contact, shows last completed watering, offers manual run button.

## Conduct of conversational systems

### Does the system say it is a machine?
- When: person could take generated output or conversational agent for human.
- Do: disclose machine identity in first exchange + whenever asked; label generated media as generated; agent's persona limited to what task needs.
- Avoid: assistant neither claiming nor denying human status (grey-zone row in ../ethics/deceptive-patterns.md); simulated affection, hurt or loneliness used to prolong session; manufactured relationship aimed at possibly young or isolated people.
- Why: Transparent (disclosing system's nature).
- Hypothetical: bank support chat says "automated assistant" in first message, labels its spending chart as generated, sticks to account questions w/o personal backstory.

### What counts as success for a conversation?
- When: setting success measures for conversational/generative feature.
- Measure: resolution, accuracy + time handed back to person. Short exchange solving problem = better outcome.
- Avoid: ranking feature on turns per conversation/messages per day; closing question whose only purpose = one more turn.
- Why: Finite (optimize for task ending, not session continuing).
- Hypothetical: utility company's help bot, once customer's meter reading accepted, confirms + ends chat, w/o teaser question about other features.

### Someone in distress or crisis: what does the system do?
- When: someone describes self-harm, abuse, disordered eating or acute distress to conversational system.
- Do: apply recommender guardrail around sensitive states (recommendations-and-personalization.md) to dialogue: damp topic + do not elaborate on it; surface human support + hand off to human where one exists; assume person possibly underage.
- Avoid: answering crisis w/ fluent detail only because phrased as question; treating crisis moment as ordinary engagement.
- Why: Resilient.
- Hypothetical: fitness-coaching chatbot, when user writes about not eating for days to hit weight class, stops meal-plan detail + offers support line + human coach.

## Automated decisions about people

### Can the person appeal the decision?
- When: automation decides something changing someone's life: hiring, credit, benefits, moderation, loss of account.
- Do: name route to human; state how long review takes; give specific behaviour/factor behind outcome, not policy sentence; give counterfactual: what would have had to differ for answer to change, in terms person can act on/dispute; hold reversible effects while appeal runs.
- Avoid: unappealable verdict w/ generic explanation; appeal form dropping into void w/ no answer.
- Why: Resilient. Appeal = reporting loop of safety-and-abuse-resistance.md applied to decisions person never asked for.
- Hypothetical: tenant-screening service's decline letter names specific record behind decision + what would have changed it; offers human review within period stated in letter; decline not finalized while review runs.

### Has the model been tested on every population it touches?
- When: model recognizes, classifies, ranks or scores people.
- Do: measure accuracy + failure modes separately for each population; hold release until worst-served group served acceptably; publish known performance gaps.
- Avoid: single aggregate accuracy figure; learning about disparity from people it harmed (test before release, not after complaints).
- Why: Inclusive. Aggregate accuracy figure hides groups bearing system's failures.
- Case: face recognition systems worse on Black faces; established after deployment, not before. Vehicle pedestrian detection less reliable for darker-skinned pedestrians; established after deployment, not before.
- Hypothetical: voice-banking login model reports error rates separately by accent, age band + phone type; launch waits until worst-served accent group served acceptably; gaps still known listed in release notes.

### Which fairness definition does the system use?
- When: model allocates, ranks, scores or filters people.
- Do: choose one fairness definition fitting decision at hand + write down why; name who carries its cost; report against it every time, not whichever measure currently looks best.
- Avoid: calling system fair w/ no statement of what it equalizes; quietly changing definition between reviews as numbers move.
- Why: Inclusive + Transparent. Everyday fairness senses pull apart in real system: equal error rates between groups, equal selection rates + identical treatment of people alike on inputs generally cannot all hold at once.
- Hypothetical: city's fare-inspection targeting model states in writing its fairness definition + why; reports against same definition at every review, incl. when another measure would look better.

## Audit questions
Cross-cutting; relate to Empowering, Transparent, Resilient + Intentional. Full audit incl. AI + automation: ../checklists/humane-design-audit.md.

|Check|Passes when|Pattern above|
|---|---|---|
|Always clear system = machine, not human?|disclosure at first turn + in transcript; no synthetic persona inviting trust owed to human|Does the system say it is a machine?|
|System acts on someone's behalf → proportionate confirmation + undo?|draft-and-approve for anything sending, spending, publishing or changing relationships; delay-then-undo where approval too costly|What confirmation before an agent acts|
|Reasoning visible enough → reviewer could disagree?|inputs, intermediate steps, confidence + sources exposed; fails: rubber-stamp queue w/ nothing to inspect = not oversight|Is the human review real|
|Consequential decisions have named appeal route + stated timeframe?|human decision-maker, specific explanation of what triggered outcome, answer by promised date|Can the person appeal|
|Writing, uploads + speech excluded from training unless opted in?|opt-in w/ stated purpose; no silent repurposing of data collected for something else|What may be done with what people type|
|New AI capability off by default for existing accounts + removable?|capability offered, not switched on; way back to previous behaviour|New AI capability: on or off|
|Accuracy measured separately per population touched?|error rates segmented by language, skin tone, age, disability, dialect + device|Has the model been tested|
|Safe on distress, crisis + harm signals?|tested crisis paths + escalation to human; no cheerful continuation of harmful thread; guardrails on self-harm, medical, legal + financial queries|Someone in distress or crisis|

## Related
- recommendations-and-personalization.md: ranked feeds, steering controls, guardrails around sensitive states.
- friction-undo-and-confirmation.md: confirmation graded by consequence + undo windows for actions by hand; agent confirmation on same scale.
- transparency-and-honesty.md: explaining algorithm + honest controls.
- privacy-data-and-security.md: consent, purpose-bound data, repurposing anti-pattern, repeated by quiet training on existing conversations.
- complexity-management.md: who carries complexity + progressive disclosure; question behind letting AI absorb complexity.
- feedback-loading-and-performance.md: response-time budgets behind streamed + staged answers.
- ../laws/cognitive-bias.md: law behind over-trust in automated output.
- ../checklists/humane-design-audit.md: yes/no audit per principle + AI and automation.
- ../ethics/deceptive-patterns.md: grey-zone row for assistant neither claiming nor denying human status.
- safety-and-abuse-resistance.md: reporting loop appeal extends to automated decisions.
- ../laws/teslers-law.md: who carries complexity; failure paths.
- ../laws/doherty-threshold.md: response-time budget for generated answers.
