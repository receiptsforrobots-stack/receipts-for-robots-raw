# 03-how-ai-works - raw material

---
## FILE: script.md

~~~~
# Video 3 — How AI works (and why it makes things up)

Format: animated explainer, 5:33. Voice: Microsoft David. Built by `tools/build_video_03.py` (narration and every scene live in that file; the full narration is also in `receipts-for-robots-03.srt`).

Why this topic: the research on 2026-11-14 put "how does AI actually work" at the top of what beginners search for, and it sets up the channel's tests by explaining why tools fabricate.

## Structure

| Time | Scene | What is on screen |
|---|---|---|
| 0:00 | Hook | An answer appearing one token at a time |
| 0:17 | Title | The five steps |
| 0:30 | 1 Tokens | A sentence split into tokens, then ID numbers |
| 0:50 | 2 Numbers | A 2-D "map of meaning" with three clusters |
| 1:15 | 3 Layers | Layer stack; attention arcs from "it" to "invoice"; then the per-token rework |
| 1:56 | 4 Guess | Probability bars for the next token; one is picked |
| 2:26 | 5 Repeat | The loop; a sentence growing token by token |
| 2:42 | Training | Dials (weights) nudged after a wrong guess; error shrinking |
| 3:21 | Context window | Instructions + conversation + files + tool results + message |
| 3:50 | What is missing | No fact database, no truth check |
| 4:05 | Why it makes things up | Common pattern vs rare pattern |
| 4:32 | Tie to video 2 | The tools ran code instead of predicting sums |
| 4:48 | Three habits | Source, calculate, check |
| 5:05 | Disclosure | Simplified; charts are illustrations |

## Accuracy notes

- All numbers on screen (token IDs, the 92% bar, embedding values, the error bar) are illustrative and labelled so on screen and in the narration.
- Simplifications made on purpose: sub-word tokenisation shown with one example; embeddings drawn in 2 dimensions; attention shown for one token; sampling described as "a little randomness"; fine-tuning described in one sentence.
- "No database of facts, no truth check" is about the model alone. The context-window scene and the video 2 scene cover tools added around it.

~~~~

