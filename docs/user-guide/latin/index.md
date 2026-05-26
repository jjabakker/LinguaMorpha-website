# Latin Coach

The Latin module is a complete study system for classical Latin morphology. It covers all five declensions (including i-stem 3rd-declension and 4th-declension neuters), all five adjective patterns, the full classical verb system across the present and perfect systems, eleven pronouns, and twenty-nine numerals. Every form is macron-accurate by default and the answer-check can be set to strict or lenient on a per-user basis.

This guide documents every screen in the Latin module and the standard workflows for using them. Each section follows the same **Setup / Study / Test** structure as the rest of the app.

---

## What's in the Latin module

The Latin module is organised by part of speech. Each category has its own Setup / Study / Test pipeline.

- **[Declensions](declensions/setup/)** — around 270 nouns across all five declensions. Pick your word pool, study paradigms, then drill production and recognition.
    - [Selecting Declensions](declensions/setup/) — the word-pool picker and the irregular-noun footnote.
    - [Declension Paradigms](declensions/paradigms/) — the study screen with full case × number tables.
    - [Decline the Noun](declensions/decline/) — the production drill (type the requested form).
    - [Recognise the Form](declensions/recognise/) — the recognition drill (identify case, number, gender).
- **[Adjectives](adjectives/)** — around 150 adjectives across all five patterns, with comparative and superlative derivation.
    - [Adjectives overview](adjectives/) — the five patterns, comparative / superlative, and the drills.
    - [Concordance Drill](adjectives/concordance/) — adjective–noun agreement in a real sentence frame. No other consumer iOS Latin app implements this.
- **[Verbs](verbs/)** — around 300 verbs across all five conjugations, full tense paradigms, indicative + subjunctive + imperative, active + passive, plus participles, gerundive, infinitives, and supine.
- **Pronouns** — eleven all-irregular paradigms (personal, demonstrative, relative, interrogative). Surfaced as a top-level Grammar category with the same Setup / Study / Test shape.
- **Numerals** — twenty-nine cardinals. *Ūnus*, *duo*, and *trēs* decline fully; *quattuor* through *centum* are indeclinable reference cards.

Across categories, two features are unique to Latin and have dedicated pages:

- **[Sentence Parser](sentence-parser/)** — paste any Latin sentence and get every word parsed (lemma, case, number, gender, tense, voice, translation). Handles enclitics, capitalisation, punctuation, and macron-folded matches.
- **[Macrons](macrons/)** — how the app handles macrons (strict vs lenient checking, how to type them on iOS, and what the macron drill in v1.5 will cover).

---

## Recommended workflow

If you're new to Latin or returning to it after a long gap:

1. Go to **[Selecting Declensions](declensions/setup/)** and pick a manageable starting set — typically *first and second declension only*. That covers a few hundred nouns and is what every textbook starts with.
2. Use **[Declension Paradigms](declensions/paradigms/)** as your study reference. Read through the tables before drilling.
3. Drill **[Decline the Noun](declensions/decline/)** in one direction (nominative → all other cases) until you can produce the forms without thinking.
4. Drill **[Recognise the Form](declensions/recognise/)** in the other direction (form → case, number, gender). The two drills reinforce different muscles.
5. Move on to adjectives — **[Adjectives overview](adjectives/)** then the **[Concordance Drill](adjectives/concordance/)** once you can recognise noun forms reliably.
6. Use the **[Sentence Parser](sentence-parser/)** whenever you hit Latin text in the wild (Caesar, Vergil, Vulgate, your homework) and want to check your reading.

If you're a classics student following Wheelock or LLPSI:

1. The catalogue is aligned to Wheelock chapters 1–25 and LLPSI *Familia Romana* capitula I–XIV. Use the topic filter in Selecting Declensions / Selecting Adjectives / Selecting Verbs to scope your pool to the chapter you're on.
2. Read the chapter in your textbook, then drill the same vocabulary here until it's automatic.
3. The Guided Grammar Lessons system (arriving v1.3) will pace exactly this workflow.

---

## What's not in v1.0

A few features are committed but ship in later releases:

- **Macron drill** (v1.5) — type a stripped Latin word with its macrons restored. Different muscle from the main drills.
- **Etymology bridge** (v1.5) — hover any Latin word to see its Spanish / French / Italian / Portuguese descendants.
- **Approximate classical TTS** (v1.5) — Italian voice + transformation layer (hard *c*, *v* → *w*, *ae* → *ai* diphthong). v1.0 is read-not-spoken because iOS ships no native Latin voice.
- **Guided Grammar Lessons** (v1.3) — structured textbook-paced curriculum. Implementation is in the codebase but feature-flagged off in v1.0.

All four are included free in any v1.0 purchase.
