# Sentence Parser

The Sentence Parser is one of the two features that make LinguaMorpha's Latin module stand alone on consumer iOS. Paste any Latin sentence — Caesar's opening, a Vulgate verse, a line from Cicero, your homework — and the app shows you a full parse of every word.

<!-- TODO: screenshot when Latin screenshot kit lands -->

It lives in **Self Study → Identify a Form**, where the top toggle switches between **Word** mode (lookup a single inflected form) and **Sentence** mode (parse a whole sentence).

---

## A worked example

Paste this into the sentence box:

> *Gallia est omnis dīvīsa in partēs trēs.*
>
> (Gaul is, as a whole, divided into three parts.)

Tap **Parse**. The app renders six tappable chips:

| Chip | Parse |
|---|---|
| **Gallia** | proper noun, fem. — *Gaul*. Nom. sg. |
| **est** | *sum, esse* — *to be*. 3sg. pres. ind. act. |
| **omnis** | *omnis, omne* — *all, every*. Nom. sg. fem. (in agreement with *Gallia*). |
| **dīvīsa** | *dīvidō, dīvidere, dīvīsī, dīvīsum* — *to divide*. PPP, nom. sg. fem. (predicate participle with *est* → periphrastic perfect passive). |
| **in** | preposition, takes acc. or abl. (here acc. — *partēs* is accusative). |
| **partēs** | *pars, partis* (f., 3rd-decl i-stem) — *part*. Acc. pl. fem. |
| **trēs** | numeral *trēs* (declinable). Acc. pl. (agreeing with *partēs*). |

Tap any chip to jump to the full lemma view — the verb's conjugation table, the noun's declension paradigm, the adjective's full agreement table, and so on.

---

## How ambiguity is handled

Latin words frequently have **multiple parses**. *Vēris* could be:

- genitive singular of *vēr* (spring) — second-declension neuter
- second-person singular future indicative active of *vereor* (to fear / revere) — semi-deponent

The chip shows **every** parse, stacked. Each parse is ranked by pedagogical likelihood — the one most likely in the surrounding context is highlighted; the others are dimmed but selectable. The ranking is heuristic, not semantically intelligent — it favours forms whose lemma is in the high-frequency tier of the catalogue, and forms whose gender / number matches an adjacent agreement target. It's right most of the time but you should treat it as a hint, not a verdict.

For forms with three or more parses, the chip shows the top two by default and an "expand" affordance reveals the rest.

---

## What the parser handles

- **Enclitics** — *-que*, *-ve*, *-ne* are split off and parsed independently. *Filiusque* parses as *filius* + *-que*.
- **Capitalisation** — sentence-initial capitals and proper-noun capitals are folded for matching; the original capitalisation is preserved in the display.
- **Trailing punctuation** — *.* *,* *;* *:* *?* *!* are stripped before lookup. Quotation marks (*"* and *'*) and parentheses are also handled.
- **Macron-folded matching** — paste *Gallia est omnis divisa* without macrons; the parser finds *dīvīsa* anyway. The display preserves the macrons from the catalogue, not from the input.
- **Compound forms** — the periphrastic perfect passive (*amātus est*), pluperfect passive (*amātus erat*), and future perfect passive (*amātus erit*) are recognised when the participle and the form of *esse* are adjacent.
- **Unknown words** — if a form isn't in the catalogue, the chip shows the word verbatim with a "no parse" indicator. The catalogue has around 750 lemmas in v1.0; rarer vocabulary will hit "no parse" until the catalogue grows.

What it doesn't handle:

- **Word order or syntax** — the parser is morphology-only. It tells you what each word *is*; it doesn't tell you what each word is *doing* in the sentence (subject, object, indirect object, agent of passive, etc.). Syntax-aware parsing is a v2.x bet, not v1.x.
- **Elision** — Latin verse elides vowels at word boundaries (*atque ego → atqu' ego*). The parser does not reconstruct elided forms; paste the unelided text if you want a parse.
- **Reading-order disambiguation** — if a Latin sentence has two valid readings (a real Caesar problem), the parser shows all the parses for each word and lets you choose. It does not pick a reading for you.

---

## Settings

- **Show alternative parses by default** — toggle in Settings. When on, the chip always shows all parses; when off (the default), only the top-ranked parse is shown unless you tap to expand.
- **Show case labels in the chip** — toggle. When on, the chip prefixes each parse with the abbreviated case label (*nom.*, *gen.*, *dat.*, …) for fast scanning.

---

## When to use it

- **Reading any Latin text** — Caesar, Cicero, Vergil, the Vulgate, your textbook's reading passages. Paste the sentence, get the morphology, then work out the syntax yourself. The parser is the dictionary-and-paradigm-table you don't have to flip pages in.
- **Cross-checking your own translation** — if you've translated a sentence and you're not sure you got a form right, paste it and see what the parser thinks.
- **Sight-reading practice** — paste a sentence cold, see how many words you can identify without the parser, then check yourself with the parser.
- **Studying ambiguous forms** — the parser is also the fastest way to see how often a given form (say *populī*) is ambiguous in real texts. Paste the sentence, see the multiple parses.

The parser is not a substitute for learning Latin. It's a faster reference than flipping through a textbook's appendix.

---

## Roadmap

- **v1.1** — Expanded catalogue and a few more high-frequency lemmas; better ranking of ambiguous parses; "common phrase" recognition (e.g. *eō ipsō*, *nē quid*).
- **v1.5** — Etymology bridge: hover any parsed Latin word to see its Romance descendants (Spanish *partes*, French *parties*, Italian *parti*, Portuguese *partes*).
- **v2.x** — Syntax-aware annotations: subject / object / agent labels on chips, agreement arrows between agreeing words. Big bet; not committed.
