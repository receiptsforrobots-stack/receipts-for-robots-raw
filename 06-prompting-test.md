# 06-prompting-test - raw material

---
## FILE: answers.md

~~~~
# Video 6 — raw answers and scoring (run 2026-11-18, one attempt each, fresh chat each, no retries)

Setup: ChatGPT free, logged out (model not shown). Gemini free, logged out, model shown as "Flash-Lite" (different from video 5, where Gemini was signed in on "Auto"). Prompts and the 8-point rubric are in `protocol.md`, written before any run.

## ChatGPT

**D (vague):** Subject "Request for Assistance – Broken Headphones". Body: says the headphones "are not working properly", asks whether they can be "repaired, replaced, or refunded", offers a receipt, signs "[Your Name]".

**A (plain, specific):** Subject "Damaged Headphones on Arrival – Order #48213". Mentions order #48213, delivered November 10, crack in left ear cup, photo attached, replacement rather than refund, response within 5 business days. Signed Sam.

**B (role trick):** Subject "Replacement Request – Order #48213". Same facts; adds "as the product arrived in unacceptable condition". Signed Sam.

**C (pressure trick):** Opened with "Take a breath — I've got you. Here's a polite, professional, and firm email under 120 words." Same facts in the email. After the email it added a line saying the email is clear, firm and professional. Signed Sam.

## Gemini (logged out, Flash-Lite)

**D (vague):** Subject with "[Brand/Model of Headphones]" and "Order #[Order Number]". Body full of placeholders ([Date of Purchase], [describe the issue...]); asks for "a replacement or a repair"; mentions "a copy of my receipt/invoice [and photos of the damage, if applicable]"; signature block with [Your Name], [Your Phone Number], [Your Email Address]. Ended by offering to add warranty details.

**A (plain, specific):** All facts present; signed Sam.

**B (role trick):** All facts present; signed Sam.

**C (pressure trick):** All facts present, plus two things not in the prompt: "Since these headphones are urgently required for my professional work" and "an immediate replacement". It also asked SoundHub to "confirm the replacement shipment within 5 business days so I can plan accordingly". Signed Sam.

## Claude (added 2026-11-18 at the user's request; same four prompts, same rubric, rubric unchanged)

