# Concordance Drill

The Concordance Drill is the most pedagogically distinctive test type in the Latin module. No other consumer iOS Latin app implements it.

<!-- TODO: screenshot when Latin screenshot kit lands -->

It works like this. The app shows you a one-line Latin sentence with a blank where an adjective should go. The noun in the sentence is already in its inflected form. Your job is to pick the adjective form that **agrees with the noun in case, number, and gender** — the *concordance* the drill is named after.

---

## A worked example

> *Puer ___ rosam puellae bonae dat.*
>
> (The boy gives a ___ rose to the good girl.)
>
> Pick the form of *pulcher* that fits the blank:
>
> - pulcher
> - pulchram
> - pulchrārum
> - pulchrīs

The noun *rosam* is accusative singular feminine — direct object of *dat*. The adjective has to agree: **accusative singular feminine** → *pulchram*. Tap that one.

If you pick wrong, the feedback explains exactly which axis you missed:

- Pick *pulcher* (nominative singular masculine) → *"pulcher is nominative masculine — rosam is accusative feminine. Case and gender both wrong."*
- Pick *pulchrārum* (genitive plural feminine) → *"pulchrārum is genitive plural — rosam is accusative singular. Case and number both wrong."*
- Pick *pulchrīs* (dative/ablative plural) → *"pulchrīs is plural — rosam is singular. Number wrong."*

This axis-by-axis feedback is what makes the drill instructive rather than just punishing. You leave each question knowing *what* you got wrong, not just *that* you got it wrong.

---

## Where the sentences come from

The sentence templates are stored inline in `LatinConcordanceTemplates`. Each case has a small library of natural Latin sentences with a `{N}` placeholder for the noun and a `{___}` placeholder for the adjective slot.

Example templates for accusative singular feminine:

- *Puer {N} videt.* (The boy sees the {N}.)
- *Magister {N} laudat.* (The teacher praises the {N}.)
- *Servus {N} portat.* (The slave carries the {N}.)

When the drill picks a noun + adjective pairing, it picks a sentence template appropriate to the case + number + gender, substitutes the noun into `{N}`, and presents the four adjective candidates.

The templates are written to be **pedagogically natural** — they use vocabulary the learner will already know and avoid syntactic complications like indirect statement that would distract from the agreement question. Hand-curated examples for tricky nouns take precedence; the auto-generated templates fill the gap for everything else.

---

## What's drilled

The drill exercises:

- **Case agreement** — does the adjective match the noun's case?
- **Number agreement** — singular with singular, plural with plural?
- **Gender agreement** — masculine with masculine, feminine with feminine, neuter with neuter?

All three at once. That's the point. The other Latin drills isolate each skill; this drill makes you produce all three correctly in a sentence context.

Substitutions across the four answer choices are deliberately near-miss. The wrong answers are not random — they're the same adjective in adjacent cases / numbers / genders. So the distractors are always plausible and you have to actually do the agreement reasoning.

---

## Settings

- **Switch noun gender** — by default the noun is drawn from across your declension pool; if you want to focus on a specific gender (e.g. neuter agreement, which trips up the most students), filter the noun pool from the Declensions Setup screen and the concordance drill follows your filter.
- **Switch adjective pool** — same model for adjectives. Filtering the Adjectives Setup pool to a specific pattern (e.g. 3rd-decl two-ending) restricts what the concordance drill draws from.
- **Show case names on each answer** — Settings toggle. Off by default (more pedagogically demanding); on shows "acc. sg. fem." under each candidate so you don't have to parse the adjective form yourself.

---

## What's not covered (yet)

In v1.0 the concordance drill only covers **attributive agreement** — adjectives in the same phrase as their noun. It does **not** cover:

- **Predicate agreement** — *Rōsa pulchra est.* The noun is in the nominative; the adjective agrees but they're not in the same phrase. Coming in v1.1.
- **Substantive adjectives** — *bonī laudant* (the good men praise). The adjective stands without a noun, with the noun implied by the form. Coming in v1.1.
- **Agreement with two coordinated nouns** — *vir et fēmina bonī sunt*. Tricky because Latin can resolve gender by various conventions. Out of scope for v1.x.

The base attributive drill is the right starting point; the v1.1 additions extend the same engine.

---

## When to use it

Use the concordance drill **after** you can produce noun forms and adjective forms separately and reliably. It's the integration drill — putting two morphologically-correct outputs together into a syntactically-correct sentence is its own skill, and it's the skill that separates someone who has memorised paradigms from someone who can actually read Latin.

If you're working from Wheelock or LLPSI, this drill is what makes chapter exercises like "Translate: the good girl gives a beautiful rose to the boy" actually feel automatic instead of laborious.
