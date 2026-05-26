---
description: LinguaMorpha features — Latin morphology with all five declensions, adjective patterns, sentence parser, and concordance drills, plus Spanish as the first additional module with verb conjugation, noun gender / plural, phrases, and adaptive sessions.
---

# Features

LinguaMorpha is a Latin-based language platform. The flagship is **Latin** — every declension, every adjective pattern, comparative and superlative, macron-accurate checking, plus a sentence parser that handles arbitrary Latin text. The first additional module is **Spanish**: full verb conjugation, noun gender and plurals, phrases, and words. French, Italian, and Portuguese arrive as free updates over the next twelve months.

Every feature below is shared infrastructure — the adaptive engine, the drill loop, the example-sentence rendering, the help system — that works the same way across every module. The differences are catalogue size and language-specific grammar quirks.

---

## Latin

The Latin module is the deepest the app gets. Coverage as of v1.0:

- **~300 verbs** across all five conjugations, with full tense paradigms (present-system + perfect-system, indicative + subjunctive + imperative, active + passive, plus participles, gerundive, infinitives, supine).
- **~270 nouns** across all five declensions, including i-stem 3rd-declension, 4th-declension neuters, and plūrāle-tantum entries (*moenia*, *līberī*).
- **~150 adjectives** across all five patterns (1st/2nd-decl *-us/-a/-um*, *-er/-a/-um*, 3rd-decl two-ending *fortis/-e*, 3rd-decl one-ending *ingēns*, 3rd-decl three-ending *ācer/-cris/-cre*) — with comparative and superlative derivation.
- **11 pronouns** with full case×number×gender paradigms (the personal, demonstrative, relative, and interrogative classes).
- **29 numerals** — *ūnus / duo / trēs* with full declension, *quattuor* through *centum* as indeclinable reference cards.

### Macron-accurate answer checking

The default answer-check is **lenient on macrons** — typing *rosa* when *rōsa* is correct counts as right with a gentle reminder. A toggle in Preferences switches this to **strict** for users who want the long vowels in their muscle memory. (Macron drill — a dedicated drill that asks you to type a stripped word with its macrons restored — arrives in v1.5.)

### Sentence parser

Open Self Study → **Identify a Form** and switch to **Sentence** mode. Paste any Latin sentence — Caesar's opening, a Vulgate verse, your homework — and tap **Parse**. Each word becomes a chip showing its lemma, case, number, gender, tense, voice, and translation. Words with multiple parses (Latin is full of these — *vēris* could be gen.sg of *vēr* or 2sg.fut.ind of *vēreor*) show every parse stacked, sorted by pedagogical likelihood. Tap a chip to jump to that word's full paradigm.

### Concordance drill

The drill that no other Latin app implements. Show a one-line Latin sentence with a blank where an adjective should go. The noun appears in its inflected form; the learner picks the adjective form that agrees in case, number, and gender. Wrong answers explain which axis was wrong — *"bonum agrees with a neuter noun — puella is feminine."*

### Example sentences

Every noun and adjective in the catalogue has **three auto-generated example sentences** that pipe the lemma through the same template library the concordance drill uses. About 1,100 sentences in total across the Latin catalogue, all rendered in real Latin syntactic context with the focus form bolded and a case+number tag below. Hand-curated examples take precedence where they exist (about 28 nouns so far); the auto-examples fill the gap for everyone else.

---

## Spanish — first additional module

The first non-Latin module, fully wired into the same Setup / Study / Test pipeline.

### Verbs

Practise conjugation across all the major Spanish tenses for around 1,100 verbs.

- **Conjugation Drill** — given a verb, tense, and person, type the correct form or pick from multiple choices. Switchable on the fly.
- **Recognition** — given a conjugated form, identify the verb, tense, and person using three scroll wheels.
- **Word Meanings flashcards** — Spanish ↔ your language, both directions.
- **Past Participle**, **Gerundio**, and **Indefinido** drills — focused flashcard decks for the forms that carry the most irregularity. The decks always include all irregular members of your selection, plus a sample of regulars.
- **Conjugation tables** — full tables for every verb, with irregular forms **colour-coded**: red on just the parts of a form that deviate from the regular pattern (stem changes, irregular yo forms, y-verbs, irregular future stems), and the whole form in red where it's entirely irregular — including strong preterite verbs and forms of *ser*, *ir*, *haber*.

Verbs are filterable by **CEFR level** (A1–C2), **frequency**, **topic** (travel, food, work, …), and **verb group** (regular -ar / -er / -ir, stem-changing e→ie / e→i / o→ue, go-verbs, zco-verbs, j-verbs, guir-verbs, y-verbs, uir-verbs, strong preterite, reflexive, impersonal, gusto-type, stative). You can also toggle individual tenses on or off.

### Nouns

Around 1,300 Spanish nouns, with practice for gender, plurals, and alternate-gender pairs.

- **Pick the correct article** — *el* or *la*?
- **Singular / Plural** — produce the correct plural from the singular form.
- **Alternate gender pairs** — practise nouns whose meaning changes with the article (*el capital* = money/capital, *la capital* = capital city; *el orden* = order/sequence, *la orden* = command).
- **Meaning flashcards** — Spanish ↔ your language.
- **Reference notes** — gender rules and an explainer for alternate-gender pairs.

Filter by CEFR level, frequency, or topic (home, food, body, technology, …).

### Personal topics

In addition to the bundled topics that ship with the app, you can add **your own topics** to any verb or noun. Open a word's detail view, tap **+** in the Topics row, and either type a new tag (like *exam*, *tricky*, or *kitchen*) or pick from one you've used before. Personal topics live alongside the bundled topics in the same filter and behave the same way — you can mix them freely with CEFR level, frequency, and the standard topic categories.

