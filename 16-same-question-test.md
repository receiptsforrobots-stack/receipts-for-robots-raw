# Video 16 - Do ChatGPT, Gemini and Claude give the same answer every time?
Video: https://youtu.be/oS0WKvi3Jb0


---
## FILE: protocol.md

# Video 16 protocol - Same question, 10 times (written BEFORE any run, 2026-11-25)

## Question
If you ask an AI the exact same question 10 times, in 10 fresh chats, does it give the same answer? Two things are measured: (1) does a question with ONE correct answer get the same, correct answer every time, and (2) does a forced-choice opinion question get the same verdict every time.

## Tools
- ChatGPT (free plan, browser, temporary chat, a brand-new chat per run)
- Gemini (free plan, browser, a brand-new chat per run)
- Claude (a fresh Sonnet-class agent copy per run, no tools, short wrapper: "Do not use any tools. Reply to the user message below exactly as you would to the user directly.")
Claude is included, held to the same prompts and rules, and is a conflict of interest (disclosed).

## The two questions (pasted word for word, identical every run)
Q1 (one correct answer):
"How many days are there from March 3 to September 21 in a non-leap year, not counting March 3 itself but counting September 21? Reply with the number first, then one line of working."
Correct answer: 202 (checked with Python).

Q2 (forced choice, no correct answer):
"I am a total beginner who wants to learn programming. Which should I learn first, Python or JavaScript? Start your reply with exactly one word: Python or JavaScript. Then give one sentence of reasoning."

10 runs of each question per tool = 20 runs per tool, 60 in total. One fresh chat per run. No retries, no follow-ups, replies recorded as shown.

## Scoring (fixed now)
- Q1 score = number of runs (of 10) whose first number is 202. Also record how many DIFFERENT answers appeared.
- Q2 score = size of the majority verdict (of 10). 10 = never changed its mind, 5 = a coin flip. Also record how many different verdicts appeared.
- Main result per tool: Q1 correct (of 10) and Q2 stability (of 10). Tools within one point on a measure are a tie on that measure.
- Not scored but reported: whether the reasoning sentence changed between runs.

## Judgement calls to disclose
- Only two questions, so this says little about other kinds of question.
- Free plans; ChatGPT temporary chats; Gemini normal saved chats unless noted; Claude is agent copies under a wrapper, not the Claude app.
- Runs happen one after another in one sitting; another day could differ.
- I (Claude) wrote the questions. Q2 has no right answer, so it measures stability, not quality.
- Answers are recorded as shown; I do not retry a run.


---
## FILE: answers_claude.md

# Claude (Sonnet-class agent copy, no tools, short wrapper; fresh agent per run; run 2026-11-25). Replies verbatim, one try each, no retries.

## Q1 (correct answer 202)
Run 1: 202. Working: 28 (rest of March) + 30 (Apr) + 31 (May) + 30 (Jun) + 31 (Jul) + 31 (Aug) + 21 (Sep 1-21) = 202.
Run 2: 202. March 3 to Sept 21 is 28 (rest of March) + 30 (Apr) + 31 (May) + 30 (Jun) + 31 (Jul) + 31 (Aug) + 21 (Sept) = 202.
Run 3: 202. Working: 28 (rest of March) + 30 (Apr) + 31 (May) + 30 (Jun) + 31 (Jul) + 31 (Aug) + 21 (Sep) = 202.
Run 4: 202. Working: 28 (rest of March) + 30 (Apr) + 31 (May) + 30 (Jun) + 31 (Jul) + 31 (Aug) + 21 (Sep) = 202.
Run 5: 202. Working: 28 days left in March after the 3rd, plus 30 (Apr), 31 (May), 30 (Jun), 31 (Jul) and 31 (Aug) = 153, plus 21 days in September, so 28 + 153 + 21 = 202.
Run 6: 202. Working: 28 (rest of March) + 30 (Apr) + 31 (May) + 30 (Jun) + 31 (Jul) + 31 (Aug) + 21 (Sep 1-21) = 202.
Run 7: 202. March 3 to Sept 21, not counting March 3: 28 (rest of March) + 30 (Apr) + 31 (May) + 30 (Jun) + 31 (Jul) + 31 (Aug) + 21 (Sep) = 202.
Run 8: 202. Working: 28 (rest of Mar) + 30 (Apr) + 31 (May) + 30 (Jun) + 31 (Jul) + 31 (Aug) + 21 (Sep) = 202.
Run 9: 202. Working: days left in March after the 3rd (28) + April (30) + May (31) + June (30) + July (31) + August (31) + September 1-21 (21) = 202.
Run 10: 202. Working: 28 (rest of March) + 30 (Apr) + 31 (May) + 30 (Jun) + 31 (Jul) + 31 (Aug) + 21 (Sep) = 202.
Q1 SCORE: 10/10 correct. Different answers: 1.

