---
name: app-content
description: Use for any content work in this app - researching, writing, extending, correcting or reviewing its competencies, chapters, pages, rounds, questions, exercises, figures, terms or sources. This app's own content decisions; they take precedence over the generic lernapps content skills. Load it before you change any content.
---

# Content guide of this app

## Curriculum

- **Subject & level:** German as a Foreign Language (`subject: daf`, `strand: daf/grammatik`), CEFR **A1** (learning map band `5-6`).
- **Orientation:** Learning map `https://lernapps.net/apps/map/daf.json` (canonical source `lernapps/apps/map/daf.yaml`, based on ZfA/KMK *Rahmenplan DaF*, Goethe-Institut / ÖSD / telc A1, and CEFR Companion Volume 2020) and build brief `lernapps/apps#874` (part of overview epic `lernapps/apps#887`).
- **Standard variety:** Standard German as used in Germany (*Bundesdeutsch*) only — Austrian and Swiss everyday specialties are excluded at A1 to avoid confusing beginners.
- **Languages:** `languages: [de, en]` (`de` first per `@lernapps/app-templates 0.20.0`, full English UI tree at `/en/`).

## Competencies

### Chapter 1: `pronomen-und-verben` — Pronouns and Present-Tense Verbs (A1 · 5–6)
1. `personalpronomen-nominativ` (*I can use German nominative subject pronouns ich, du, er, sie, es, wir, ihr, sie, Sie appropriately.*) → `src/pronomen-und-verben/personalpronomen.yaml` (`pronomen-einstieg`, `pronomen-zuordnen`, `pronomen-waehlen`, `pronomen-luecken`)
2. `praesens-sein-haben` (*I can conjugate sein and haben in the present tense to describe people, states, and possessions.*) → `src/pronomen-und-verben/sein-und-haben.yaml` (`sein-haben-einstieg`, `sein-haben-tabelle`, `sein-haben-saetze`, `sein-haben-schreiben`)
3. `praesens-regelmaessig` (*I can conjugate regular German verbs in the present tense, including stems ending in -t/-d and -s/-ß/-z.*) → `src/pronomen-und-verben/regelmaessige-verben.yaml` (`regelmaessig-einstieg`, `regelmaessig-zuordnen`, `regelmaessig-luecken`, `regelmaessig-schreiben`)
4. `praesens-vokalwechsel` (*I can conjugate common stem-changing verbs with e → i, e → ie, and a → ä in du and er/sie/es.*) → `src/pronomen-und-verben/verben-mit-vokalwechsel.yaml` (`vokalwechsel-einstieg`, `vokalwechsel-wahl`, `vokalwechsel-luecken`, `vokalwechsel-schreiben`)

### Chapter 2: `satzbau-fragen-imperativ` — Verb-Second Order, Questions and Imperative (A1 · 5–6)
5. `verb-zweitstellung` (*I can build German statements with the conjugated verb in Position 2, including when time or place starts the sentence.*) → `src/satzbau-fragen-imperativ/verb-zweitstellung.yaml` (`v2-einstieg`, `v2-pruefen`, `v2-ordnen`, `v2-umstellen`)
6. `w-fragen` (*I can ask and answer W-questions with wer, was, wo, woher, wohin, wann, and wie with the verb in Position 2.*) → `src/satzbau-fragen-imperativ/w-fragen.yaml` (`w-woerter-zuordnen`, `w-fragen-waehlen`, `w-fragen-ordnen`, `w-fragen-schreiben`)
7. `ja-nein-fragen` (*I can form yes/no questions with the verb in Position 1 and answer with ja, nein, or doch.*) → `src/satzbau-fragen-imperativ/ja-nein-fragen.yaml` (`doch-einstieg`, `ja-nein-ordnen`, `ja-nein-luecken`, `ja-nein-schreiben`)
8. `imperativ` (*I can form imperatives for du, ihr, and Sie with the verb in Position 1.*) → `src/satzbau-fragen-imperativ/imperativ.yaml` (`imperativ-einstieg`, `imperativ-zuordnen`, `imperativ-wahl`, `imperativ-luecken`)