The data is stored locally on your device. There is no cloud sync; tags survive app updates but stay on the device they were created on.

### Phrases and Words

**Phrases** is the largest drillable pool in the app — around **6,000 entries**. It combines ~240 curated set phrases (greetings like *buenos días* and *mucho gusto*, time expressions like *en punto* and *de vez en cuando*, conversational chunks like *a pesar de* and *sin embargo*) with ~5,700 example sentences synthesised from the verb and noun catalogues. Every example sentence you'd see on a verb or noun detail card is also drillable here as its own phrase. Toggle the **Example** topic to switch the synthesised layer on or off as a single bucket.

**Words** covers single-word vocabulary that isn't a verb or noun — adjectives (with masculine/feminine pairs merged into one entry), adverbs, prepositions, conjunctions, and numbers. Filterable by grammatical category.

Both sections follow the same Setup / Study / Test pipeline as Verbs and Nouns. Practice is via **flashcards** in either direction (Spanish ↔ your native language, or a random mix).

### Speech

LinguaMorpha uses **iOS speech synthesis** to read Spanish forms aloud. iOS includes Spanish voices at three quality levels — Standard, Enhanced, and Premium. The Enhanced and Premium voices are free to download from iOS Settings and sound much better than the default. See the [Getting Started guide](getting-started.md#2-set-up-speech-one-time-strongly-recommended) for step-by-step instructions. A speed slider in the app lets you slow speech down for listening practice.

Latin doesn't have a native iOS TTS voice in v1.0. (An *approximate classical pronunciation* mode using the Italian voice with a transformation layer arrives in v1.5.)

### External dictionary lookups

Every Spanish verb and noun detail view has a **Look up** row with chip buttons for four well-known online dictionaries: **Linguee**, **WordReference**, **Reverso**, and **RAE** (the Real Academia Española). Tap a chip and the lookup opens in an in-app Safari sheet — you don't leave LinguaMorpha. The toggles for which services appear live in **Settings → Dictionary Services**. (Latin doesn't surface these — the sentence parser is the equivalent reference path.)

---

## Adaptive learning

Every answer you give is recorded in a local database on your device. Sessions are built using a strict priority order:

1. **Unseen words first**, ordered by significance — A1 very-common words before C2 rare words.
2. **Previously-seen words**, ordered by correct rate, weakest first. Ties broken by oldest last-seen date.

A **Learning Pace** setting (Relaxed / Balanced / Intensive) adjusts the balance between new vocabulary and review. Within a single session, each word appears exactly once. *(Adaptive learning is fully wired for Spanish in v1.0; Latin-side performance tracking lands in a follow-up release — drills work, they're just not yet adaptive.)*

---

## Guided Grammar Lessons (v1.3)

The structured-curriculum side of the app returns in v1.3. Lessons walk through verb and noun morphology in textbook-aligned chapters — paced to Wheelock or LLPSI for Latin, paced by tense for Spanish, with **Study** and **Practice** phases for each. An *Include previous* toggle lets you mix in earlier lessons to keep older material fresh.

Hidden in v1.0 to keep the launch focused; the implementation is there and tested, just feature-flagged off.

---

## What's coming

LinguaMorpha is a platform. Latin and Spanish are what's in v1.0; the rest of the Western Romance family lands as free updates over the next year, plus the structured-lessons system. **Every one of these is included free in any v1.0 purchase.**

- **v1.1** — Latin standout: the sentence parser, concordance drills, textbook vocab packs.
- **v1.2** — **French**.
- **v1.3** — Guided lessons return (Latin + Spanish first).
- **v1.4** — **Italian**.
- **v1.5** — Macron drill, etymology bridge, approximate classical TTS for Latin.
- **v1.6** — **Portuguese**.

Roadmap order may shift; every module listed here is committed.

---

## Settings

A few settings let you tune how the app fits your study habit:

- **Active language** — flip between Latin and any installed modules (Spanish in v1.0).
- **Display language** — single toggle (🇬🇧 / 🇳🇱) flips the app's chrome and the translations on flashcards between English and Dutch.
- **Session Size** — how many words appear in each session: 10, 20, 30, 50, or All.
- **Learning Pace** — *Relaxed*, *Balanced*, or *Intensive*. Biases the balance between new vocabulary and review.
- **Auto-advance** — when on, a correct answer moves to the next card after a short pause.
- **Speech** — pick a Spanish voice and adjust the speaking speed.
- **Strict macrons** — switches the Latin answer-check from lenient (macron-folded) to strict.
- **Dictionary Services** — choose which of Linguee, WordReference, Reverso, and RAE appear in the Look up row on Spanish verb and noun detail views.

You can reset your study history from **Settings → Data → Reset Progress** — by module, by category, or all at once. Your word-selection filters are not affected.

---

## Privacy

LinguaMorpha stores everything locally on your device. There is no account, no sign-in, no cloud sync, and no analytics that personally identify you. The full [Privacy Policy](../privacy-policy.md) has the details.

---

## Pricing

LinguaMorpha is **free to download** from the App Store and **free to use for 21 days** with every feature unlocked. After the trial, a single **one-time purchase of €29.99** unlocks the app for good. No subscriptions, no renewals, no ads, no in-app upsells.

The purchase is per Apple ID, so it covers your iPhone and iPad together if both are signed in to the same account. **Every future Western Romance module — French, Italian, Portuguese — and the structured-lessons system are included in this one-time purchase at no additional charge.** Pricing in non-Euro App Store regions follows Apple's regional pricing matrix; the App Store listing is the source of truth for your country.
