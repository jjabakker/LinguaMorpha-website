---
description: Frequently asked questions about LinguaMorpha — Latin and Spanish modules, price and trial, supported devices, where data is stored, voices, dictionary lookups, and the sentence parser.
---

# Frequently Asked Questions

---

## General

**What is LinguaMorpha?**

A Latin-based language platform. The flagship module is **Latin** — every declension, every adjective pattern, comparative and superlative, macron-accurate answer checking, a sentence parser that handles arbitrary Latin text, and a concordance drill no other consumer iOS app implements. The first additional module is **Spanish** — full verb conjugation, noun gender and plurals, phrases, and words. French, Italian, and Portuguese arrive as free updates over the next twelve months. It is not a full language course; it is the structured, grammar-first drill tool you reach for when you want to actually master what you have been taught elsewhere. See the [Features page](features.md) for what's inside.

**Which languages can I learn?**

In v1.0: **Latin** and **Spanish**. French arrives in v1.2, Italian in v1.4, Portuguese in v1.6 — all as **free updates** to anyone who buys v1.0.

**Is LinguaMorpha free?**

LinguaMorpha is **free to download** from the App Store and **free to use for 21 days** with every feature unlocked. After the trial, a single **one-time purchase of €29.99** unlocks the app for good. No subscriptions, no renewals, no ads. The purchase is per Apple ID, so it covers iPhone and iPad together if both are signed in to the same account. **Every future Western Romance module (French, Italian, Portuguese) and the structured-lessons system are included in that one purchase at no additional charge.** Pricing outside the Euro zone follows Apple's regional pricing matrix; the App Store listing in your country is the source of truth.

**What devices does LinguaMorpha support?**

iOS 16.0 or later on iPhone and iPad.

**Do I need an internet connection to use the app?**

No. LinguaMorpha works fully offline. All word data is bundled with the app, all answers are stored on your device, and speech (where supported) uses iOS's built-in voices.

**Which Spanish dialect does the app teach?**

The vocabulary is general Spanish — usable in both Latin America and Spain. The verb conjugation tables include the *vosotros* forms used in Spain. For speech, you choose which regional Spanish voice you prefer (Spain, Mexico, Latin America, …) from your installed iOS voices.

**What variety of Latin does the app teach?**

Classical Latin (Caesar / Cicero / Vergil era). Forms are macron-accurate by default; vowel length is consistent with Wheelock's Latin and Allen-Greenough. The catalogue is aligned to standard textbook progressions — Wheelock chapters 1–25 and LLPSI *Familia Romana* capitula I–XIV are well-covered.

**What languages can I use as my own language?**

English or Dutch as the interface language, with translations in English or Dutch.

---

## Accounts, sync, and data

**Do I need to create an account?**

No. There is no account system. Open the app and start using it — that's the whole onboarding.

**Does my progress sync between my iPhone and iPad?**

Not currently. Each device keeps its own answer history. All data stays on the device it was created on.

**Where is my data stored?**

Inside the app's local sandbox on your device, in a SQLite database. Nothing is sent to a server.

**How do I reset my progress?**

In the app, go to **Settings → Data → Reset Progress**. You can reset by module (Latin or Spanish), by category (verbs only, nouns only), or everything at once. Your word-selection filters are not affected.

---

## Using the app

**Setup vs Study vs Test — what's the difference?**

Each section (Verbs, Nouns, Adjectives in Latin; Verbs, Nouns, Phrases, Words in Spanish) has three areas:

- **Setup** — define your word pool (which words can appear) and, where relevant, which tenses / declensions / patterns are active.
- **Study** — browse-only reference: paradigm tables, word-meaning lists, grammar notes. Nothing is recorded.
- **Test** — active practice: flashcards and drills. Every answer is recorded and feeds the adaptive engine.

**What's the difference between word pool and session size?**

Your **word pool** is the full set of words eligible to appear in sessions (defined by your CEFR / frequency / topic / declension / pattern filters). Your **session size** is how many of those words appear in a single sitting (10, 20, 30, 50, or All). The app picks the best N words from your pool each session, prioritising unseen and weak words.

**What are the three buttons on a flashcard?**

**Correct** — you knew it without hesitation. **Difficult** — you got there eventually, or were only partially right. **Incorrect** — you did not know it or were wrong. All three move the word to the next session — each word appears exactly once per session regardless of how you rated it.

