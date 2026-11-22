# 08-math-test - raw material

---
## FILE: answers.md

~~~~
# Video 8 - raw replies and scoring (run 2026-11-18, one attempt per round, fresh chat each, no retries)

Prompts: `prompt.txt` (round 1) and `prompt2.txt` (round 2). Keys: `key.py` and `key2.py` (computed by script before the runs). Scoring: `score.py`. Protocol and the round-2 addendum: `protocol.md`.

Setup: ChatGPT free web, logged out (model not shown). Gemini free web, signed in on the channel's Google account, mode "Auto". Claude: a fresh Sonnet-class agent copy per round, no tools, told to reply as a chat assistant and output only its reply - NOT the claude.ai app. Gemini and ChatGPT may use a built-in calculator/code tool (Gemini's page showed a "Show code" control); Claude's copy had none.

Round 2 was written after seeing round 1 (all 30/30) and its key fixed before it was run; this is disclosed in the video.

## Final answer lines

| Q | Round 1 key | ChatGPT | Gemini | Claude | Round 2 key | ChatGPT | Gemini | Claude |
|---|---|---|---|---|---|---|---|---|
| 1 | 66.00 | 66.00 | 66 | 66.00 | 442410312 | 442410312 | 442410312 | 442410312 |
| 2 | 30.09 | 30.09 | 30.09 | 30.09 | 24137569 | 24137569 | 24137569 | 24137569 |
| 3 | 2249.73 | 2249.73 | 2249.73 | 2249.73 | 453 | 453 | 453 | 453 |
| 4 | 48.62 | 48.62 | 48.62 | 48.62 | 250 | 250.00 | 250 | 250 |
| 5 | 0.4 | 0.40 | 0.4 | 0.4 | 48 | 48 | 48 | 48 |
| 6 | 260 | 260 | 260 | 260 | 8 | 8 | 8 | 8 |
| 7 | 190 | 190 | 190 | 190 | 11.11 | 11.11 | 11.11 | 11.11 |
| 8 | 0.15 | 0.15 | 0.15 | 0.15 | 36 | 36 | 36 | 36 |
| 9 | 9 | 9 | 9 | 9 | 48 | 48 | 48 | 48 |
| 10 | 298285 | 298285 | 298285 | 298285 | 7871.20 | 7871.20 | 7871.20 | 7871.20 |
| **Score** | | **10/10** | **10/10** | **10/10** | | **10/10** | **10/10** | **10/10** |

Total: ChatGPT 20/20, Gemini 20/20, Claude 20/20. Reply files: `chatgpt_reply.txt`, `gemini_reply.txt`, `claude_reply.txt` (round 1) and the `*_reply2.txt` files (round 2). ChatGPT's reply to round 1 contained only the answer lines; Gemini and Claude showed working first. For round 2, Gemini's and ChatGPT's final answer lines were read from the page; the working shown for Gemini matched the final lines.

Notes outside the rubric: no formatting breaks; ChatGPT wrote 0.40 and 250.00 (equal to the key). No tool fell for the quick-answer traps (Q8/Q9 in round 1, Q5 in round 2).

