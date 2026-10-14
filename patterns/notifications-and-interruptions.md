# Notifications and interruptions

## Scope + principles behind these patterns
- Use for: humane patterns: what may interrupt person · when · on what channel · controlled by whom.
- Applies when: designing/reviewing push, sound, badge, email, digest, read-receipt, presence or prompt behavior.
- Principles underneath:
  - ../principles/respectful.md: every entry serves it.
  - ../principles/intentional.md: notifications off by default; sender's way not to interrupt.
  - ../principles/inclusive.md: budgeting against most interruption-sensitive person.
  - ../principles/finite.md: sleep protection.

### Event could trigger a push, sound, badge or email: which channel?
- When: whenever event could trigger push, sound, badge or email (let urgency set delivery).
- Do: classify notification events by importance. Interruptive delivery (sound, vibration, lock screen) only for time-sensitive events. Everything not time-sensitive → passive delivery: badge, in-app inbox or digest.
- Avoid: likes, follows + promotions on same buzzing channel as message needing reply.
- Why: ../principles/respectful.md.
- Hypothetical: home-security app sounds alert for forced door; firmware release notes wait silently in its inbox.

### Send this notification at all?
- When: deciding whether to send at all (interrupt-only-if test).
- Do: interrupt only if message urgent, advances person's task, or matters to person; any one of three enough. None holds → do not send.
- Avoid: engagement pings dressed up as urgency.
- Evidence: regaining focus after broken concentration takes ~25-45 min → weigh against cost of missed message.
- Why: ../principles/respectful.md.
- Hypothetical: banking app never buzzes to announce new card design, but does for payment awaiting person's approval.

### How loud and how often may anything interrupt?
- When: deciding what may interrupt, how loudly + how often (budget against most interruption-sensitive person).
- Do: set interruption threshold by people paying most. Recruit testers self-described as easily derailed.
- Avoid: judging alert by how unhurried designer finds it on quiet afternoon. Single on/off switch forcing everything or nothing.
- Why: interruption cost uneven, not average: pop-up one person shrugs off costs another their whole remaining day. People w/ attention or sensory differences, second-language readers, people in pain + people already anxious pay most. ../principles/respectful.md + ../principles/inclusive.md.
- Hypothetical: hospital ward paging tool sets alert loudness + repeat rate from trials w/ nurses saying they derail easily, not from product team's own reaction at quiet desk.

### Message or comment arrives on an opted-in channel: tease or show it?
- When: messages + comments reach someone via email/push channel they opted into (full content in notification).
- Do: whole message body inside notification → nobody has to launch app to read it.
- Avoid: "someone replied, tap to view" teasers engineered to force return visit.
- Why: ../principles/respectful.md.
- Hypothetical: courier's push "Left your parcel in the side porch" shows in full on lock screen, readable w/o opening app.

### Update is nice to know but not time-sensitive?
- When: updates nice to know, not time-sensitive (let low-urgency information wait).
- Do: show in feed/inbox on person's next open. Batch rest into scheduled digest at time person chooses.
- Avoid: pushing followed-account activity into someone's day.
- Why: ../principles/respectful.md; digests + badges inside product in feeds-scrolling-and-pacing.md.
- Hypothetical: hiking-club app shows new trail reports in feed on member's next open + gathers route-change notices into Sunday-morning summary member scheduled.

### Tempted to add a modal for ratings, installs or sign-in?
- When: tempted to add modal serving business, not person (do not nag).
- Do: show content person requested. Ask for review, if ever, only after completed positive task + never twice.
- Avoid: rating prompts on first use. App-install banners blocking content. Forcing sign-in before someone can read content.
- Why: ../principles/respectful.md.
- Hypothetical: train-ticket app asks for rating once, right after refund goes through smoothly; never on first launch + never second time.

### Onboarding, or adding a new notification type?
- When: during onboarding + whenever new notification type added (notifications off by default).
- Do: ship notifications disabled except crucial few essential to product purpose. Setup earns only 1-2 alerts w/o which product cannot do job person signed up for; ask for those singly + say where remaining controls live. Request each other type when its value visible, not as wall of toggles on first launch. Every other permission waits for situation making it worth granting. Every alert dismissable on first appearance.
- Avoid: all-on defaults w/ buried opt-out. Repeated prompting to enable.
- Why: permission moments compete w/ each other → ask for each in context. ../principles/respectful.md + ../principles/intentional.md.
- Case: one messaging app prompted people to enable notifications four separate times.
- Hypothetical: language-learning app asks for practice reminder only after learner picks study time, + names where other alert settings live.

