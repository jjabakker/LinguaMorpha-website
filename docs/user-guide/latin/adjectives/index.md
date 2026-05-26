# Latin Adjectives

The Latin Adjectives section covers all five textbook adjective patterns, with full case × number × gender paradigms for every adjective in the catalogue plus comparative and superlative derivation. The catalogue contains around 150 adjectives in v1.0 across the five patterns.

<!-- TODO: screenshot when Latin screenshot kit lands -->

This section has the same **Setup / Study / Test** layout as Declensions, with one extra test type unique to Latin — the [Concordance Drill](concordance/).

---

## The five adjective patterns

### 1st/2nd-declension *-us / -a / -um*

The textbook starting point. Masculine takes 2nd-declension *-us* endings, feminine takes 1st-declension *-a*, neuter takes 2nd-declension *-um*. Examples: *bonus / bona / bonum*, *magnus / magna / magnum*, *malus / mala / malum*.

This is by far the largest group — about 70 of the 150 adjectives in the catalogue follow this pattern.

### 1st/2nd-declension *-er / -a / -um*

Same shape as the *-us* pattern, but the masculine nominative singular ends in *-er* instead of *-us*. Two sub-patterns:

- **Keeps the *e* in oblique cases**: *miser / misera / miserum* (acc. *miserum*, gen. *miserī*…)
- **Drops the *e*** : *pulcher / pulchra / pulchrum*, *sacer / sacra / sacrum*

The app handles both automatically based on the lemma's stored stem.

### 3rd-declension two-ending

The masculine and feminine share a form; the neuter takes a different one. Examples: *fortis / fortis / forte*, *brevis / brevis / breve*, *facilis / facilis / facile*.

These follow the i-stem 3rd-declension pattern in the oblique cases (ablative singular in *-ī*, genitive plural in *-ium*, neuter nom/acc plural in *-ia*).

### 3rd-declension one-ending

A single nominative form across all three genders, with a distinct paradigm visible in the genitive. Examples: *ingēns* (gen. *ingentis*), *fēlīx* (gen. *fēlīcis*), *sapiēns* (gen. *sapientis*), *audāx* (gen. *audācis*).

The lemma is always shown with the genitive in the lexicon entry so the stem is unambiguous.

### 3rd-declension three-ending

Three distinct nominative singular forms across the three genders. The smallest group — about a dozen adjectives. Examples: *ācer / ācris / ācre*, *celer / celeris / celere*, *alacer / alacris / alacre*.

---

## Comparative and superlative

Every adjective in the catalogue produces its **comparative** (*-ior / -ius*) and **superlative** (*-issimus / -issima / -issimum* by default, plus the textbook irregulars).

The comparative is regular: *fortis → fortior, fortius*; *altus → altior, altius*. The comparative declines as a 3rd-declension two-ending adjective with consonant-stem endings (not i-stem) — so genitive plural *fortiōrum / fortiōrum* (not *fortiōrium*) and ablative singular *fortiōre / fortiōrī*.

The superlative is mostly regular with three productive sub-rules:

- Default: *-issimus / -issima / -issimum* — *altus → altissimus*, *fortis → fortissimus*.
- After *-er* stems: *-rimus* — *miser → miserrimus*, *ācer → ācerrimus*, *celer → celerrimus*.
- After the *facilis* family (six adjectives): *-illimus* — *facilis → facillimus*, *difficilis → difficillimus*, *similis → simillimus*, *dissimilis → dissimillimus*, *gracilis → gracillimus*, *humilis → humillimus*.

The fully irregular suppletives — *bonus → melior → optimus*, *magnus → maior → maximus*, *malus → peior → pessimus*, *parvus → minor → minimus*, *multus → plūs → plūrimus* — are stored explicitly and surfaced with a "suppletive" tag on their lexicon entries.

---

## What's on each screen

### Setup

- **Select Adjectives** — pick which adjectives are in your drill pool. Filterable by pattern, CEFR / textbook chapter, topic, and frequency.
- **Select Tenses (not applicable)** — adjectives don't have tenses, so this row doesn't appear in the Adjective coach.

### Study

- **Adjective Paradigms** — full case × number × gender tables for every adjective. Same shape as the noun Declension Paradigms screen.
- **Adjective Meanings** — searchable list with translations, browsable A–Z.
- **Comparative / Superlative Reference** — a dedicated card showing the comparative and superlative for the currently-viewed adjective, with the derivation rule annotated.

### Test

- **Decline the Adjective** — production drill, given lemma + case + number + gender, type the form. Same model as Decline the Noun.
- **Recognise the Form** — recognition drill, given a form, identify case + number + gender.
- **Comparative / Superlative Drill** — given the positive form, produce the comparative or superlative. Catches the irregulars and the *-rimus* / *-illimus* sub-rules.
- **[Concordance Drill](concordance/)** — adjective–noun agreement in a real sentence frame. The drill no other consumer iOS Latin app implements; covered on its own page.

---

## Recommended workflow

1. Start with **1st/2nd-decl *-us* / -a / -um*** as your pool. It's the largest group and the textbook starting point.
2. Use **Adjective Paradigms** as your reference while you're drilling.
3. Run **Decline the Adjective** and **Recognise the Form** in alternating sessions, the same as for nouns.
4. Add **3rd-declension two-ending** as your second pool. The i-stem features in the oblique cases need separate muscle memory.
5. Add the comparative / superlative drill once positive forms are automatic.
6. The **[Concordance Drill](concordance/)** is the integration drill — use it once you can produce both noun and adjective forms reliably. It tests whether you can put them together in a sentence, which is the real skill.
