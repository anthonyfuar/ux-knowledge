# Forms and data entry

## Scope + laws behind these patterns
- Use for: usability patterns: fields · formats · defaults · validation timing · checkout · payment failure · accessible errors.
- Applies when: designing/reviewing any form, sign-up, checkout, payment or data-entry flow.
- Laws underneath:
  - ../laws/teslers-law.md: pre-filling moves complexity to builders.
  - ../laws/parkinsons-law.md: autofill → finish faster than expected.
  - ../laws/hicks-law.md: fewer choices per screen + per control.
  - ../laws/cognitive-load.md.
  - ../laws/working-memory.md: holding codes while typing.
  - ../laws/chunking.md: grouping formatted strings.
  - ../laws/postels-law.md: liberal input formats.
  - ../laws/jakobs-law.md: conventional controls.

## Less to enter

### Value already known or inferable: make people type it?
- When: field's value already known to system or system can infer it.
- Do: prefill whatever system holds; propose probable values from contacts + past activity; one action copies earlier entry.
- Avoid: people re-typing what system has.
- Why: Tesler's Law: pre-filling doesn't erase complexity; builders now hold it, where it belongs.
- Hypothetical: clinic booking form fills patient name + insurer from profile, suggests usual doctor from visit history + offers "same contact details as last visit".