## Verdict
On these 20 problems no tool gave a wrong answer. This does not show that AI is never wrong at math. Limits: 20 problems I chose, one try each, free tiers, tools may have used built-in calculators (Claude's copy had none), Claude run as agent copies (not the app).

~~~~

---
## FILE: chatgpt_reply.txt

~~~~
Q1: 66.00
Q2: 30.09
Q3: 2249.73
Q4: 48.62
Q5: 0.40
Q6: 260
Q7: 190
Q8: 0.15
Q9: 9
Q10: 298285

~~~~

---
## FILE: chatgpt_reply2.txt

~~~~
Q1: 442410312
Q2: 24137569
Q3: 453
Q4: 250.00
Q5: 48
Q6: 8
Q7: 11.11
Q8: 36
Q9: 48
Q10: 7871.20

~~~~

---
## FILE: claude_reply.txt

~~~~
Q1. 80 x 0.75 = 60; 60 x 1.10 = 66.00.
Q2. 127.50 x 1.18 = 150.45; split five ways = 30.09. The dessert is already in the bill, so it changes nothing.
Q3. 2000 x 1.04^3 = 2000 x 1.124864 = 2249.73.
Q4. 7.2 x 3.65 = 26.28 L; 26.28 x 1.85 = 48.618, which rounds to 48.62. The car's colour doesn't matter.
Q5. 2.4 x 1/4 = 0.6 kg is left after the first use; 2/3 of that is 0.4 kg after using 1/3.
Q6. March 3 to March 31 is 28 days. April through October is 30+31+30+31+31+30+31 = 214 days. Add 18 days in November: 28 + 214 + 18 = 260.
Q7. Sunday is 2 x 44 = 88. Total = 44 + 58 + 88 = 190. The 5 smaller apples are still apples picked.
Q8. Let the pen cost p. Then p + (p + 2.00) = 2.30, so p = 0.15.
Q9. Each worker paints one fence alone, so the time stays 9 hours.
Q10. 487 x 639 = 311193; 311193 - 12908 = 298285.

Q1: 66.00
Q2: 30.09
Q3: 2249.73
Q4: 48.62
Q5: 0.4
Q6: 260
Q7: 190
Q8: 0.15
Q9: 9
Q10: 298285

~~~~

---
## FILE: claude_reply2.txt

~~~~
Q1: 442410312
Q2: 24137569
Q3: 453
Q4: 250
Q5: 48
Q6: 8
Q7: 11.11
Q8: 36
Q9: 48
Q10: 7871.20

~~~~

---
## FILE: gemini_reply.txt

~~~~
Q1: 66
Q2: 30.09
Q3: 2249.73
Q4: 48.62
Q5: 0.4
Q6: 260
Q7: 190
Q8: 0.15
Q9: 9
Q10: 298285

~~~~

---
## FILE: gemini_reply2.txt

~~~~
Q1: 442410312
Q2: 24137569
Q3: 453
Q4: 250
Q5: 48
Q6: 8
Q7: 11.11
Q8: 36
Q9: 48
Q10: 7871.20

~~~~

---
## FILE: key.py

~~~~
"""Answer key for video 8, computed by script BEFORE any tool was run."""
from datetime import date
from decimal import Decimal as D, ROUND_HALF_UP
def r2(x): return x.quantize(D("0.01"), ROUND_HALF_UP)
KEY = {
 1: r2(D(80)*D("0.75")*D("1.10")),
 2: r2(D("127.50")*D("1.18")/5),
 3: r2(D(2000)*D("1.04")**3),
 4: r2(D(365)*D("0.072")*D("1.85")),
 5: D("2.4")*D("0.25")*D(2)/D(3),
 6: D((date(2026,11,18)-date(2026,3,3)).days),
 7: D(44+58+2*44),
 8: D("0.15"),
 9: D(9),
 10: D(487*639-12908),
}
if __name__ == "__main__":
    for k,v in KEY.items(): print(k, v)

~~~~

---
## FILE: key2.py

~~~~
"""Round 2 answer key (harder), computed by script BEFORE any tool saw round 2."""
from datetime import date
from decimal import Decimal as D, ROUND_HALF_UP, getcontext
getcontext().prec = 40
def r2(x): return x.quantize(D("0.01"), ROUND_HALF_UP)
KEY = {
 1: D(48372*9146),
 2: D(17**6),
 3: D((date(2028,2,14)-date(2026,11,18)).days),
 4: D(230)/(D("0.8")*D("1.15")),
 5: D(48),
 6: D("strawberry raspberry blackcurrant".count("r")),
 7: r2(D(4)/D(36)*100),
 8: D(36),
 9: D(1234567 % 97),
 10: r2(D(5000)*(1+D("0.065")/12)**84),
}
if __name__ == "__main__":
    for k,v in KEY.items(): print(k,v)

~~~~

---
## FILE: prompt.txt

~~~~
Solve each of the 10 problems below. Show brief working if you like, but end your reply with exactly 10 final lines in this format, one per problem: "Q1: <number>" ... "Q10: <number>". Use plain numbers (no units, no commas). Round money to cents.

Q1. A jacket costs $80. It is marked down 25%, and then 10% sales tax is added to the marked-down price. What is the final price in dollars?
Q2. Five friends split a $127.50 restaurant bill and add an 18% tip on the bill. Two of them also ordered dessert, which is already included in the bill. If the total with tip is shared equally, how many dollars does each person pay?
Q3. You put $2,000 in an account that pays 4% interest per year, compounded once a year. How many dollars are in the account after 3 years?
Q4. A car uses 7.2 litres of fuel per 100 km. Fuel costs $1.85 per litre. The road trip is 365 km, and the car is a blue sedan. How many dollars does the fuel cost?
Q5. A bag holds 2.4 kg of flour. A baker uses 3/4 of it, then uses 1/3 of what is left. How many kilograms remain?
Q6. How many days are there from March 3, 2026 to November 18, 2026 (counting from March 3 to November 18, so March 3 to March 4 is 1 day)?
Q7. On Friday Maya picks 44 apples. On Saturday she picks 58. On Sunday she picks double Friday's amount, but 5 of Sunday's apples are smaller than average. How many apples does she pick in total over the three days?
Q8. A notebook and a pen cost $2.30 together. The notebook costs $2.00 more than the pen. How many dollars does the pen cost?
Q9. It takes 6 workers 9 hours to paint 6 identical fences, each worker painting one fence alone. How many hours does it take 18 workers to paint 18 identical fences the same way?
Q10. What is 487 multiplied by 639, minus 12,908?

~~~~

---
## FILE: prompt2.txt

~~~~
Solve each of the 10 problems below. Show brief working if you like, but end your reply with exactly 10 final lines in this format, one per problem: "Q1: <number>" ... "Q10: <number>". Use plain numbers (no units, no commas, no percent sign). Round money to cents and percentages to two decimals.

Q1. What is 48,372 multiplied by 9,146?
Q2. What is 17 to the power of 6?
Q3. How many days are there from November 18, 2026 to February 14, 2028 (counting so that November 18 to November 19 is 1 day)?
Q4. A coat is discounted by 20%, then 15% sales tax is added to the discounted price. The final price is $230. What was the original price in dollars, before the discount?
Q5. A driver goes from town A to town B at 60 km/h and returns the same road at 40 km/h. What is the average speed for the whole round trip, in km/h?
Q6. How many times does the letter "r" appear in total in these three words: strawberry raspberry blackcurrant?
Q7. Two fair six-sided dice are rolled. What is the probability, as a percentage, that the sum is 9?
Q8. Tom is 3 times as old as his sister Ana. In 12 years Tom will be twice as old as Ana. Their dog is 5 years old. How old is Tom now?
Q9. What is the remainder when 1,234,567 is divided by 97?
Q10. You invest $5,000 at 6.5% annual interest, compounded monthly, for 7 years. How many dollars do you have at the end?

~~~~

---
## FILE: protocol.md

~~~~
# Video 8 - math test: protocol (written BEFORE any run, 2026-11-18)

Question: can AI do everyday math reliably? Ten word problems, one prompt, three tools (ChatGPT, Gemini, Claude), one attempt each, fresh chat, no retries, no edits. Claude is included (user ruling 2026-11-18).

The answer key was computed by script (`key.py`) before any tool was run. The prompt is in `prompt.txt` and is identical for every tool.

Design: Q1-Q5, Q10 are plain multi-step arithmetic. Q2, Q4 and Q7 carry an irrelevant detail (distractor). Q6 is date counting. Q8 and Q9 are "trap" problems where the quick answer is wrong (Q8 quick answer 0.30; Q9 quick answer 18). Q8 and Q9 follow well-known puzzle patterns with changed numbers.

## Scoring (decided now, same for all)
- One point per problem (10 total), judged on the final line "Qn: value" only. Working shown is not scored.
- Correct = equals the key (money to the cent; Q5 0.4; others exact). Rounding to the stated precision is accepted; anything else is wrong.
- A missing or unparseable final line = wrong. Matching is done by script (`score.py`).
- Anything notable outside the rubric (wrong working with right answer, formatting breaks) is reported separately, not scored.

## Setups (differences disclosed)
- ChatGPT: free web, logged out, model not shown.
- Gemini: free web, as the pane allows (signed in "Auto" or logged-out Flash-Lite, recorded in answers.md).
- Claude: fresh Sonnet-class agent copy, no tools, not claude.ai, told to reply as a chat assistant and output only its reply.

Limits: one prompt of ten problems, one try each, free tiers, Claude run as an agent copy.

---
## ADDENDUM - Round 2 (written 2026-11-18, after round 1 and BEFORE round 2 was run)

Round 1 result: ChatGPT 10/10, Gemini 10/10, Claude 10/10 (round 1 was too easy to separate the tools). Round 2 is a harder set of 10, added openly after seeing that result; it was not tuned against any tool's answers. Key: `key2.py` (computed by script before the run). Prompt: `prompt2.txt`. Same scoring rules, same setups, one attempt each, fresh chat, no retries. Round 1 stays in the video as it happened.
Round 2 mix: big multiplication (Q1), a power (Q2), date counting across a leap year (Q3), reverse percentage (Q4), average speed (Q5, quick answer 50 is wrong), letter counting (Q6), probability (Q7), age puzzle with a distractor (Q8), modular arithmetic (Q9), monthly compound interest (Q10).
Notable: ChatGPT/Gemini free web may use a built-in calculator or code tool silently, while Claude's agent copy has none; this is a setup difference to be disclosed in the video.

~~~~

---
## FILE: score.py

~~~~
"""Score a tool's reply file against key.py. Usage: python score.py reply.txt"""
import re, sys
from decimal import Decimal as D, InvalidOperation
import os
from importlib import import_module
KEY = import_module(os.environ.get("KEYMOD","key")).KEY
t = open(sys.argv[1], encoding="utf8").read()
got = {}
for m in re.finditer(r"Q\s*(\d+)\s*[:=]\s*\**\s*\$?\s*(-?[\d,]*\.?\d+)", t):
    got[int(m.group(1))] = m.group(2).replace(",", "")  # last one wins
n = 0
for k, v in KEY.items():
    g = got.get(k)
    try: ok = g is not None and D(g) == v
    except InvalidOperation: ok = False
    n += ok
    print(f"Q{k}: key {v}  got {g}  {'OK' if ok else 'WRONG'}")
print(f"TOTAL {n}/10")

~~~~

---
## FILE: script.md

~~~~
# Video 8 - Can AI do everyday math?

3:46. Narration and scenes live in tools/build_video_08.py (narration also in the .srt). Test design, replies and scores: protocol.md, answers.md. Result: 60/60, a tie at the ceiling; round 2 added after round 1 (disclosed).

~~~~

