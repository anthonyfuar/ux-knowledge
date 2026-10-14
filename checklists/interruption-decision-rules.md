# Interruption decision rules

## Use when
- Deciding whether, how + when product may interrupt person / reviewing existing interruption.
- Covers: send test · urgency → modality table · attention-demand classes · timing · personalization + etiquette rules.
- Stance: every interruption = conversation; time it as considerate person would.

## 1. Send test
Before sending, interruption must pass at least 1:

|Check|Passes when|
|---|---|
|Urgent?|yes|
|Advances person's current task?|yes|
|Concerns something person genuinely cares about?|yes|

- If none apply → do not send; show item in product at next app open.
- Weigh: interruption benefit vs cost of breaking person's task + cost of missed message.
- Why high bar: regaining focus after disruptive interruption takes ~25–45 min.

## 2. Urgency → modality
Urgency = urgency to person.

|Urgency|Means|Modality|
|---|---|---|
|Critical|safety, security, money leaving|status shout: sound + vibration + lock screen; impossible to miss|
|High|someone needs reply now|1 interruptive channel, dismissable, w/ full content|
|Medium|relevant, can wait hours|badge / digest; haptics only if person opted in|
|Low|nice to know|peripheral channels only: in-app inbox, ambient indicator, scheduled digest|

- Never stack all interruption modes on low-urgency message.
- Hypothetical, critical: glucose-monitor app reads dangerously low level; city alert service sends flood evacuation notice for person's street.
- Hypothetical, high: rider's booked carpool driver asks rider for pickup entrance.
- Hypothetical, medium: school portal posts new grade; library notes borrowed book due next week.
- Hypothetical, low: recipe app's new seasonal collection; bank's weekly savings tip.

## 3. Attention demanded
Besides urgency, classify each interruption by attention demanded.

|Class|Person …|
|---|---|
|Full attention|must stop current activity|
|Partial attention|takes message in + carries on|
|Barely any attention|message sits at periphery until person looks at it|

- Only full-attention interruption justifies stacking sound + vibration + screen.
- Companion test: can person keep doing something else while handling interruption?
- Why: spoken sentence from device takes over room + any conversation in it; tone / light / single-tap reply costs a second + leaves both intact.

## 4. Timing
|Situation|Do|
|---|---|
|Quiet hours (default ~10 pm–8 am)|hold every interruption below critical|
|Younger teens, after 9 pm|no interruptions at all|
|Focus, safe / night mode on|hold every interruption below critical|
|Person driving, in meeting, in bright sunlight / noise|shift modality (haptic, larger contrast, tone instead of speech) or defer|
|Person already in app|deliver medium- + low-urgency items there, not as push notifications|

## 5. Adapting to behaviour
|Signal|Do|Avoid|
|---|---|---|
|Person consistently ignores notification category|suggest snoozing it; reduce / stop it automatically|—|
|Person engages w/ notification category|keep it|escalating its cadence|

## 6. Asking for permission
- Ask in context, not at setup: offer notification when its value clear.
- Hypothetical: pharmacy app, right after refill request sent, offers alert for when order ready to collect.
- Avoid wall of notification toggles on first launch.
- If in-context + setup requests compete → context wins.
- Setup may ask only for essential alerts (1–2; product cannot do its stated job w/o them) → ask each singly.
- At setup, tell person where remaining notification controls live.
- Every other permission request → leave to situation justifying it.

## 7. Controls + etiquette
- Controls → per-sender, per-category + per-channel, global mute + one-click night mode; ensure people know they exist.
- Signals → whisper, not shout: soft tones, gradual transitions, warm indicator colours. Alarm-style signals only for stakes warranting them.
- Read receipts, presence + 'seen' indicators → opt-in for observed person.
- Delivery → asynchronous by default; instant interruption = exception recipient opts into.
- Speech → communicate w/o speech where possible. Why: tone / light needs no translation + does not break conversation.
- Cost → show before click: reading time, step count, scope.

## Related
- ../patterns/notifications-and-interruptions.md: when / do / avoid entries: what interrupts, when, through what channel + under whose control.
- ../patterns/calm-technology-and-device-etiquette.md: peripheral attention, quiet signalling, failing gracefully.
- ../principles/respectful.md: humane principle on well-being, attention + time behind these rules.
- [Attention and distraction evidence](../evidence/attention-and-distraction.md): interruption cost, phone checking + notification load.
- calm-technology-scorecard.md: scores notifications + indicators beside 4 other categories.
- humane-design-audit.md: yes/no questions per humane principle + AI and automation.
- ../ethics/attention-hijacks.md: levers taking attention against person's interest + counter to each.
- ../laws/selective-attention.md: usability-side law on attention.
