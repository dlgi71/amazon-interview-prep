# amazon coding interview questions: what the OA and onsite rounds actually ask, how grading works, and a six-week prep plan

Most people searching for Amazon coding interview questions are not looking for another 200-item problem dump. They want to know which questions repeat, how the rounds are structured, and what the grader is actually scoring. So let's start there, then get into the problems themselves.

## What the Amazon process actually looks like

Amazon's loop is short compared to Google or Meta, but it has more moving parts than most candidates expect.

For new grads and interns, it usually starts with the Online Assessment (OA), which Amazon splits into parts:

- **OA1** — debugging and logical reasoning. Typically 5–7 short code snippets with a subtle bug (off-by-one, infinite loop conditions) plus some reasoning questions.
- **OA2** — LeetCode-style coding, usually one or two problems in a timed window.
- **OA3** — work style assessment and logical reasoning. Hypothetical situations where you pick the most "Amazonian" action; reviewing the 14 Leadership Principles first is the standard advice, and it's good advice.

Experienced SDEs typically skip OA1 and go straight to OA2. If you're new grad or intern, expect at least two of the three parts.

Timing varies by the platform you're tested on. On HackerRank it's commonly around 135 minutes; other platforms differ. Two things are consistent: you take a photo of your ID with your webcam at the start, and your browser activity is monitored. There's no human proctor watching live, the session isn't video-recorded, but tab-switching gets flagged. In practice that means you should be fluent in your language's syntax and standard library before the test, not Googling it during.

Then comes the onsite loop. Candidate reports from the last couple of years describe roughly this shape: two or three DSA rounds with two coding questions each, Leadership Principle questions mixed into the same rounds, and a final Bar Raiser round that is largely behavioral but can include a problem. Bar Raiser interviewers sit outside the hiring team and can veto a hire, which is why people who "pass" three technical rounds still get rejected.

## The questions that keep showing up

Amazon's problem set is narrower than Google's. Rather than exotic graph theory, you get repeated shapes: sliding window, heaps, trees/DFS, prefix sums, and light dynamic programming. Coin Change, House Robber, and grid path counting cover most of the DP you'll face at the SDE I / SDE II level.

Problems that appear repeatedly in candidate write-ups and community-compiled lists:

| Category | Frequently reported problems |
| --- | --- |
| Array / hashing | Two Sum (often extended), Product of Array Except Self, Group Anagrams, Subset Sum |
| Sliding window | Longest Substring Without Repeating Characters, Minimum Window Substring, Longest Repeating Character Replacement |
| Heap / top-K | Top K Frequent Elements, Kth Largest Element in an Array, Merge k Sorted Lists |
| Trees | Binary Tree Level Order Traversal, Validate BST, Min Depth / Max Path Sum, Count Good Nodes, Invert Binary Tree |
| Binary search | Search in Rotated Sorted Array, Koko Eating Bananas, First/Last Position of Element in Sorted Array |
| Graphs / BFS-DFS | Number of Islands, Rotting Oranges, Course Schedule II, Flood Fill, Bipartite check |
| DP | Coin Change, House Robber, Jump Game II, unique grid paths with obstacles |
| Design | LRU Cache, LFU Cache, Min Stack, SummaryRanges, expression evaluator |

That last column matters more than the difficulty labels. Amazon's OA problem archive shows a recurring pattern of simulation-plus-greedy questions dressed up in warehouse or logistics language — "Efficient Harvest", "Autoscale Policy, Utilization Check", "Fill The Truck", "Max Profit", "Good Segment", "Decode String Frequency". These are not famous LeetCode problems. They're the same underlying techniques (sliding window, sorting, greedy intervals, string parsing) wrapped in a story about fulfillment centers. If you've only memorized problem names, these will feel unfamiliar.

## How Amazon grades what you write

Getting to a correct solution is maybe half the score in a live round.

The interviewer is watching for a specific flow: restate the problem and clarify constraints before writing anything, name the pattern and the approach, state time and space complexity out loud, then code, then walk through a test case. Candidates who jump straight to typing tend to get steered with hints, which shows up in the debrief.

