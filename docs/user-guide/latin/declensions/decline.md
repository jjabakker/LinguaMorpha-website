# Decline the Noun

The Decline-the-Noun drill is the production half of the Latin noun coach. The app shows you the lemma (citation form), a case, and a number — your job is to produce the correct inflected form.

<!-- TODO: screenshot when Latin screenshot kit lands -->

---

## How a question looks

A typical question:

> **rōsa, rōsae, f.** — *rose*
>
> Produce the **Dative Plural**.

You type your answer (or pick from multiple-choice options, depending on the mode). Tap **Check** for instant feedback.

A correct answer is marked in green; the next question loads automatically (or on your tap, depending on your Auto-advance setting). An incorrect answer is marked in red and the correct form is shown alongside your answer for comparison.

---

## Type mode vs Pick mode

Same as the Spanish Conjugation Drill, this drill supports two modes that you can switch between at any time using the picker at the top of the screen:

- **Type mode** — the keyboard opens and you type the form. Macrons are not required by default (lenient checking); typing *rosis* when the expected answer is *rosīs* counts as correct with a gentle reminder. Switch to strict mode in **Settings → Strict macrons** if you want vowel length in your muscle memory.
- **Pick mode** — four plausible forms appear as buttons; tap the one you think is correct. The distractors are deliberately near-miss (the same noun in adjacent cases, or the right case in the wrong number) so you have to actually think about the morphology.

Pick mode is what most learners start with; Type mode is what muscle memory ultimately needs. Both feed the same adaptive engine.

---

## Vocative handling

The drill does **not** ask for the vocative when the vocative is identical to the nominative — which is most nouns. For the small set where vocative ≠ nominative (second-declension *-us* and *-ius* nouns), the drill includes the vocative as a separate question. The case label in the question card always says exactly which case is being asked, including the vocative.

---

## Locative handling

Latin's surviving locative shows up for a tiny set of nouns — city names (*Rōmae*, *Athēnīs*), small islands, and a few common nouns (*domī*, *humī*, *rūrī*, *bellī*, *mīlitiae*). The drill includes the locative case **only** for the nouns where it's attested. For everything else, the locative is suppressed.

---

## Macron handling

By default the answer-check is **lenient** on macrons. Macrons matter for classical scholarship and for understanding meter, but they're not part of standard manuscript spelling, and forcing them on every drill answer turns vocabulary work into typing practice. The lenient check counts *rosis* as right when *rosīs* is correct, but flags the missing macrons with a gentle "Don't forget the macron on the *i*" reminder.

If you want strict macron-accuracy in your drilling, flip the switch in **Settings → Strict macrons**. Strict mode counts *rosis* as wrong; the macron drill in v1.5 will add a dedicated drill for the macron skill itself.

See the [Macrons page](../macrons/) for a full explanation of macron handling and how to type macrons on iOS.

---

## What's recorded

Every answer (correct, incorrect, or skip) is recorded in the device's local SQLite database. The adaptive engine uses this history to:

- Promote weak nouns (low correct rate) to the top of the next session.
- Demote strong nouns once you've consistently produced their forms correctly.
- Schedule unseen nouns ahead of already-seen ones, ordered by CEFR + frequency.

Latin-side performance tracking is partially wired in v1.0 — drills work, scores are recorded, but the full adaptive scheduling for Latin lands in a follow-up release. Spanish-side adaptation is already fully wired.

---

## Recommended workflow

1. Start in **Pick mode** so the drill feels welcoming. Get a session or two of green ticks under your belt before switching.
2. Switch to **Type mode** once you can pick reliably. Pick mode lets you eliminate; Type mode forces recall.
3. Run **strict macrons** off for the first month, then on once the forms are solid. The macron skill is its own muscle.
4. Pair this drill with **Recognise the Form** in alternating sessions — production and recognition reinforce different parts of the same morphology.