## Q2 (forced choice)
Run 1: Python. Its clean, readable syntax lets you focus on learning core programming concepts instead of fighting punctuation, and it's useful for everything from automation to data work, so you can switch to JavaScript later if you want to build websites.
Run 2: Python. Its clean, readable syntax lets you focus on learning core programming concepts (variables, loops, functions) without fighting extra symbols and quirks, and it's useful for everything from automation to data and AI.
Run 3: Python. Its clean, readable syntax lets you focus on learning core programming concepts instead of fighting punctuation, and it's useful for everything from automation to data and AI, so you can pick up JavaScript later if you want to build websites.
Run 4: Python. Its syntax is clean and close to plain English, so a beginner can learn core programming concepts without fighting punctuation or browser setup, and the skills carry over to web, data and automation work later.
Run 5: Python. Its clean, readable syntax lets you focus on learning core programming concepts like variables, loops, and functions without fighting confusing quirks, and you can move on to JavaScript later once those basics are solid.
Run 6: Python. Its syntax reads close to plain English and has fewer quirks than JavaScript, so you can focus on learning core ideas like variables, loops and functions before moving on to anything else.
Run 7: Python. Its clean, readable syntax lets you focus on learning core programming concepts without fighting punctuation or quirks, and it's useful for almost everything from automation to data and AI, so you can pick up JavaScript afterward if you want to build websites.
Run 8: Python. It has simple, readable syntax that lets you focus on learning core programming concepts first, and it's useful for many things (automation, data, AI, and general scripting), so you can pick up JavaScript later if you want to build websites.
Run 9: Python. Its syntax reads close to plain English and has little extra punctuation, so you can focus on learning core ideas like variables, loops, and functions before moving on to JavaScript later.
Run 10: Python. Its syntax is clean and close to plain English, so you can focus on learning how to think like a programmer instead of fighting punctuation, and it's useful for everything from automation to data work to web backends.
Q2 SCORE: 10/10 majority verdict (Python). Different verdicts: 1. The reasoning sentence was worded differently every run, but the same idea (readable syntax, fewer quirks) each time.

Note: run order above follows the agents' run numbers, not the order they finished.


---
## FILE: answers_chatgpt.md

# ChatGPT (free, signed in on the user's Chrome, temporary chat, brand-new chat per run; run 2026-11-26). Replies as shown, one try each, no retries. Read from the page text after each run.

## Q1 (correct answer 202)
Run 1: 202 days. Working: 28 (March) + 30 + 31 + 30 + 31 + 31 + 20 (September) = 201 days.   [first number 202, but its own working line ends in 201 and uses 20 for September - self-contradictory; counted correct by the protocol rule "first number", flagged here]
Run 2: 202. Working: 28 (March 4-31) + 30 + 31 + 30 + 31 + 31 + 21 = 202 days.
Run 3: 202 days. Working: 28 + 30 + 31 + 30 + 31 + 31 + 21 = 202 days
Run 4: 202 days. Working: 28 (March) + 30 + 31 + 30 + 31 + 31 + 21 = 202 days.
Run 5: 202 days. Working: 28 (March 4-31) + 30 + 31 + 30 + 31 + 31 + 21 = 202 days.
Run 6: 202 days. Working: 28 (March 4-31) + 30 + 31 + 30 + 31 + 31 + 21 = 202 days.
Run 7: 202 days. Working: 28 (March 4-31) + 30 + 31 + 30 + 31 + 31 + 21 = 202 days.
Run 8: 202 days. Working: 28 (March 4-31) + 30 + 31 + 30 + 31 + 31 + 21 = 202 days.
Run 9: 202 days. Working: 28 (March 4-31) + 30 + 31 + 30 + 31 + 31 + 21 = 202 days.
Run 10: 202 days. Working: 28 (March 4-31) + 30 + 31 + 30 + 31 + 31 + 21 = 202 days.
Q1 SCORE: 10/10 first number 202. Different first numbers: 1. One run (1) had a working line that contradicted its own answer (201).

