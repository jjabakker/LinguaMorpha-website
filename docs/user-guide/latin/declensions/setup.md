# Selecting Declensions

The Selecting Declensions screen is the word-pool picker for the Latin noun drills. Whatever you select here defines the eligible pool of nouns that can appear in the **Decline the Noun** and **Recognise the Form** tests, and also defines which nouns appear in the Declension Paradigms study screen.

<!-- TODO: screenshot when Latin screenshot kit lands -->

---

## How the picker is organised

The picker is grouped by **declension** — first, second, third, fourth, fifth — and inside each declension by **gender** (masculine, feminine, neuter). Each row shows a count: *e.g.* "First declension · feminine · 96 nouns". Tap the row to scope your drill pool to that group; tap again to remove it.

You can also filter by:

- **CEFR / textbook chapter** — *Wheelock ch. 1–10*, *LLPSI cap. I–VII*, and similar tags scope the pool to the vocabulary your textbook introduces in that range.
- **Topic** — bundled topics (family, war, religion, body, food) and any personal topics you've added.
- **Frequency** — high / medium / low, based on a corpus of Caesar, Cicero, and Vergil.

These filters intersect — if you pick "Second declension masculine" + "Wheelock ch. 1–10", you get the second-declension masculines that appear in those chapters and nothing else.

---

## The footnote about irregular nouns

If you select **All nouns**, the count at the top reads something like "Selected: 272 of 274 nouns". The two nouns the picker silently excludes are *vīs* (force, strength) and *Iuppiter* (Jupiter) — both have paradigms that don't fit the regular declension engine and can't be auto-generated.

A footnote on the picker spells this out explicitly so you can see what's excluded. Both nouns are documented in the catalogue and surface in the Sentence Parser; they just don't appear in the production / recognition drills. This is tracked in the project backlog and will be fixed in a follow-up release when the engine handles per-noun custom paradigms.

---

## Saving your selection

Your selection persists across sessions — close the app, come back next week, your pool is the same. To reset the picker to a default (typically *all nouns of first and second declension*), use the **Reset** button at the bottom of the screen.

If you want to clear the picker and start a fresh selection, tap **Clear all** at the top. The drill screens will refuse to start with an empty pool and prompt you back to this screen.

---

## Recommended starting sets

For learners new to Latin:

- **First and second declension only** — covers ~150 nouns, including most of the high-frequency vocabulary. This is what Wheelock chapters 1–4 and LLPSI cap. I–III use.
- **Add third declension** once you can produce first- and second-declension forms reliably. Third declension is the largest and most diverse group.
- **Add i-stem 3rd-declension** as its own focused drill once the regular 3rd is automatic. The i-stem pattern (*urbs*, *cīvis*, *mare*) deserves its own session because the genitive plural in *-ium* and the neuter ablative in *-ī* are the most-forgotten forms.
- **Fourth and fifth declension last** — they're the smallest groups and follow the textbook order.

For classics students reviewing a specific chapter, use the textbook-chapter filter and ignore declension grouping entirely.
