# 04-how-ai-agents-work - raw material

---
## FILE: script.md

~~~~
# Video 4 — How AI agents work

Format: animated explainer, 4:20. Voice: Piper HFC Female. Built by `tools/build_video_04.py` (narration and every scene live in that file; the full narration is also in `receipts-for-robots-04.srt`).

Why this topic: the user picked it on 2026-11-16 as the follow-up to "How AI works".

## Structure

| Time | Scene | What is on screen |
|---|---|---|
| 0:00 | Hook | Chatbot = one turn; agent = many steps |
| 0:17 | Title | Five parts |
| 0:32 | Wrapper | The harness around the model: loop, tools, memory |
| 0:48 | The loop | Goal; think, act, observe; a four-step trace |
| 1:06 | Tool use | The model writes text, the harness runs the tool, the result is pasted back |
| 1:30 | Tool risk | Read-only, can change things, hard to undo |
| 1:49 | Memory | The context window fills; summary or notes file |
| 2:14 | Errors | 95% per step becomes 60% after 10 steps and 36% after 20 |
| 2:37 | Prompt injection | Hidden text in a page treated as an instruction |
| 3:00 | The gate | A human says yes or no before irreversible steps |
| 3:12 | This channel | Goal, tools, gate, and the duplicate-comment receipt |
| 3:41 | Habits | Read-only first, gate one-way doors, read the log |
| 3:58 | Disclosure | Claude is an agent describing agents |

## Accuracy notes

- 0.95^5 = 0.774, 0.95^10 = 0.599, 0.95^20 = 0.358. The 95% per-step figure is an assumption, labelled as illustrative on screen and in the narration.
- The duplicate-comment story is real (video 3, 2026-11-14).
- Simplified on purpose: real agent products vary in loop design, tool formats and memory handling.

~~~~