## Q2 (forced choice)
Run 1: Python. Python has simpler, more beginner-friendly syntax, so you can focus on learning programming fundamentals without getting overwhelmed by complicated code.
Run 2: Python. Python has simpler, more readable syntax, making it easier for complete beginners to learn programming fundamentals while building useful projects.
Run 3: Python. Python has simpler, more beginner-friendly syntax, so you can focus on learning programming fundamentals before tackling more complex concepts.
Run 4: Python. Python has simpler, more readable syntax, making it easier for complete beginners to learn programming fundamentals while building useful projects quickly.
Run 5: Python. Python has simpler, more beginner-friendly syntax, so you can focus on learning programming fundamentals without getting overwhelmed by complicated code.
Run 6: Python. Python has simpler, more beginner-friendly syntax, so you can focus on learning programming fundamentals without getting overwhelmed by complex code.
Run 7: Python. Python has simpler, more readable syntax for beginners, letting you focus on learning programming fundamentals without getting overwhelmed by complex code.
Run 8: Python. Python has simpler, more readable syntax, making it easier for beginners to learn programming fundamentals while building useful projects.
Run 9: Python. Python has simpler, more readable syntax for beginners, letting you focus on learning programming fundamentals before tackling more complex concepts.
Run 10: Python. Python has simpler, more beginner-friendly syntax, so you can focus on learning programming fundamentals without getting overwhelmed by complicated code.
Q2 SCORE: 10/10 majority verdict (Python). Different verdicts: 1. The reasoning sentence varied only in a few words (same idea each time).

TOTAL ChatGPT: Q1 10/10 (first number), Q2 10/10.


---
## FILE: answers_gemini.md

# Gemini (free, Auto, signed in on the user's Chrome; run 2026-11-26). NORMAL chats (not temporary), a brand-new chat per run, one try each, no retries. Replies as shown (page text; Gemini's math formatting sometimes splits a line across lines, joined here).

## Q1 (correct answer 202)
Run 1: 202. (31 - 3) in March + 30 in April + 31 in May + 30 in June + 31 in July + 31 in August + 21 in September = 28 + 30 + 31 + 30 + 31 + 31 + 21 = 202 days.
Run 2: 202. 28 (Mar) + 30 (Apr) + 31 (May) + 30 (Jun) + 31 (Jul) + 31 (Aug) + 21 (Sep) = 202 days.
Run 3: 202. 28 (Mar) + 30 (Apr) + 31 (May) + 30 (Jun) + 31 (Jul) + 31 (Aug) + 21 (Sep) = 202
Run 4: 202. 28 (March) + 30 (April) + 31 (May) + 30 (June) + 31 (July) + 31 (August) + 21 (September) = 202 days.
Run 5: 202. 28 (March) + 30 (April) + 31 (May) + 30 (June) + 31 (July) + 31 (August) + 21 (September) = 202 days.
Run 6: 202. 28 (March) + 30 (April) + 31 (May) + 30 (June) + 31 (July) + 31 (August) + 21 (September) = 202 days.
Run 7: 202. 28 (Mar) + 30 (Apr) + 31 (May) + 30 (Jun) + 31 (Jul) + 31 (Aug) + 21 (Sep) = 202 days.
Run 8: 202. 28 (March) + 30 (April) + 31 (May) + 30 (June) + 31 (July) + 31 (August) + 21 (September) = 202 days.
Run 9: 202. 28 (March) + 30 (April) + 31 (May) + 30 (June) + 31 (July) + 31 (August) + 21 (September) = 202.
Run 10: 202. 28 (March) + 30 (April) + 31 (May) + 30 (June) + 31 (July) + 31 (August) + 21 (September) = 202 days.
Q1 SCORE: 10/10 correct. Different answers: 1. Working lines all consistent with the answer.