How it was run: four fresh Claude instances (Sonnet-class, spawned as subagents of the session that runs this channel), one per prompt, none aware of the test or of the other prompts, no tools, one attempt each. The instruction given with each prompt was: reply exactly as a chat assistant would reply in a chat window, output only your reply. That is NOT the claude.ai app, and the "output only your reply" line is a harness difference the other two tools did not get (it may have kept Claude's replies free of preambles). Claude is made by Anthropic, the company that built the session that ran this test; that is a conflict of interest, handled by fixing the rubric first and counting words by script.

**D (vague):** Subject "Broken Headphones - Request for Repair, Replacement, or Refund". Brackets for store name, brand/model, order number, date, purchase method, the problem and the signature block; asks the store to choose between a replacement, a repair or a full refund; says "I have attached photos of the defect and a copy of my receipt"; also wrote "I have used the headphones as intended and have not subjected them to any damage" (never stated by the user). Ended with a tip to fill in the brackets. 178 body words.

**A (plain, specific):** Subject "Order #48213 - Damaged Headphones, Replacement Requested". All facts present; also asks what is needed "including any return of the damaged unit". Signed Sam.

**B (role trick):** Subject "Replacement Request – Order #48213". All facts present; asks the store to confirm a new unit will be shipped. Signed Sam.

**C (pressure trick):** Subject "Replacement Request – Order #48213 (Damaged Headphones)". All facts present; asks how to return the damaged pair and when the replacement will ship. No preamble, no career line, no invented reason. Signed Sam.

## Scores (8 checks, counted from the outputs; body words by script)

| Prompt | ChatGPT | words | Gemini | words | Claude | words |
|---|---|---|---|---|---|---|
| D vague | 1/8 | 74 | 0/8 | 120 | 1/8 | 178 |
| A plain, specific | 8/8 | 76 | 8/8 | 86 | 8/8 | 73 |
| B + role trick | 8/8 | 77 | 8/8 | 79 | 8/8 | 71 |
| C + pressure trick | 8/8 | 75 | 8/8 | 87 | 8/8 | 91 |

Claude D scored 1/8 on "photo attached" (it said photos were attached, unconditionally); it failed "under 120 words" at 178 and the rest.

Notes on scoring:
- D scored only on checks it could meet: ChatGPT D passed "under 120 words" (74). Gemini D's body was exactly 120 words, which is not under 120, so it failed that too.
- Gemini C: check 6 ("asks for a reply within 5 business days") counted as passed, but the wording changed to "confirm the replacement shipment within 5 business days". Flagged in the video.
- Not part of the pre-registered rubric, reported separately: Gemini C invented a reason ("urgently required for my professional work"); ChatGPT C added a preamble and a closing comment outside the email. A "no invented facts" check was not in the rubric, so these are observations, not points.

## Verdict

On this task, the role trick and the pressure trick made no measurable difference to the 8 checks on any of the three tools. What moved the score was giving the facts (D versus A). The pressure line leaked into the output in ChatGPT and Gemini, in different ways; it did not in Claude, with the caveat that Claude's copies were told to output only the reply.

Limits: one task, one try each, a task with clear checkable constraints, free tiers for ChatGPT and Gemini (Gemini on Flash-Lite this time), Claude run as Sonnet-class agent instances rather than the claude.ai app.

~~~~

---
## FILE: protocol.md

~~~~
# Video 6 — prompting test: protocol (written BEFORE any run, 2026-11-18)

Question: do popular prompt "tricks" change the result, or is it the facts you give?

Tools: ChatGPT (free, logged out) and Gemini (free, channel account, "Auto"). Fresh chat for every run. One attempt per prompt, no retries, no edits.

## Scenario (invented)

Store "SoundHub", order #48213, wireless headphones delivered Nov 10, left ear cup cracked on arrival, want a replacement (not a refund), photo attached, reply within 5 business days, polite but firm, under 120 words, signed "Sam".

## The four prompts

- **D (vague control):** `Write an email to a store about my broken headphones.`
- **A (plain, specific):** `Write an email to SoundHub support. Order #48213, wireless headphones delivered Nov 10, left ear cup cracked on arrival. I want a replacement, not a refund. Mention that a photo is attached. Ask for a reply within 5 business days. Polite but firm. Under 120 words. Sign off as Sam.`
- **B (A + role trick):** `You are a world-class customer service expert. ` + A
- **C (A + pressure trick):** A + ` Take a deep breath. This is extremely important to my career.`

## Rubric (8 checks, 1 point each, applied to every output, decided now)

1. Mentions order #48213
2. Asks for a replacement (not a refund)
3. Mentions the cracked left ear cup
4. Mentions delivery on Nov 10
5. Says a photo is attached
6. Asks for a reply within 5 business days
7. Body under 120 words (greeting and sign-off excluded; counted by script)
8. Ready to send: no [bracketed placeholders] left, signed Sam

D is a control: it cannot score the fact checks, because the facts were never given. It shows what a vague prompt costs, not a "trick".

## Addendum (2026-11-18, after the ChatGPT and Gemini runs)

The user asked that Claude be tested the same way, since the channel should cover all top AI companies. Claude was run afterwards with the same four prompts and the same rubric (unchanged), as four fresh Claude instances (Sonnet-class agents, no tools, one per prompt). It is not the claude.ai app, and the instruction wrapper ("reply as a chat assistant, output only your reply") is a difference from the other two tools. Claude's makers also built the system running this channel, so the rubric stayed fixed and words were counted by script.

## What would count as a result

- A, B and C within 1 point of each other on both tools: tricks made no measurable difference on this task.
- Anything else is reported as it comes, with the limits (one try each, one task).

~~~~

---
## FILE: script.md

~~~~
# Video 6 — Do prompt tricks work?

Format: animated explainer plus a real test, 3:45. Voice: Piper HFC Female. Built by `tools/build_video_06.py` (narration and scenes live in that file; the narration is also in `receipts-for-robots-06.srt`).

Why this topic: topic 1 of the 2026-11-16 round 2 research (the user picked it on 2026-11-18). "How to use AI" is a top-searched question; this tests the tricks people repeat.

## Test design

- One task (a complaint email), four prompts: D vague, A plain/specific, B = A + role trick, C = A + pressure trick.
- ChatGPT (logged out) and Gemini (logged out, Flash-Lite), fresh chat per run, one attempt each.
- 8-point rubric written in `protocol.md` before any run. Word count by script.
- Claude added on the user's request (2026-11-18): four fresh Sonnet-class agent copies, same prompts, same rubric, one attempt each; not the Claude app; wrapper instruction "output only your reply" (disclosed). Duration is now 4:38.

## Results (see `answers.md`)

- D: ChatGPT 1/8, Gemini 0/8, Claude 1/8. A, B, C: 8/8 on all three tools.
- Claude D: 178 words and an invented "not subjected to any damage". Claude C: no leak (caveat: reply-only instruction).
- Tricks added no points. Observations outside the rubric: ChatGPT C preamble and closing comment; Gemini C invented "urgently required for my professional work" and "immediate", and turned the reply request into "confirm the replacement shipment within 5 business days".

## Structure

| Time | Scene |
|---|---|
| 0:00 | Hook: the three tricks |
| 0:13 | Title |
| 0:25 | The setup |
| 0:42 | The four prompts |
| 1:07 | The 8-point scoring |
| 1:30 | The vague prompt |
| 1:52 | The tricks scorecard |
| 2:12 | The surprise: the trick leaked |
| 2:43 | What to do instead |
| 3:00 | What this does not show |
| 3:25 | Disclosure |

## Accuracy notes

- Gemini's check 6 passed but the wording shifted; stated in the video.
- Gemini D's body was exactly 120 words, which fails "under 120"; D is a control, scored only against what it could meet.
- The video makes no claim beyond this task, these tiers and this day.

~~~~