### Two or more notification sources: who sets manner, timing, sender?
- When: ≥2 notification sources (recipient sets manner, timing + sender).
- Do: per-sender, per-category, per-channel + quiet-hours controls. Let people switch sound to haptic, or off. Ensure people know controls exist.
- Avoid: single global notification switch. Settings so deep people either endure everything or disable everything.
- Why: ../principles/respectful.md.
- Hypothetical: ride-share driver app lets drivers turn trip-request sounds into vibration while carrying passengers + set quiet hours for promotional messages, w/ pointer to these controls on first alert.

### Person needs silence now?
- When: person needs silence now (global mute, safe mode, one-tap night mode).
- Do: one control silencing everything. No-interruptions mode. Scheduled quiet hours. Protect late-night rest by default.
- Avoid: making people silence each app/category one by one. Promotional pushes at midnight.
- Case: one video app silences sounds + vibrations 10pm–8am by default.
- Case: one short-video service sends no push notifications after 9pm to 13-to-15-year-olds.
- Why: ../principles/respectful.md; sleep protection = ../principles/finite.md.
- Hypothetical: e-reader tablet w/ one "silence everything" tile + bedtime schedule switched on by default.

### A notification type is consistently ignored?
- When: notification type consistently ignored (adapt to observed behavior).
- Do: treat every interaction w/ notification as part of conversation. Reduce/change alerts nobody opens. Suggest snoozing routinely dismissed categories.
- Avoid: escalating cadence when engagement drops, e.g. five recommendation emails in one week to someone having opened none.
- Why: ../principles/respectful.md.
- Hypothetical: public-library app sees "new arrivals" emails unopened for months → asks whether to replace them w/ in-app list.

### Product can sense time, activity, motion, light or connectivity?
- When: product can sense time, activity, motion, light or connectivity (adapt to context).
- Do: hold notifications back during meetings, driving, sleep + focused work. Change delivery form to fit situation, as polite person reads the room. Time interruptions from signals already held or cheap to read: what screen open, whether keys moving, whether device in motion, hour on person's own clock. No usable context signal → send less rather than sense more; item waits for next open.
- Avoid: identical interruptions regardless of situation. Voice assistant answering in full sentences during meeting. Assuming more data → better-timed interruptions (wrong; use coarsest working signal).
- Bounds: guard context signals used for timing against reuse for targeting. Never justify location history, always-on microphone or behavioral profile as courtesy for better-timed notifications. Nobody should face closer watching as price of fewer interruptions.
- Why: person's location, known roughly, + what goes on around them usually times alert well, w/o inferring their identity. ../principles/respectful.md.
- Hypothetical: smart-home hub holds "replace the air filter" notice while keys moving on linked laptop, + switches from spoken message to soft light ring after household's bedtime hour.

### Designing messaging, read receipts or presence?
- When: designing messaging, read receipts, online status or "seen" indicators (asynchronous delivery + opt-in presence).
- Do: disclosure signals such as read receipts + online status = opt-in toggles. Prefer inboxes + digests to pop-overs for messages between people. Instant interruption = exception recipient chooses.
- Avoid: forced read receipts → heighten urgency + obligation. Features revealing where recipient opened message w/ no recipient opt-out.
- Case: one email client reversed its location-revealing read receipts after backlash.
- Why: ../principles/respectful.md.
- Hypothetical: tenant-landlord messaging portal: "seen" markers stay off unless tenant switches them on.

### Messages cross into someone else's evening or night?
- When: product carries messages between people, so one person's working hours land in another's evening, weekend or night shift (give sender way not to interrupt).
- Do: compose-now-deliver-later = first-class control beside send. Propose delivery time inside recipient's ordinary waking/working hours. Let people publish away/slow-to-reply status. One control pausing whole context (work account + everything notifying from it) on schedule, not app by app.
- Avoid: design where only considerate path = remembering at midnight to sit on message until morning. Treating quiet hours as recipient's problem alone.
- Why: ../principles/respectful.md + ../principles/intentional.md.
- Hypothetical: school staff-messaging tool suggests delivery at start of colleague's next school day; part-time teacher posts "in Tue–Thu, replies then" as status.

## Related
- ../checklists/interruption-decision-rules.md: rules for urgency, modality, timing + etiquette of any interruption.
- calm-technology-and-device-etiquette.md: peripheral attention + quiet signalling for what need not interrupt.
- feeds-scrolling-and-pacing.md: digests, badges + stopping points once person inside product.
- ../ethics/attention-hijacks.md: levers taking attention against person's interest + counter to each.
- ../evidence/attention-and-distraction.md: evidence on interruption cost, phone checking, notification load.
- ../principles/respectful.md: principle every notification entry serves.
- ../laws/selective-attention.md: usability-side law on attention; read alongside when judging what may interrupt.
- onboarding-and-first-use.md: usability side of first-run prompts + re-engagement nudges.