## Q2 (forced choice)
Run 1: Python. Python uses clean, readable syntax that lets beginners focus on core programming logic before tackling web browser quirks and asynchronous behavior.
Run 2: Python. Python has clean, readable syntax that lets complete beginners focus on core programming logic rather than punctuation and setup details.
Run 3: Python. Its clean, readable syntax and wide versatility make it easier to grasp core programming concepts while letting you build scripts, data projects, or backend tools right away.
Run 4: Python. Python's clean, readable syntax lets you focus on core programming logic rather than punctuation and boiler-plate code.
Run 5: Python. Its clean, readable syntax lets you focus on core programming logic rather than punctuation and boilerplate code.
Run 6: Python. Its clean, readable syntax lets you focus on core logic and problem-solving before dealing with browser quirks or complex language rules.
Run 7: Python. Its clean, English-like syntax and immediate feedback loop let you focus on core programming logic rather than punctuation and browser setup.
Run 8: Python. Its clean, readable syntax lets you focus on core programming logic rather than punctuation rules.
Run 9: Python. Python features clean, readable syntax that lets complete beginners focus on core logic and problem-solving before tackling complex language mechanics.
Run 10: Python. Python offers clean, readable syntax that lets beginners focus on core programming logic before tackling web browser quirks and asynchronous behavior.
Q2 SCORE: 10/10 majority verdict (Python). Different verdicts: 1. Reasoning sentence reworded every run, same idea (clean readable syntax, focus on logic).

TOTAL Gemini: Q1 10/10, Q2 10/10.

Note: unlike ChatGPT, these were normal (saved) chats, not temporary chats; the account has older chats from this channel's tests in its history. Each run was a brand-new chat.


---
## FILE: results.md

# Video 16 results - FINAL (all three tools, 20 runs each, run 2026-11-25 (Claude) and 2026-11-26 (ChatGPT, Gemini)). Protocol: protocol.md (written before any run).

## Scores
| Tool | Q1: first number was 202 (of 10) | Different Q1 answers | Q2: majority verdict (of 10) | Different Q2 verdicts |
|---|---|---|---|---|
| ChatGPT (free, temporary chats) | 10 | 1 | 10 (Python) | 1 |
| Gemini (free, Auto, normal chats) | 10 | 1 | 10 (Python) | 1 |
| Claude (20 fresh Sonnet-class agent copies) | 10 | 1 | 10 (Python) | 1 |

Protocol rule: within one point = a tie. Result: a three-way tie, 10/10 on both questions, for every tool. Nobody changed its answer or its verdict in 10 fresh chats.

## What did vary (not scored)
- Wording: the reasoning sentence on Q2 was reworded in every tool (ChatGPT only in a few words, Claude and Gemini more), but the idea stayed the same.
- ChatGPT Q1 run 1: gave "202 days" first, but its working line used 20 for September and ended "= 201 days". The first number was right, so it counts as correct under the protocol, but its own working contradicted it. This was the only wobble in 60 runs.
- Working lines differed in style (how March was written, whether September was 21 or "Sep 1-21") but all added to 202 except the one above.

## Judgement calls / caveats to report
- Only two questions, both easy for current models. A harder or more ambiguous question could show real variation (published studies find answer drift on harder prompts and on lists/recommendations).
- Q2 has no right answer, so 10/10 means stable, not good.
- Claude ran as fresh agent copies under a short wrapper, not the Claude app. Claude is a conflict of interest.
- ChatGPT: temporary chats on the free plan. Gemini: normal saved chats (account has older chats from this channel); not temporary.
- Runs were done one after another in one sitting per tool; a different day could differ. Claude ran 2026-11-25, ChatGPT and Gemini 2026-11-26.
- I (Claude) wrote the questions.
- Fresh chats isolate each run from the others, but a tool might still have been influenced by account memory/personalisation on ChatGPT/Gemini; I did not check or turn it off.

