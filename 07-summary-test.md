# 07-summary-test - raw material

---
## FILE: answers.md

~~~~
# Video 7 — raw answers and scoring (run 2026-11-18, one attempt each, fresh chat each, no retries)

Prompts, documents and both rubrics are in `protocol.md`, written before any run. Both documents are invented.

Setup: ChatGPT free, logged out (model not shown). Gemini free, signed in on the channel's Google account, mode "Auto" (same as video 5). Claude: two fresh Sonnet-class agent copies (one per document), no tools, no knowledge of the test, each told to "reply exactly as a chat assistant would reply in a chat window, output only your reply" — NOT the claude.ai app, and the reply-only line is a difference the other tools did not get. Claude is made by Anthropic, the company behind the system that ran this test (conflict of interest, handled by fixing the rubric first and counting words by script).

## Document A (walnut article, "under 100 words")

**ChatGPT (82 words):** "A small pilot study found that adults who ate 30 grams of walnuts daily for eight weeks improved their word-recall scores by an average of 12%. Younger participants improved by 14%, while older adults improved by 4%, a result that may be due to chance. However, the study had no control group, making it impossible to confirm that walnuts caused the improvement. Researchers stress that larger controlled studies are needed. The research was industry-funded, and reported sleep improvements were not objectively measured."

**Gemini (95 words):** "A small pilot study from the Marlow Institute of Nutrition suggests eating 30 grams of walnuts daily for eight weeks may modestly boost memory. Across 48 adults, word-recall scores improved by an average of 12%—driven mainly by a 14% gain in adults under 65, while older participants saw a negligible 4% uptick. Participants also self-reported slightly better sleep. However, the findings are preliminary. The trial lacked a control group, did not include children, and was funded by the Pacific Walnut Council. Researchers emphasize that a larger, controlled study is needed to confirm the benefits."

**Claude (96 words):** "A small pilot study suggests eating 30 grams of walnuts daily may help memory. In the study, 48 adults ate walnuts for eight weeks and scored about 12% higher on a word-recall test. Adults under 65 improved 14% on average, while those 65 and older improved only 4%, which could be chance. Because there was no control group, the results can't prove walnuts caused the gains. The authors call the findings preliminary and want a larger controlled trial. A walnut trade group funded the work, though the paper says it had no role in the analysis."

### Scores A (8 checks)

| Check | ChatGPT | Gemini | Claude |
|---|---|---|---|
| 1 sample 48 | no | yes | yes |
| 2 overall about 12% | yes | yes | yes |
| 3 older group weak / chance | yes | yes ("negligible") | yes |
| 4 no control group | yes | yes | yes |
| 5 preliminary / pilot / larger trial | yes | yes | yes |
| 6 names the funder | no ("industry-funded" only) | yes | yes |
| 7 nothing unsupported | yes | yes | yes |
| 8 under 100 words | yes (82) | yes (95) | yes (96) |
| **Total** | **6/8** | **8/8** | **8/8** |

Judgement calls, stated openly: ChatGPT's "industry-funded" was scored as not naming the funder (the rubric says "Pacific Walnut Council or a walnut trade group"); counting it would make ChatGPT 7/8. Gemini's "negligible 4% uptick" was accepted as "weak" even though the text said "could be due to chance". Gemini's "may modestly boost memory" was accepted as hedged.

## Document B (Project Lantern memo, "under 80 words")

**ChatGPT (62 words):** "Project Lantern's launch has been delayed from March 4 to March 18 due to payment vendor testing delays. The budget increased from $40,000 to $52,000 to cover additional testing fees, with finance approval secured. Omar Singh replaced Dana Reyes as project owner on the 11th. Further vendor delays could push launch to April. The next review meeting is Friday at 2 p.m."

**Gemini (61 words, with a heading):** "Project Lantern Update. Status & Timeline: Launch moved from March 4 to March 18 due to payment vendor testing delays. Further slippage risks pushing launch to April. Budget: Increased from $40,000 to $52,000 (finance-approved) to cover extra vendor testing fees. Ownership: Transitioned from Dana Reyes to Omar Singh on the 11th. Next Step: Review meeting scheduled for Friday at 2:00 PM."

**Claude (57 words):** "Project Lantern: Launch slipped from March 4 to March 18 because the payment vendor's testing ran late. Budget rose from $40,000 to $52,000 for extra testing fees; finance has approved it. Omar Singh took over from Dana Reyes on the 11th. Risk: another vendor delay could push launch to April. Next review is Friday at 2 pm."

### Scores B (7 checks)

All three: 7/7 (current launch date March 18, current budget $52,000, current owner Omar Singh, reason for delay, April risk, no old value presented as current, under 80 words). Each described the old values as changes, not as current.

## Verdict

On two short, clean, invented documents: Gemini 8/8 and 7/7, Claude 8/8 and 7/7, ChatGPT 6/8 and 7/7. No tool invented a fact. The one gap was an omission: ChatGPT left out the sample size and did not name the funder. The documents were short and clear; the published studies on summaries of long, messy or technical papers found more distortion, so this does not show summaries are safe in general.

Limits: two short invented documents, one try each, free tiers, Claude run as agent copies (not the app, with a reply-only instruction), rubric judgement calls listed above.

~~~~