**Can I add my own categories to words?**

Yes. Every verb and noun detail view has a **Topics** row with a **+** button — tap it to add a personal topic (e.g. *exam*, *tricky*, *kitchen*). Your topics live alongside the bundled ones (food, travel, work, …) in the same Topic filter on the Select screens, marked with a small person icon so you can still tell them apart. They're stored locally on your device and persist across app updates.

**What is the sentence parser?**

A Latin-only feature in Self Study → **Identify a Form**. Switch to **Sentence** mode, paste any Latin sentence, and tap **Parse**. Each word becomes a tap-through chip showing its lemma, case, number, gender, tense, voice, and translation. Words with multiple parses (Latin is full of these) show every parse stacked. The parser handles enclitics (-que, -ve, -ne), trailing punctuation, and capitalisation; it folds macrons so you can paste text without them.

**What is the concordance drill?**

A Latin-only drill that no other iOS app implements. Show a one-line Latin sentence with a blank where an adjective should go. The noun appears in its inflected form; the learner picks the adjective form that agrees in case, number, and gender. Pedagogically what separates real Latin syntax from paradigm-rote.

**What is the Look up row on a Spanish verb or noun?**

A row of chip buttons that opens four well-known online Spanish dictionaries — **Linguee**, **WordReference**, **Reverso**, and **RAE** — in an in-app Safari sheet, so you don't leave LinguaMorpha. Useful when you want a fuller definition or extra example sentences. All four are free and need no account. You can switch any of them off in **Settings → Dictionary Services**. Latin doesn't have an equivalent row — the sentence parser is the reference path.

**Why is part of a Spanish verb form shown in red?**

In Spanish conjugation tables, irregular forms are colour-coded. A **partial red** highlight marks the part of a form that deviates from the regular pattern (a stem change, an irregular yo form, etc.). A **fully red** form is completely irregular and must be memorised whole — strong preterite verbs are shown this way too. See the [Verbs section in the User Guide](../user-guide/verbs/) for the full key.

**How does the adaptive learning work?**

Unseen words come first, ordered by CEFR level + frequency so the most important vocabulary is introduced before the obscure stuff. Already-seen words are ordered by correct rate, weakest first. A **Learning Pace** setting (Relaxed / Balanced / Intensive) controls the mix of new vs review. *(Spanish drills are fully adaptive in v1.0; Latin drills work the same way but performance tracking is wired in a follow-up release.)*

---

## Speech

**Why does the Spanish speech sound robotic?**

iOS ships with Standard Spanish voices by default. They sound mechanical. Download a free **Enhanced** or **Premium** voice from **iOS Settings → Accessibility → Spoken Content → Voices → Spanish** and then select it inside LinguaMorpha under **gear icon → Speech**. The difference is dramatic.

**Why doesn't Latin have speech?**

iOS doesn't ship with a Latin TTS voice — Apple hasn't built one. An *approximate classical pronunciation* mode using the Italian voice with a transformation layer (hard *c*, *v* → *w*, *ae* → *ai* diphthong) arrives in v1.5. For v1.0, Latin is read-not-spoken.

**Can I slow the speech down?**

Yes — there's a Speed slider in **Settings → Speech** inside the app.

---

## Feedback and bugs

**How do I report a problem or suggest something?**

Give your iPhone a quick shake from anywhere in the app. A pre-filled email compose sheet opens immediately with a screenshot of the current screen already attached. Describe what you saw and send. Feedback goes straight to the developer.

**The app is crashing — what should I do?**

Try these in order:

1. Force-quit and reopen the app.
2. Check for an app update in the App Store.
3. Restart your device.
4. Reinstall the app. **Heads-up:** because data is stored locally only, reinstalling will lose your answer history. Do this only as a last resort.

If the issue persists, shake the device to send a bug report, or email [support@linguamorpha.nl](mailto:support@linguamorpha.nl) with your device model and iOS version.

---

## Privacy

**What data does LinguaMorpha collect?**

Nothing personal. See the [Privacy Policy](../privacy-policy.md) for the full statement.

**Does LinguaMorpha share my data with third parties?**

No — there is no server to share data with. All data stays on your device.

---

## Still have a question?

[Contact Support](../support.md){ .md-button }