There's a well-known four-step framing — clarify, plan, implement, test & optimize — and it holds up. In an actual 45-minute round, the clarify phase shouldn't consume ten minutes, but it should exist. Ask about input size, duplicates, negative numbers, whether the array is sorted. Those questions determine whether your O(n log n) answer is fine or whether the interviewer wanted O(n).

Behavioral questions ride along in the same rounds. Two Leadership Principle prompts per technical round is a common pattern, and the follow-ups dig deep — candidates report being asked, in sequence, what the process looked like before a change, whether anything broke after, and what they'd do differently today. Prepare three or four STAR stories with that level of detail ready. A vague story gets dismantled in follow-ups.

## The AI-assisted round Amazon now runs

This is the part of the process that changed most recently. Some employers, Amazon included, have started putting candidates in AI-augmented coding rounds: a sandboxed editor with a built-in AI chat panel, or a paired session where you use AI tooling while an interviewer watches.

AlgoMonster launched a free hub covering exactly this format, with company-by-company breakdowns of tooling for Meta, Shopify, Canva, LinkedIn, Amazon, Microsoft, Stripe, Coinbase and Snowflake. Their published rubric weights problem-solving and algorithm selection at roughly 35–40% of the score, code understanding and quality at 25–30%, verification and debugging at 15–20%, and communication at 15–20%.

The practical takeaway from that weighting: asking the AI to solve the whole problem end-to-end scores badly even when the code compiles. The behavior that scores well is thinking through the approach first, explaining it to the interviewer, prompting for a narrow piece of implementation, then testing the output rather than trusting it. If you go in expecting to prompt your way through, you'll be graded on judgment you didn't demonstrate.