---
## FILE: protocol.md

~~~~
# Video 7 — summary test: protocol (written BEFORE any run, 2026-11-18)

Question: can AI summarize a document without distorting it? Two invented documents, three tools, one attempt each, fresh chat per run, no retries, no edits. Claude is included (user ruling 2026-11-18).

Tools: ChatGPT (free web, as the pane allows), Gemini (free web, as the pane allows), Claude (fresh Sonnet-class agent copies, no tools, not the claude.ai app; each told: reply as a chat assistant would, output only your reply).

Both documents are invented for this test; the organisations and people do not exist.

## Document A (science news, hedged finding)

Prompt A (one line, document pasted inline):

`Summarize the following news article in under 100 words for a general reader. Article: New study suggests a daily walnut snack may help memory scores. A pilot study from the Marlow Institute of Nutrition reports that adults who ate 30 grams of walnuts a day for eight weeks scored about 12% higher on a word-recall test than they did at the start. The study followed 48 adults: 36 aged 25 to 64 and 12 aged 65 or older. Among the 36 younger adults the average improvement was 14%. Among the 12 older adults it was 4%, which the authors say could be due to chance. There was no control group, so every participant ate walnuts. The authors call the result preliminary and say a larger controlled trial is needed. The study was funded by the Pacific Walnut Council, a trade group, which according to the paper had no role in the analysis. Participants also said they slept slightly better, but sleep was not measured objectively. The researchers did not test children.`

Rubric A (8 checks, 1 point each):
1. States the sample: 48 adults
2. Gives the overall result of about 12%
3. Says the older group's result was weak / possibly chance (4%)
4. Says there was no control group
5. Calls it preliminary / a pilot / needs a larger trial
6. Names the funder (Pacific Walnut Council or "a walnut trade group")
7. Says nothing the text does not support (no overclaiming such as "proves", "boosts memory" as a settled fact, "improves sleep" as a finding, and no invented facts)
8. Under 100 words (counted by script)

## Document B (memo with changed facts)

Prompt B:

`Summarize the following memo in under 80 words for a busy manager. Memo: Project Lantern update, sent Monday. Launch date: originally March 4. Last Tuesday the team moved it to March 18 because the payment vendor's testing slipped. Budget: approved at $40,000 in January, then revised to $52,000 on Thursday after the vendor quoted extra testing fees; finance has approved the revision. Owner: Dana Reyes led the project until the 10th, and Omar Singh took over on the 11th. Open risk: if vendor testing slips again, launch may move to April. Next review meeting is Friday at 2 pm.`

Rubric B (7 checks, 1 point each):
1. Gives the current launch date: March 18
2. Gives the current budget: $52,000
3. Names the current owner: Omar Singh
4. Gives the reason for the delay (vendor testing slipped)
5. Mentions the risk of moving to April
6. Says nothing the memo does not support, and does not present an old value (March 4, $40,000, Dana Reyes) as current
7. Under 80 words (counted by script)

## Scoring rules

- Decided now, applied to every output the same way. Words counted by script on the summary text only (not any preamble or closing note).
- Anything outside the rubric that is notable (invented facts, preambles, odd framing) is reported separately, not scored.
- Results are reported as they come, with the limits (two documents, one try each, free tiers, Claude run as agent copies).

~~~~

---
## FILE: script.md

~~~~
# Video 7 — Can AI summarize without distorting?

Format: animated explainer plus a real test, 4:22. Voice: Piper HFC Female. Built by `tools/build_video_07.py` (narration and scenes live in that file; the narration is also in `receipts-for-robots-07.srt`).

Why this topic: topic 1 of the 2026-11-18 research round (the user picked it). Search evidence was secondary (Utrecht summary-distortion study and a BBC investigation as reported in news write-ups; a Smallpdf vendor study).

## Test design

- Two invented documents: A, a short science article with hedges (pilot, 48 adults, about 12%, older group 4%, no control group, trade-group funder); B, a project memo with changed values (March 4 to 18, $40,000 to $52,000, owner Dana Reyes to Omar Singh).
- Three tools, one attempt each, fresh chat each: ChatGPT (free, logged out), Gemini (free, signed in, Auto), Claude (two fresh Sonnet-class agent copies, no tools, reply-only wrapper, not the app).
- Rubrics (8 checks for A, 7 for B) written in `protocol.md` before any run. Word counts by script.

## Results (see `answers.md`)

- A: ChatGPT 6/8, Gemini 8/8, Claude 8/8. B: 7/7 for all three.
- No invented facts. ChatGPT omitted the sample size and did not name the funder ("industry-funded").
- Judgement calls shown in the video and description.

## Structure

| Time | Scene |
|---|---|
| 0:00 | Hook |
| 0:11 | Title |
| 0:22 | The setup |
| 0:45 | Document A |
| 1:12 | The checklist for A |
| 1:35 | Result A |
| 1:53 | Document B |
| 2:14 | Result B |
| 2:28 | The judgement calls |
| 2:59 | What it shows |
| 3:17 | What to do |
| 3:33 | What this does not show |
| 3:59 | Disclosure |

## Accuracy notes

- The "published studies ... have reported more distortion" line rests on secondary reports; worded with "reported".
- The video says this is the good case (short, clear, invented documents) and not a ranking.

~~~~