### Purchase, booking or data-gated flow: how fast should it feel?
- When: purchases, bookings, flows gated by essential data.
- Do: autofill + stored details → task done faster than users expect (Parkinson's Law). Benchmark = user's expectation, not raw speed.
- Avoid: flows w/ slack letting task balloon.
- Hypothetical: hotel app keeps guest's ID details + room preferences from first stay; next booking asks only dates.
- Hypothetical: prescription refill: insurer + delivery address already on file → patient only checks medicine name + quantity before confirming.

### Most users pick the same value: default it?
- When: most users pick same value.
- Do: baseline = sensible default user can change.
- Avoid: forcing user to decide what system could reasonably decide.
- Term: anticipatory design = product predicts + decides for user; far end of range of help forms can give.
- Humane bound: no preselection on consent or money → defaults-and-choice-architecture.md.
- Hypothetical: library renewal form defaults loan extension to standard period, editable in same field.

### Paid add-on at checkout: on or off?
- When: insurance, protection plans, donations, any paid extra at checkout.
- Do: paid add-ons unchecked; added only by user's choice.
- Avoid: pre-adding/pre-checking paid items (sneaking + preselection deceptive patterns).
- Why: pre-adding violates cart model: only shopper decides cart contents.
- Case: luggage retailer defaulted $8.25 shipping-protection toggle to on.
- Hypothetical: concert-ticket checkout lists refund protection as unticked option, price beside it.

### Novice facing setup or creation: blank page or partly done?
- When: novice setup, configuration, creation tasks.
- Do: novices start from worked example, template or partly completed state w/ editable defaults user finishes.
- Why: worked-example effect + completion-problem effect explain benefit to novices. Empty form/canvas → novices pushed into trial + error eating much of their mental capacity.
- Caveat: experts need way to skip scaffold (expertise reversal effect).
- Hypothetical: small-business invoicing tool opens first invoice pre-laid-out w/ sample line + editable payment terms; "start blank" link for experienced users.

## Structure, formats + controls

### Long or complex form: one screen or steps?
- When: long or complex forms.
- Do: split across several screens, each w/ fewer choices + less mental effort; options in each select/radio set at minimum (Hick's Law).
- Avoid: one screen w/ every field + option.
- Hypothetical: visa application split into travel, identity, documents + review screens.

### Codes + long strings: how to display + accept them?
- When: phone numbers, codes, long strings, especially ones copied between places (licence keys, vouchers, account IDs).
- Do: fixed groups w/ visible delimiters, e.g. 25-character key as five groups of five. Accept pastes w/ or w/o separators.
- Avoid: unbroken digit strings; making people hold code in mind while typing different digits.
- Why: Chunking: grouped strings → glance, hold one group, type it, repeat. Working Memory: similar material interferes most w/ material held in mind.
- Hypothetical: home router label prints setup key in short dash-separated groups; setup page accepts key pasted w/ or w/o dashes.

### Money, dates, phones, addresses: how many fields, which formats?
- When: structured values: money, dates, phone numbers, addresses.
- Do:
  - Conservative field count + liberal formats (Postel's Law).
  - Money: accept "$10.00" or "10", normalise on server.
  - Dates: parse "Thu", "tomorrow", "11 April" + dates w/o leading zeros; calendar picker for hard-to-name dates (e.g. second Tuesday of next February).
  - Show examples of most reliable input format, since parsers have limits.
  - Before splitting value into many fields → ask what detail business needs.
- Avoid: blocking keystrokes or showing alerts for input w/ clear meaning; lecturing on format up front, then scolding.
- Hypothetical: hospital registration team plans separate first, middle + last name boxes; asking what hospital needs → one full-name field + one preferred-name field.
- Hypothetical: parcel-delivery form takes "where to leave it" as one text box; courier's system later sorts it into location + access notes.

### Which controls + where does the primary action go?
- When: choosing toggles, radios, checkboxes, buttons.
- Do: standard form controls (Jakob's Law, ../laws/mental-model.md); primary action directly below last input, where finger/pointer already rests; group controls used in sequence (../laws/fittss-law.md).
- Avoid: Save in top header, far from final field; Cancel + Submit side by side, since misses always happen.
- Origin: standard controls' look derives from familiar physical control panels.
- Hypothetical: expense-claim form: "submit claim" under last receipt field; "discard" apart as text link.

## Validation + errors

### When to validate a field?
- When: any validated field.
- Do: validate when person leaves field or submits, not every keystroke. Once field showed error → re-check while typing; error clears once fixed. On submit → focus first error or linked error summary. Valid-field confirmation quiet.
- Avoid: flagging email invalid after first character; clearing field w/ error; red error persisting after input fixed.
- Why: mid-typing error interrupts task attention (../laws/selective-attention.md) + adds message to hold in mind (Cognitive Load). Fits usability heuristics of error prevention + helping users recognise + recover from errors.
- Hypothetical: pension-portal tax-ID field silent while member types; on leaving shows one error, gone once ID valid.

### Leniently parsed value w/ real consequences: act on it directly?
- When: leniently parsed value has real consequences, e.g. donation or payment amount.
- Do: show interpreted value + ask confirmation, even when within normal range.
- Avoid: silently stripping text to number + acting on it: result surprising + costly.
- Hypothetical: like pharmacist reading dose back before handing over medicine, utility-payment form shows "paying [amount] to account ending [digits]: confirm?" before charging.

### Required fields still empty: disable submit?
- When: required fields still unfilled.
- Do: submit stays active; on tap show every problem at once, focus first invalid field or error summary, keep all input. Disable submit only while submission in flight, w/ visible pending state.
- Avoid: disabled submit w/ no reason: users cannot identify missing input.
- Why: many disabled buttons fail contrast + get skipped by screen readers.
- Hypothetical: job-application form w/ empty references field still lets candidate press "send"; jumps to references + names missing items beside them, every other entry kept.

### How to show errors accessibly?
- When: any form error.
- Do:
  - Each error tied to its field: visible text beside it, also programmatically associated.
  - Announce via polite live region, or move focus to linked error summary at top.
  - Problem + fix stated in words, not red colour alone.
  - Error text ≥ 4.5:1 contrast.
  - Layout intact at 200% text size + w/ platform text scaling (Dynamic Type, Android font scale).
- Avoid: placeholder as field's only label; errors shown only by red border; error toasts vanishing before screen reader or slow reader reaches them.
- Hypothetical: council permit form shows "Enter the date in the future: permits cannot start in the past" under date field, read out by screen reader when focus lands.

## Checkout, sign-up + payment

### Checkout + sign-up: which fields + consents?
- When: guest checkout, sign-up, payment details.
- Do:
  - Guest checkout asks email (or phone) early + says why: receipt + order status.
  - Mark optional fields "(optional)", not starring required ones.
  - Drop checkout fields business does not use.
  - Card-storage consent via unchecked "Save card for next time" box; saved cards first only for opted-in users.
  - Support wallets + autofill w/ correct input types + autocomplete attributes.
  - Order total, delivery cost + delivery date shown before final button.
  - Final button names action + amount, e.g. "Pay $42.00".
- Avoid: forced account creation before payment; phone number asked w/ no stated reason; pre-checked marketing or card-saving consent.
- Humane bound: state why data needed beside request; drop fields you cannot justify → privacy-data-and-security.md.
- Hypothetical: garden-centre checkout asks email "for your receipt + delivery updates", shows total + delivery day above "Pay [amount]", "save card" unticked.

### Payment declines, times out or needs bank approval: what then?
- When: any card or wallet payment; failure paths need deliberate design.
- Do:
  - Idempotent submission: one request key per attempt → retry or double tap cannot charge twice.
  - Disable pay button only while request in flight, w/ pending label.
  - Bank verification (3-D Secure, in-app bank approval) = part of flow; tell person it may appear.
  - User leaves for bank app → keep order state + return them to same step.
  - Card decline → keep all fields, clear only security code; plain-words reason when processor provides one; offer another payment method.
  - Payment timeout → check order status before offering retry.
- Avoid: wiping form after decline; generic "Something went wrong" w/ no next step; retry prompt when first charge may have gone through.
- Misreading: Wrong: double-submit protection = application of Doherty Threshold → Right: = error prevention + system design.
- Hypothetical: furniture-store payment times out; page checks order status, finds it paid → shows confirmation, not "try again" button.

## Related
- errors-and-input-tolerance.md: error prevention + recovery, tolerant input, limits stated at input, destructive actions.
- calls-to-action-and-touch-targets.md: size, spacing + placement of Submit + other form buttons; disabling w/ reason.
- progress-goals-and-completion.md: progress indicators + completion for multi-step forms.
- defaults-and-choice-architecture.md: humane bound on defaults: opt-in not opt-out, no preselection on consent or money decisions.
- privacy-data-and-security.md: humane bound on fields: say why data needed beside request, drop fields you cannot justify.
- friction-undo-and-confirmation.md: explicit confirmation before purchases; timeouts warning before discarding half-completed form.
- inclusive-and-accessible-design.md: accessibility floors, labelled fields, name + identity fields fitting real people.
- ../ethics/deceptive-patterns.md: sneak into basket + hidden costs, named patterns behind pre-added extras + late fees.
- ../laws/teslers-law.md · ../laws/parkinsons-law.md · ../laws/postels-law.md: pre-filling, speed vs expectation, liberal formats.
- ../laws/chunking.md · ../laws/working-memory.md: grouped codes, interference.
- ../laws/hicks-law.md · ../laws/jakobs-law.md: fewer choices, conventional controls.