👉 [See how Amazon's AI-assisted coding round is structured and graded](https://algo.monster/ai-coding-interview?fpr=li69)

## Where a question list stops being enough

Search results give you lists. Lists don't tell you which pattern a new problem belongs to at minute three, under pressure.

That's the gap AlgoMonster was built for. It's a text-and-diagram platform created by ex-Google engineers that teaches coding patterns rather than problem volume — each pattern gets an explanation, a code template, and a set of problems mapped to it, so the point is transfer to problems you've never seen. Their Amazon page breaks the OA down by part (OA1/OA2/OA3) and walks through the core patterns behind Amazon's OA and virtual onsite questions, including the FAQ answers about webcam use, timing, proctoring and how solutions are evaluated against open and hidden test cases.

Two things about it are worth knowing before you pay.

First, the fit: no video walkthroughs anywhere. It's reading plus interactive diagrams plus an in-browser editor. If you learn by watching someone solve problems, this will feel like work.

Second, the ceiling: system design coverage is introductory. It's fine for load balancing and caching basics, not enough for a senior system design round. Behavioral content is also shallow. If you're targeting SDE II with a system design component, budget for a separate resource.

What it does have that question dumps don't: pattern-level ROI charts showing which patterns carry the most weight for Amazon specifically, Speedrun mode for timed drills, decision flowcharts for classifying a problem before you code it, and an archive of company-specific OA problems in their forum with real Amazon OA questions going back several years.

👉 [Work through Amazon OA questions on AlgoMonster](https://algo.monster/problems/amazon_online_assessement_questions?fpr=li69)

## AlgoMonster plans and current pricing

AlgoMonster doesn't do month-to-month billing. The paid options are annual or a one-time lifetime purchase, and the site runs promotions frequently enough that the number on the pricing page moves.

| Plan | What you get | Price | Billing | Start |
| --- | --- | --- | --- | --- |
| Free | Limited access to a sample of patterns and problems — enough to judge whether the text-and-diagram format works for you, not enough for real prep | $0 | — | [Try the free tier](https://algo.monster/subscribe?fpr=li69) |
| Pro – Yearly | All patterns, lessons and problems; unlimited Speedrun; unlimited AI Assistant usage; company questions updated monthly; 500+ lessons across 6 courses, 1,000+ illustrations, 3,000+ editorials; bonus Foundation and Build-an-LLM courses; member discount on live bootcamps | ~$99–$119/year (shown as $8.25–$9.92/mo billed annually depending on the active sale) | Annual, 12 months of access | [Get Pro Yearly](https://algo.monster/subscribe?fpr=li69) |
| Pro – Lifetime | Everything in the annual plan plus lifetime updates — one payment, permanent access to current and future content | ~$189–$459 one-time, depending on the promotion running at checkout | One-time | [Get Pro Lifetime](https://algo.monster/subscribe?fpr=li69) |

Those price ranges aren't me hedging. Snapshots of AlgoMonster's own subscribe page from different periods show the annual plan at $99/year and $119/year, and lifetime at $189 and $459, with the discount stated as a percentage off list. The lifetime list price has been advertised as $918 during the $459 promotion. So the checkout page is the only source you should trust on the day you buy — and if a sale is live, that's the moment to take it. Quant Interview Prep, developed with an external partner, is sold separately and isn't included.

Which plan makes sense for an Amazon loop? If your interview is weeks away and you're doing a single focused push, the annual plan is the cheaper commitment. If Amazon is one stop in a longer job hunt — or you're at the stage where you'll interview again in two years for a promotion or an external offer — the math on lifetime flips after roughly one or two renewals, and lifetime buyers keep access to everything added later.

One honest caveat worth flagging: there's no live interview simulation. AlgoMonster builds pattern recognition; it doesn't put a senior engineer on the other side of the screen asking follow-ups for 45 minutes. If your failure mode is freezing under observation rather than not knowing the approach, add mock interviews somewhere else.

👉 [Compare the AlgoMonster plans and lock in the current price](https://algo.monster/subscribe?fpr=li69)

## A six-week Amazon prep plan

The AlgoMonster curriculum is designed to be completed in roughly 4–8 weeks at around 1–2 hours a day. Here's how that maps onto an Amazon-specific timeline.

**Weeks 1–2 — patterns, not problems.** Work through arrays, strings, hashing, two pointers, sliding window, prefix sums, and binary search. For every problem, write down which pattern it belongs to before you touch the editor. If you can't name the pattern in under two minutes, you haven't learned it yet.

**Weeks 3–4 — trees, graphs, heaps, DP basics.** Level order traversal, BST validation, islands, topological sort, top-K with a heap, then the light DP set (Coin Change, House Robber, grid paths). This is where Amazon's problem mix actually concentrates.

**Week 5 — Amazon-specific simulation.** Stop solving famous problems and start solving the OA-style ones: warehouse simulations, string decoding, interval merging, greedy scheduling. Also do at least three timed sessions, because the OA doesn't care that you'd have solved it in another ten minutes. Speedrun mode is built for exactly this.

**Week 6 — behavioral and review.** Write out four STAR stories covering conflict, failure, ambiguity, and a project you owned end to end. Rehearse the follow-up layer — not just what you did, but what broke, what you measured, and what you'd change. Then re-solve the patterns you were slowest on and leave the new material alone.

## Questions people ask before they start

**Do I need to know system design for Amazon?** At SDE I, usually not in depth. For SDE II and above, expect a design round, and AlgoMonster's introductory coverage won't be enough for it.

**Is LeetCode alone enough?** For raw volume, yes. For recognizing which pattern a disguised Amazon problem needs, less so — that's the skill the OA tests, and it's the reason pattern-based prep exists as a category.

**Can I use AI during the Amazon OA?** Your browser activity is monitored. Don't plan on it. In AI-assisted rounds, where an AI panel is provided, your use of that tool is part of the score.

**What if I have two weeks?** Skip volume entirely. Learn the ten patterns that show up most in Amazon OA write-ups, drill them timed, and practice narrating your approach out loud. It's not ideal, but it beats starting a 300-problem list you won't finish.

**How much does prep cost?** AlgoMonster's annual plan sits below a year of LeetCode Premium at list prices, and the lifetime option is a one-time payment. If you're also buying a system design resource and mock interviews, budget for those separately.
