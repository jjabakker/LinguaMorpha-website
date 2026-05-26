# Macrons

Macrons are the horizontal bars over Latin vowels — *ā*, *ē*, *ī*, *ō*, *ū* — that mark the vowel as long. *Rosa* (with short *a*) means "rose" in the nominative singular; *rosā* (with long *a*) means "by/from/with a rose" in the ablative singular. Same letters, different meaning, different vowel length.

LinguaMorpha is **macron-accurate by default** in the catalogue but **lenient by default in answer checking**. This page explains how that works and what your options are.

---

## What macron-accurate means in the catalogue

Every noun, adjective, verb, pronoun, and numeral in the Latin catalogue stores the citation form and every inflected form with macrons exactly where they belong in classical Latin. The reference for vowel length is the consensus of Wheelock's *Latin: An Introductory Course* and Allen-Greenough's *New Latin Grammar* — the standard scholarly sources for classical pronunciation.

You'll see this everywhere in the app:

- **Lemma headers** show *rōsa, rōsae* (not *rosa, rosae*).
- **Paradigm tables** show *rōsam, rōsīs, rōsārum* (with macrons exactly where classical scholarship places them).
- **Verb principal parts** show *amō, amāre, amāvī, amātum* (with the long *-ā-* of the 1st-conj. stem and the long *-ī* of the perfect 1sg).
- **The Sentence Parser** restores macrons from the catalogue even if you paste un-macron-ed text.

This is the same standard you'd see in any well-edited Latin textbook. Macrons aren't decorative — they encode genuine phonological information that distinguishes meanings, drives metre in poetry, and clarifies otherwise-identical forms.

---

## What macron-accurate means in answer checking

The Latin drills can run in **two modes**, controlled by **Settings → Strict macrons**:

### Lenient (default)

The answer-check folds macrons before comparing. Typing *rosis* when the expected answer is *rosīs* counts as correct, with a gentle reminder: *"Right! (Macrons aside — the long *ī* belongs on the *i*.)"*

This is the default because forcing macron-perfect typing on every drill answer turns vocabulary work into typing practice. Most learners (a) don't have macron keys readily accessible on their phone keyboards, (b) don't yet need vowel-length to be muscle memory, and (c) benefit more from seeing many forms in many sessions than from being marked wrong on a typing detail.

### Strict

The answer-check is character-exact. *Rosis* counts as wrong when *rosīs* is expected. The wrong-answer feedback shows your input and the expected form side by side so you can see exactly which vowel was missing a macron.

Use strict mode when:

- You're preparing for a Latin exam that grades on macrons (some university courses do; most high-school courses don't).
- You want vowel length to be a part of your muscle memory for poetic metre or pronunciation.
- You're a teacher demoing the strict-checking behaviour to a class.

The toggle is global — once on, every Latin drill checks strictly. Switch it back off if you want to relax again.

---

## How to type macrons on iOS

iOS's keyboard has macron support **built in but slightly hidden**. Long-press the relevant vowel key and a popover appears with diacritic options.

- **Long-press *a*** — see *à á â ä æ ã å ā* — the last one is *ā*.
- **Long-press *e*** — *è é ê ë ē ė ę* — *ē* is in the row.
- **Long-press *i*** — *î ï í ī į ì* — *ī* is the fifth.
- **Long-press *o*** — *ô ö ò ó œ ø ō õ* — *ō* is the seventh.
- **Long-press *u*** — *û ü ù ú ū* — *ū* is the fifth.

This works on every keyboard layout iOS ships. Slide your finger to the macron-vowel without lifting and release to insert it. It's slow at first; you'll get faster with practice.

For typing Latin in any text field, a **dedicated Latin keyboard** is a faster option:

- **iOS Settings → General → Keyboard → Keyboards → Add New Keyboard**
- Add a keyboard that includes macron-vowels in its primary layout — *Hawaiian* and *Māori* both have *ā ē ī ō ū* on their primary keys, and they live happily alongside your English layout.
- Switch between keyboards with the globe key when you need macrons.

We've intentionally **not** added an in-app macron keyboard. iOS's keyboard model means a third-party keyboard would have to ship as a separate keyboard extension that the user enables in Settings — which is a worse UX than long-pressing on the system keyboard, plus it would request more permissions than the app needs.

---

## Macron drill (v1.5)

A dedicated **Macron Drill** is committed for v1.5. It works the other way around from the main drills: the app shows you a Latin word with the macrons **stripped**, and your job is to type it back with the macrons restored.

> Restore the macrons: **rosa**
>
> (Hint: ablative singular)
>
> Your answer: ____

This is the muscle that strict-mode answer-checking exercises, but isolated as its own drill — useful for students who want to learn macrons explicitly without making every vocabulary drill harder.

The drill includes a built-in macron keyboard so you don't have to fight iOS's long-press popover; macron-vowels are first-class keys in the drill's input field only. (Outside the macron drill, you still use the system keyboard.)

---

## Why we bothered

Most Latin apps drop macrons entirely — too much engineering work, too much UI friction, and most users won't notice. LinguaMorpha keeps them because:

- They're scholarly correct, and the app's positioning depends on being the deepest Latin module on consumer iOS.
- They make poetic metre legible without separate annotation. *Arma virumque canō, Trōiae quī prīmus ab ōrīs…* scans correctly when the vowel-lengths are visible.
- They distinguish forms that would otherwise be identical. *Rosā* (abl. sg.) vs *rosa* (nom. sg.) is a real ambiguity in unmacroned text, and the drill engine needs macrons to teach the distinction.
- Once they're in the data, the cost of *displaying* them is zero. The cost of asking the user to *type* them is what the lenient/strict toggle exists to manage.

So: macrons everywhere in display, optional in input. Strict if you want; lenient if you don't.
