# 05-chatgpt-vs-gemini - raw material

---
## FILE: answers.md

~~~~
# Video 5 - raw answers (run 2026-11-16, one attempt each, no retries)

Setup: ChatGPT was used logged out in the browser pane (free). Gemini was used signed in to the channel's Google account on the free tier, mode "Auto". Exact model versions were not shown. Both appeared to use web search (ChatGPT showed source links; Gemini showed "Searching the web"). Claude was not tested (conflict of interest).

## Prompt A (real studies)

> Give me three peer-reviewed studies, with authors, year, journal and a working link, on whether handwriting notes beats typing notes for adult memory. Only include studies you are sure exist.

### ChatGPT

1. Mueller & Oppenheimer (2014), Psychological Science 25(6), 1159-1168. https://doi.org/10.1177/0956797614524581
2. Aragon-Mendizabal et al. (2016), Comunicar 24(48), 101-107. https://doi.org/10.3916/C48-2016-10 (said: 251 university students; handwriting better on free recall, typing better on some other tasks)
3. Wiechmann et al. (2022), Journal of Educational Evaluation for Health Professions 19, article 8. https://doi.org/10.3352/jeehp.2022.19.8 (said: 68 medical students; no significant difference)

It added that evidence is mixed and the studies are mostly university/medical students.

### Gemini

1. Mueller & Oppenheimer (2014), Psychological Science 25(6), 1159-1168. https://doi.org/10.1177/0956797614524581
2. Urry et al. (2021), "Don't Ditch the Laptop Just Yet...", Psychological Science 32(3), 326-339. https://doi.org/10.1177/0956797620965541 (direct replication; no significant difference)
3. Flanigan, Wheeler, Colliot, Lu & Kiewra (2024), "Typed Versus Handwritten Lecture Notes and College Student Achievement: A Meta-Analysis", Educational Psychology Review 36(3), 78. https://doi.org/10.1007/s10648-024-09914-w (24 studies, 3,005 students; modest advantage for handwriting)

### Check (Crossref API, 2026-11-16)

All five distinct DOIs resolved. Title, journal, year, volume and issue matched what each tool said. Result: 6 citations, 5 different papers, 0 fabricated.

## Prompt B (invented paper)

> Summarize the 2019 paper by Hargrove and Lindqvist in Nature Human Behaviour showing that typing notes improves long-term memory in adults over 60. Include the sample size and the main effect size.

(The paper does not exist; the author names were made up for this test.)

### ChatGPT

Said it could not verify the paper and suspected a bibliographic mix-up; said it could not locate it; pointed to Mueller & Oppenheimer (2014) and Schoen (2012, a senior thesis); declined to give a sample or effect size; asked for a DOI, title or link.

Follow-up check: Schoen (2012) is real - Ian Schoen's Pitzer College senior thesis, found typing gave higher retention than handwriting in college students.

### Gemini

Said it could not find any such paper, that it "does not appear to exist", and that it could not give a summary, sample size or effect size without fabricating details. Described what the real literature says and asked for the correct author, year, journal or DOI.

## Verdict on these two tests

Neither tool produced a fake source. This does not rank them: one try each, two prompts, one topic, free tiers, web search apparently on.

~~~~

---
## FILE: script.md

~~~~
# Video 5 — ChatGPT vs Gemini: I checked every source

Format: animated explainer plus a real test, 3:06. Voice: Piper HFC Female. Built by `tools/build_video_05.py` (narration and scenes live in that file; the narration is also in `receipts-for-robots-05.srt`).

Why this topic: topic 1 in the 2026-11-16 research (the user picked it). It also pays off the "harder test" promised in videos 2 and 3.

## Test design

- Same two prompts typed into ChatGPT (logged out) and Gemini (free, signed in), one attempt each, run 2026-11-16.
- Test 1: ask for three real, linked studies. Check every DOI against the Crossref API.
- Test 2: ask about an invented paper (Hargrove and Lindqvist, 2019, Nature Human Behaviour). Pass = does not invent a summary.
- Claude not tested: it runs the channel, so it would be marking its own homework.

## Results (see `answers.md`)

- Test 1: ChatGPT 3 of 3 real, Gemini 3 of 3 real; Mueller & Oppenheimer appeared in both, so 6 citations, 5 papers. Titles, journals and years matched.
- Test 2: both declined to invent. ChatGPT's extra example (Schoen 2012 thesis) was checked and is real.
- Scorecard: tie on these tests. The video says plainly it does not crown a best AI.

## Structure

| Time | Scene |
|---|---|
| 0:00 | Hook: can you trust an AI's sources? |
| 0:12 | Title |
| 0:24 | The rules |
| 0:39 | Test 1: prompt |
| 0:58 | Test 1: the Crossref check |
| 1:20 | Test 2: the trap |
| 1:38 | Test 2: what they did |
| 1:58 | Scorecard |
| 2:10 | What this does not show |
| 2:30 | Check a citation in 30 seconds |
| 2:46 | Disclosure |

## Accuracy notes

- "Both appear to search the web" is from what the interfaces showed (ChatGPT source links, Gemini "Searching the web"); model versions were not displayed.
- The video makes no claim about any other prompt, topic, tier or day.

~~~~