### Chapter 3: `trennbare-verben-und-aduso` — Separable Verbs and Coordinating Conjunctions (A1 · 5–6)
9. `trennbare-verben` (*I can split separable verbs in main clauses with the verb in Position 2 and the stressed prefix at the end.*) → `src/trennbare-verben-und-aduso/trennbare-verben.yaml` (`trennbar-einstieg`, `trennbar-waehlen`, `trennbar-ordnen`, `trennbar-luecken`)
10. `konjunktionen-aduso` (*I can connect main clauses with aber, denn, und, sondern, and oder on Position 0 without changing Position-2 word order.*) → `src/trennbare-verben-und-aduso/konjunktionen-aduso.yaml` (`aduso-einstieg`, `aduso-waehlen`, `aduso-ordnen`, `aduso-verbinden`)

## Content structure

- **Story world (fixed across all pages):** **Peter** (12, English-speaking student who moves with his parents for a year to **Lindenberg**, a fictional mid-sized town in central Germany, joining **Klasse 6**), family friends **Familie Weber** (**Frau Weber / Katrin**, **Herr Weber / Thomas**, **Lukas** 12, **Mina** 9), class teacher **Herr Braun**, and classmate **Nadia** (12). Recurring visual model: movable **Sentence Cards** (*Satzkarten*) with a locked **Position-2 Verb Anchor** (*Verb-Anker*).
- **Page flow (1 competency per page, max 350 reading words, max 4 consecutive text blocks):**
  1. `einstieg` (Opening): 1–2 sentence Lindenberg scene (everyday age-12 world: school, football, bikes, park, family dinner) + optional Sentence Cards SVG + an immediate, easy opening task before the main rule.
  2. `regel` (Rule): Compact reference table, SVG diagram where helpful, `vocabulary` block where verbs are introduced, and a short `note` naming the main English-speaker trap in plain age-12 language.
  3. `uebung` (Practice): 3 more varied exercises (4 total per competency page), progressing from recognition/matching/ordering to gap-fill and sentence writing, ending with what Peter can do now.
- **Chapter self-assessment:** Each `chapter.yaml` defines `selfAssessment` drawing 1–2 self-contained, active exercises per competency page (6 in Ch 1, 6 in Ch 2, 4 in Ch 3 — 16 total across the app).

## Terminology

- **Address to learners:** Informal *you* in English (`en`) and informal *du* in German (`de`) throughout.
- **Core learner terms:** *Satzkarten* / *Sentence Cards*, *Verb-Anker* / *Verb Anchor*, *Position 1 / Position 2 / Position 0*, *Satzklammer* / *sentence bracket*, *Vorsilbe* / *prefix*, *Vokalwechsel* / *stem vowel change*, *ADUSO* (*aber, denn, und, sondern, oder*).
- **Standard German in Germany (*Bundesdeutsch*) used:** *Brötchen*, *Fahrrad*, *Klasse 6*, *Sportplatz*, *Tischtennis*, *Fußball*.
- **Avoided:** Dense linguistics jargon (*Mittelfeld*, unexplained *Subjekt-Verb-Inversion*), exchange-student / host-family / language-school framing, and inline backticks in prose.

## Exercise patterns

- **Pattern 1 — Situation opening (`single-choice`):** Short Lindenberg scene testing a classic English-speaker trap (e.g. `src/satzbau-fragen-imperativ/verb-zweitstellung.yaml`, `v2-einstieg`). Every option has a rule-based `info`.
- **Pattern 2 — Form & meaning recognition (`matching`, `true-false`):** Match pronouns/W-words/verb forms/imperatives or check Position-2 sentences (e.g. `src/satzbau-fragen-imperativ/verb-zweitstellung.yaml`, `v2-pruefen`).
- **Pattern 3 — Card ordering (`ordering`):** Arrange Sentence Cards into valid V2 statements, W-questions, yes/no questions, separable-verb brackets, and ADUSO clauses (e.g. `src/trennbare-verben-und-aduso/trennbare-verben.yaml`, `trennbar-ordnen`).
- **Pattern 4 — Guided conjugation & choice (`language-task`, `mode: table`, `choice`, `gap`):** `languages: { source: en, target: de }`, plain English `source`, German `[gap]` targets, `form: { case: hint }`, and diagnosed `mistakes` (e.g. `src/pronomen-und-verben/sein-und-haben.yaml`, `sein-haben-saetze`).
- **Pattern 5 — Productive sentence writing (`language-task`, `mode: write`):** Learners write full German sentences with `form: { punctuation: ok }` and targeted error feedback (e.g. `src/trennbare-verben-und-aduso/konjunktionen-aduso.yaml`, `aduso-verbinden`).
- Every competency page has **4 varied exercises** (≤ 2 guessable choices, ≥ 2 active tasks).

