# Feeds, scrolling and pacing

## Scope + principles behind these patterns
- Use for: humane patterns on stopping points · infinite scroll vs load more · autoplay · variable rewards · session length.
- Applies when: designing/reviewing any feed, continuously loading list, media queue or short-form stream.
- Principles underneath:
  - ../principles/finite.md: underlies feeds patterns; most of them serve it.
  - ../principles/intentional.md: moderation prompts after extended use.
  - ../principles/transparent.md: effort + scope made estimable.
  - ../principles/empowering.md: direct path to person's goal.
  - ../principles/resilient.md: for minors in short-form media.

### Everything new has been seen: show an end?
- When: any chronological or ranked feed.
- Do: all new seen → clear "all caught up" marker (stopping = fine). Scroll position kept on return.
- Avoid: silently looping/backfilling older + recommended content so feed never ends; reset to top after opening item.
- Why: Finite.
- Hypothetical: school-parent app: after last unread class update, inline divider: nothing else new; no older items load below; back from opened update → same spot.

### List would auto-load near the bottom: load more or keep loading?
- When: list would auto-load as person nears bottom.
- Do: each chunk ends w/ explicit "load more" control; show how many seen of total; people choose how many load at a time.
- Avoid: infinite scroll default on every list because it lifts engagement numbers.
- Why: Finite ("load more" instead of infinite scroll).
- Hypothetical: job board ends each match batch w/ "show more jobs" button + count of jobs seen out of all matches; selector sets batch size.

### Infinite scroll or pagination?
- When: choosing how long list loads.
- Do:
  - Infinite scroll only for aimless browsing of homogeneous content.
  - Pagination where people search, compare items far apart in list, or scan top results.
  - If continuous loading kept → page landmarks, reachable footer, proper feed role for screen readers, skip link for keyboard users.
- Avoid: endless scroll on catalogs, search results + task lists; false impression of complete list, from white space or ad sitting above not-yet-loaded content.
- Why: Finite (infinite scroll only for aimless browsing).
- Hypothetical: university course search paginates results → student can weigh course near top against one far down.
- Hypothetical: home-decor inspiration board (aimless browsing of similar images) keeps loading, but each batch gets heading landmark, footer stays reachable + skip link jumps past board.

### Video, episode or track ends: autoplay or "up next"?
- When: video, episode or track ends.
- Do: show what's next; only deliberate tap starts it. Ship autoplay off, especially for minors. Autoplay exists → periodic "still watching?" check + easy toggle.
- Avoid: countdown timers starting next item unless person intervenes.
- Why: Finite ("up next" instead of autoplay).
- Case: video service turned autoplay off for under-18s.
- Hypothetical: language-course app: lesson video ends → next lesson's title + "start" button; nothing plays by itself.

### Session runs long: step in?
- When: sessions run long, especially w/ binge-prone media.
- Do: after extended use, ask if person wants to continue. Offer session intent ("how long do you have?") + end session there.
- Avoid: silently continuing indefinitely; willpower as only way out.
- Why: Finite + Intentional (moderation prompt after extended use).
- Hypothetical: online chess site, after long run of back-to-back games, asks: start another or stop for now, both equal buttons.
- Hypothetical: museum-guide app asks visitor how long they have, builds tour ending at that time.

### Ordinary action yields an unpredictable payoff: how to deliver new items?
- When: action (pull to refresh, badge tap, swipe) yields unpredictable payoff.
- Do: batch new items + deliver at predictable times user chooses. Measure value delivered, not checks per day.
- Avoid: slot-machine mechanics; fake/inflated badge counts; withholding likes to release when re-opening app most likely.
- Why: Finite (variable rewards → predictable delivery). Variable-reward loop needs no author: nobody set out to turn inbox, badge or pull to refresh into slot machine. Nobody earns from checks turning up nothing, yet loop still forms. Unpredictable payoff after ordinary action → same compulsion whether or not anyone intended it.
- Review question: never ask about intent behind possible hook; ask only whether payoff schedule unpredictable.
- Hypothetical: hospital-ward team-chat tool delivers non-urgent channel updates in one batch at shift-change times each nurse picks, not one by one as they arrive.

### Genuine updates run out: pad the feed or stop?
- When: genuine updates run out.
- Do: show handful of updates from people person interacted w/ → declare them caught up. Little high-value content over large volume.
- Avoid: padding feed w/ suggested/recycled content to extend sessions.
- Why: Finite (meaningful over voluminous).
- Hypothetical: family photo-sharing app shows few new photos from relatives person exchanges with, then: everything new seen; no suggested albums appended.

### No cue of how long a flow or feed takes: make effort estimable?
- When: flow or feed gives no cue of how long it takes.
- Do: before commitment state steps, documents needed, estimated reading time or items remaining. People open product on own initiative, not summoned by it.
- Avoid: "Get started" button hiding twelve-step form; one-star rating tap opening three-page survey.
- Why: Transparent.
- Hypothetical: passport-renewal service lists required documents + step count on start page.
- Hypothetical: online course unit shows how many lessons remain beside play button.

### Every intent routed through the feed: give a direct path?
- When: every intent (posting, checking event, signing in elsewhere) routed through feed.
- Do: dedicated routes to common intents, bypassing feed + notification centre.
- Avoid: bundling person's visit reason w/ business's, like store hiding milk at back.
- Why: Empowering.
- Hypothetical: club-membership app links straight to "book a court" from home screen icon + reminder email, w/o passing through member news.

### Short-video or rapid-reward feed: protect attention + sleep how?
- When: building/ranking short-video or similar rapid-reward feeds.
- Do: research linking heavy short-form use to reduced attention, anxiety + stress = design constraints. Build breaks, time limits + friction for long sessions into feed. Break + bedtime reminders on by default for teens.
- Avoid: ignoring session length because long sessions look good in metrics.
- Why: Finite; Resilient for minors.
- Evidence: research links heavy short-form media use to reduced attention, anxiety + stress.
- Case: break reminders on by default for 13-to-17-year-olds in short-video feed.
- Hypothetical: hobby-community short-video app pauses feed after long session w/ "take a break" screen; teen account: bedtime reminder already on.

## Related
- ../principles/finite.md: principle most feeds patterns serve.
- recommendations-and-personalization.md: algorithmically ranked feeds, steering controls, rabbit holes.
- habits-streaks-and-gamification.md: streaks, counters + rewards; neighbouring reward mechanics.
- notifications-and-interruptions.md: badges, digests + what may summon person back.
- ../ethics/attention-hijacks.md: levers taking attention against person's interest + counter to each.
- ../evidence/addiction-and-variable-rewards.md: evidence on compulsion loops, variable rewards, time lost.
- ../evidence/children-and-adolescents.md: evidence on effects on minors + age-appropriate design.
- search-and-results.md: usability side: results layout, filters + zero results for searched lists.
- feedback-loading-and-performance.md: auto-advance only in work queues; consumption feeds end on stopping point.
