---
description: What grammar LinguaMorpha drills — Latin morphology in full (all declensions, all adjective patterns, all tenses) plus Spanish verb conjugation, noun gender / plural, and adjectives, with explicit rules and adaptive drills.
---

# Grammar Coverage

LinguaMorpha was built around a simple conviction: the grammar of these languages is **knowable**. There are rules, the irregular forms cluster into patterns, and once you can see those patterns, the language stops feeling arbitrary. This page is a tour of the grammar LinguaMorpha drills, module by module, and the ways the app makes that grammar visible.

---

## Latin

The Latin module is the deepest the app gets. Catalogue at v1.0:

- **~300 verbs** across all five conjugations
- **~270 nouns** across all five declensions
- **~150 adjectives** across all five patterns
- **11 pronouns** with full case×number×gender paradigms
- **29 numerals**

### Verb grammar

Every classical tense, mood, and voice the morphology engine can derive — drilled with the same Setup / Study / Test pipeline as Spanish.

**Indicative — present system (active + passive)**

- Praesēns
- Imperfectum
- Futūrum

**Indicative — perfect system (active + passive — periphrastic with PPP + esse)**

- Perfectum
- Plūsquamperfectum
- Futūrum Exactum

**Subjunctive — every tense (active + passive)**

- Praesens Subjūnctīvus
- Imperfectum Subjūnctīvus
- Perfectum Subjūnctīvus
- Plūsquamperfectum Subjūnctīvus

**Imperative**

- Praesens (the everyday "do this!")
- Futūrum (formal / legal register — Twelve Tables, prayers, philosophical maxims)
- Plus their passive counterparts

**Non-finite forms**

- Six infinitives (three tenses × two voices)
- All four participles (Praesens Āctīvum, Perfectum Passīvum, Futūrum Āctīvum, Futūrum Passīvum / Gerundīvum)
- Gerundium (verbal noun)
- Supīnum (acc. -um for purpose, abl. -ū for respect)

You can toggle any tense on or off in **Select Tenses**, the same way Spanish works.

### Noun grammar

All five declensions are first-class:

- **First** (-a / -ae, mostly feminine): *puella*, *aqua*, *rosa*
- **Second** (-us / -ī or -um / -ī, mostly masculine or neuter, plus the -er masculine sub-pattern): *servus*, *bellum*, *puer*
- **Third** (varies / -is, all genders) — including the **i-stem** sub-pattern (*urbs*, *cīvis*, *mare*) and the **-or → masculine** convention with feminine exceptions (*arbor*) all handled explicitly
- **Fourth** (-us / -ūs, mostly masculine, with notable feminine *manus*, *domus*): *exercitus*, *fructus*
- **Fifth** (-ēs / -ēī, almost all feminine): *diēs*, *rēs*

**Selection grain:** the Setup picker lets you scope the drill pool to whichever declensions you want active. Two **irregular** nouns (*vīs*, *Iuppiter*) sit outside the picker because their paradigms aren't auto-generated; both are listed in a footnote so you can see what's excluded.

### Adjective grammar

All five textbook patterns:

- **1st/2nd-decl** (-us / -a / -um): *bonus*, *magnus* — masc 2nd-decl, fem 1st-decl, neut 2nd-decl
- **1st/2nd-decl -er** (-er / -a / -um): *pulcher*, *miser*, *sacer* — same shape but the masc nominative drops -us
- **3rd-decl two-ending** (*fortis* / *forte*): masc + fem share a form, neut takes -e
- **3rd-decl one-ending** (*ingēns*, gen. *ingentis*): identical across genders in nom., distinct paradigm via genitive stem
- **3rd-decl three-ending** (*ācer* / *ācris* / *ācre*): three distinct nominative singulars

**Comparative + superlative derivation:** every adjective produces its comparative (*-ior / -ius*) and superlative (*-issimus / -ior + -rimus* for -er stems / -illimus for *facilis*-family). Irregulars (*bonus → melior → optimus*, *magnus → maior → maximus*) are stored explicitly.

### Pronouns and numerals

Both surfaced as top-level Grammar categories.

**Pronouns** — eleven all-irregular paradigms grouped by pedagogical class:

- **Personal:** *ego*, *tū*, *suī* (reflexive)
- **Demonstrative:** *is*, *hic*, *ille*, *iste*, *ipse*, *īdem*
- **Relative:** *quī*
- **Interrogative:** *quis*

**Numerals** — 29 cardinal numbers. Three decline fully (*ūnus / duo / trēs*) and get the full paradigm view; the rest (*quattuor* through *centum*, plus *mīlle*) are indeclinable and surface as a reference card with the citation form.

### How the app makes Latin patterns visible

**Macron-accurate answer checking.** The default check is lenient — *rosa* counts as right when *rōsa* is expected, with a gentle reminder. A toggle in Preferences switches to strict mode for users who want vowel length in their muscle memory.

**Sentence parser.** Paste any Latin text into Self Study → **Identify a Form** (sentence mode); every word becomes a tap-through chip with its full parse. Handles enclitics, capitalisation, punctuation, and macron-folded matches.

**Concordance drill.** Show a Latin sentence with a blank where an adjective should go; the noun is rendered in its inflected form; the learner picks the adjective form that agrees. Wrong-answer feedback explains which axis (gender / number / case) was off.

**Auto-generated example sentences.** Every noun and adjective gets 3 sentences piped through the concordance template library — focus form bolded, case + number tag below. Hand-curated examples take precedence where they exist.

---

## Spanish

The first additional module — fully wired into the same Setup / Study / Test pipeline, with around **1,100 verbs**, **1,300 nouns**, and **6,000 phrases**.

### Verb grammar

Every Spanish tense your textbook covers — and several it probably doesn't:

**Indicative — simple tenses**

- Presente
- Pretérito Imperfecto
- Pretérito Indefinido (preterite)
- Futuro Simple
- Condicional Simple

**Indicative — compound tenses**

- Pretérito Perfecto
- Pretérito Pluscuamperfecto
- Futuro Perfecto
- Condicional Perfecto

**Subjunctive — simple tenses**

- Presente de Subjuntivo
- Pretérito Imperfecto de Subjuntivo

**Subjunctive — compound tenses**

- Pretérito Perfecto de Subjuntivo
- Pretérito Pluscuamperfecto de Subjuntivo

**Imperative**

- Affirmative and negative command forms for all persons.

**Non-personal forms**

- Infinitivo, Gerundio (present participle), Participio (past participle).

You can switch any tense on or off in **Select Tenses**.

### Verb groups

Most Spanish verbs are regular — but the irregular ones cluster into recognisable groups. Drilling them by group rather than one at a time is the fastest way to internalise the patterns. LinguaMorpha's verb-group taxonomy includes:

**Stem-change groups**

- *e → ie* (*pensar*, *cerrar*, *querer*, *entender*, *preferir*)
- *e → i* (*pedir*, *servir*, *seguir*)
- *o → ue* (*poder*, *contar*, *volver*, *dormir*)
- *u → ue* (*jugar* — the only member)
- *i/u accent shift* (*enviar*, *confiar*, *actuar*, *continuar* — written accent on the stem vowel in present tenses)

**Yo-irregular and spelling groups**

- *yo-go* verbs (*tener*, *venir*, *poner*, *salir*, *hacer*, *decir*, …)
- Spelling-change groups: *c → qu* before *e*, *g → gu* before *e*, *z → c* before *e*, *gu → gü* before *e*

**Preterite / advanced groups**

- Strong preterites (*tener → tuve*, *venir → vine*, *hacer → hice*, *poder → pude*, *poner → puse*, *querer → quise*, *saber → supe*, *estar → estuve*, *traer → traje*, *decir → dije*)
- Reflexive verbs (*levantarse*, *vestirse*, *acostarse*)
- The handful of fully irregular verbs (*ser*, *ir*, *haber*) that have to be memorised whole

**Restricted groups**

- Defective verbs and verbs used only in third-person forms (*gustar*, *encantar*, *doler*, …) — flagged so drills don't ask you to produce a *yo* form that doesn't exist.

You can select any combination of these groups — for instance, "all stem-changers" gives you one focused drill across hundreds of verbs that share the same pattern family.

### How the app makes Spanish patterns visible