## Figures

- **Sentence Cards & Verb Builder SVGs (`src/images/*.svg`):** Self-drawn inline SVGs, `viewBox="0 0 340 <h>"` (crisp at 360 px), `source: { de: "Eigene Zeichnung", en: "Own drawing" }`, `licence: CC0-1.0`:
  - `verb-endings-cards.svg` (`regelmaessige-verben.yaml`): stem + ending builder with *machen*.
  - `stem-change-spotlight.svg` (`verben-mit-vokalwechsel.yaml`): highlights that only *du* and *er/sie/es* change their vowel (*helfen*, *sehen*, *laufen*).
  - `sentence-cards-v2.svg` (`verb-zweitstellung.yaml`): Position-2 Verb Anchor with subject vs. time on Position 1.
  - `sentence-cards-questions.svg` (`w-fragen.yaml`): W-question (Pos. 2 verb) vs. yes/no question (Pos. 1 verb).
  - `sentence-cards-bracket.svg` (`trennbare-verben.yaml`): *aufstehen* sentence bracket linking Pos. 2 verb and final prefix.
  - `sentence-cards-aduso.svg` (`konjunktionen-aduso.yaml`): Position-0 bridge (*aber*) leaving Pos. 1 + Pos. 2 untouched.
- **Color & contrast convention (≥ 4.5:1):** Neutral light card `#f8fafc` with `#cbd5e1` border and `#0f172a` text; subject blue (`#dbeafe` / `#1e3a8a`), Position-2 verb amber (`#fef3c7` / `#78350f`), rest/Position-0 green (`#dcfce7` / `#14532d`), W-word/prefix purple (`#ede9fe` / `#4c1d95`).
- Every figure leaves ≥ 24 px clear empty space at the bottom-right for the `© CC0-1.0` badge and **never reveals an exercise answer** (`explainer-figure-hides-answer`).

## Sources

- `https://lernapps.net/apps/map/daf.json` (canonical `lernapps/apps/map/daf.yaml`) — verified.
- `lernapps/apps#887` (DaF explainer overview) and `lernapps/apps#874` (build brief) — verified.
- No private creator material is committed.

## Adding a chapter or round

1. Check `https://lernapps.net/apps/map/daf.json` for competency ids and `requires`.
2. Create `src/<chapter-id>/chapter.yaml` and one YAML file per competency.
3. Register `<chapter-id>` in `src/app.yaml` (`chapters`).
4. Follow the 4-exercise pattern and 340 px SVG conventions above; 1 bis 3 ihrer Übungen in `selfAssessment` aufnehmen, wie Skill `lernapps-explainer-self-assessment` sagt.
5. Update this content guide (`.agents/skills/app-content/SKILL.md`), run `npx vp check --fix`, `npx vp build`, and `npx --no -- lernapps check`, then commit on a feature branch.

## Rules learned from mistakes

- Target age for A1 (`5-6`) is **12 years old (Klasse 6)**: Peter moves to Lindenberg with his parents for a year; Familie Weber (Katrin, Thomas, Lukas 12, Mina 9) are family friends — never write "Austauschjahr / exchange year / Gastfamilie / host family".
- SVG diagrams must use `viewBox="0 0 340 <h>"` (never `640` wide with small 11 px labels that shrink to ~6 px on 360 px phones) and leave ≥ 24 px clear bottom-right space for the `© CC0-1.0` badge.
- Never use an exercise's target sentence as the example inside a figure on the same page (e.g. `sentence-cards-questions.svg` uses *Wie heißt du?* and *Trinkst du gern Kakao?* so it does not leak *Woher kommst du?* or *Spielst du gern Fußball?*).
- Every competency page needs 4 varied exercises (not 3) and every chapter needs a `selfAssessment` block covering all its competency pages with self-contained active exercises.