**Colour coding.** Inside every conjugation table, only the part of a form that deviates from the regular pattern is highlighted in red. The rest stays in the default text colour. When the entire form is red, the verb is irregular as a whole (think *ser*, *ir*) and has to be memorised. When the *yo* form is red but everything else is plain, it's a *yo-go* irregular. When the stem vowel is red across the four "boot" persons (*yo*, *tú*, *él*, *ellos*) but plain in *nosotros*/*vosotros*, it's a classic stem-changer. The shape of the irregularity tells you what kind of verb you're looking at.

**Tense explanations.** Each tense card has an info button that opens a sheet with the endings table, usage notes, and example sentences. Available in conjugation tables and inline inside lesson screens.

**Drills tuned to specific weak spots.** Six dedicated test types target the parts of a verb you're most likely to forget:

- **Conjugation Drill** — produce the full conjugated form (type or pick).
- **Recognition** — given a form, identify the verb, tense, and person.
- **Word Meanings Flashcard** — Spanish ↔ your native language.
- **Past Participle** — recall the participio (with irregulars highlighted).
- **Gerundio** — recall the present-participle form.
- **Indefinido** — drill the *yo* and *él* preterite forms, where the strongest irregularities live.

### Noun grammar

Nouns are the area learners most often try to "just memorise" — and the area where pattern recognition pays off most. LinguaMorpha covers around 1,300 nouns plus the rules and patterns that govern them.

**Noun groups.** Like verbs, Spanish nouns cluster into recognisable patterns. A noun typically belongs to several groups at once (e.g. *lápiz* is both `z → -ces` and accent-loss-in-plural), so the group filter lets you target very specific patterns:

- **Gender traps** — *mano* / *foto* end in *-o* but are feminine; *día* / *problema* / *sistema* end in *-a* but are masculine.
- **Greek -ema / -ama / -oma** — the closed set of Greek-origin masculines.
- **Feminine suffixes** — *-ción*, *-sión*, *-dad*, *-tad*, *-tud*, *-umbre*, *-ie*, *-itis*.
- **Masculine suffixes** — *-or*, *-aje*, *-án*, *-ambre*, *-ón* (mostly).
- **Stressed *a* + feminine** — *el agua*, *el águila*, *el alma* (singular only).
- **Pairs** — *el tío* / *la tía*.
- **Epicene** — single form for both genders.
- **Meaning-changes pairs** — *el capital* (money) vs *la capital* (capital city).
- **Heteronymous pairs** — *padre* / *madre*, *hombre* / *mujer*.
- **Invariable plural** — *el lunes* / *los lunes*.
- **Mass nouns** — typically singular only.
- **Plurale tantum** — *los pantalones*, *las gafas*.
- **Plural formation rules** — *z → -ces*, accent loss, consonant + -es.
- **False cognates** — *embarazada* ≠ embarrassed.

**Drills.** Four dedicated noun tests: Meaning, Pick the Correct Article, Singular / Plural, Alternate Gender Pairs. Plus three reference screens (Gender Rules, Alternate Gender Explained, Plural Formation).

### Phrases and example sentences

Around **240 curated set phrases** plus around **5,700 example sentences** synthesised from the verb and noun catalogues — every verb / noun example sentence is also drillable as its own phrase. That brings Phrases to ~6,000 entries total. A dedicated **Example** topic tag toggles the synthesised layer on or off.

---

## The adaptive engine (cross-module)

Coverage is only half the story. What makes LinguaMorpha feel different is that the app **uses what it knows about you** to decide what to drill next:

- Every answer is recorded locally.
- Unseen words appear first, ordered by significance (A1 very-common before C2 rare).
- Once a word has been seen, it's promoted up the queue when you get it wrong and demoted when you get it right.
- A **Learning Pace** setting (Relaxed / Balanced / Intensive) controls how aggressively the app introduces new material vs reviewing.

No subscriptions, no cloud, no account. Everything is on your device.

*(Adaptive learning is fully wired for Spanish in v1.0; Latin drills work the same way but write to the performance database in a follow-up release.)*

---

## Where to next

- [Features overview](features.md) — what's in the app.
- [Getting Started](getting-started.md) — install, set up voices, run your first session.
- [Recipes](recipes.md) — worked scenarios: "I want to study Latin's 3rd declension", "I want to study Pretérito Imperfecto", "I keep mixing up por and para".
