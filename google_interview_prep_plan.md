# Your Google Interview Prep Plan

*Synthesized from the 6 files you uploaded — de-duplicated, fact-checked, and turned into something to actually work through. The companion file, `google_prep_tracker.xlsx`, is the checklist; this is the "why" and "how."*

## First, a heads-up on what you actually sent

- **Two of the files are identical.** `Google_Questions_Part1.pdf` and `Top_google_question_part-1.pdf` are byte-for-byte the same document. Together with "Part 2," they form one continuous set of **~140 Google-tagged problems with full worked C++ solutions** (dated ~2020 — solid as a reference approach, though not necessarily the most idiomatic solution by today's standards).
- **The infographic and the pasted "Most people approach LeetCode wrong" text say the same thing** — one's a graphic, one's the write-up, both describing the same 15-pattern framework. No new information between them.
- **`Google_Tagged_LeetCode_Problems__.pdf` ("SDE Sheet")** is a flat list of 457 problems reportedly asked at Google in the last 6 months — real, useful coverage data, but just a wall of numbers on its own.
- **`Google_Interview_Guide.pdf`** has a solid behavioral-prep framework, but its process/leveling/salary details are outdated — corrected below and in my reply.

I cross-referenced the 457-problem sheet against your worked-solutions set: **80 of the 457 tagged problems already have a full solution sitting in your files.** That's your cheapest starting point — start there before writing anything from scratch.

## How Google's process actually works (2026)

Worth knowing since the guide's overview is a few years stale:

- **Levels are L3–L9, not "T3–T11."** L3 = entry/new grad, L4 = mid-level (2-5 yrs), L5 = senior (leads projects, full system design round), L6+ = staff and above.
- **There's a step the guide doesn't mention at all:** a mandatory online "Google Hiring Assessment" (~50 situational/work-style questions, added 2022) that happens *before* your first human interview.
- **Interviews have been virtual since 2020** — recruiter screen → hiring assessment → technical phone screen (shared coding doc over Google Meet) → onsite loop → hiring committee (people who never met you) makes the final call.
- **System design is mostly an L5+ thing.** At L3/L4 the loop is almost entirely coding rounds (2-4) plus one behavioral/"Googleyness" round — design, if it comes up at all, is a few minutes inside a coding round, not its own interview. This matters for how you allocate prep time below.
- Comp and level-mix specifics vary by team and location, so confirm with your recruiter once you're in the process rather than planning around the guide's numbers.

## The strategy: patterns, not volume

The core idea in your infographic is right, and it's not just marketing: most coding-round problems are a small set of underlying techniques wearing different costumes. Grinding hundreds of problems teaches you to recognize *specific* problems; working pattern-by-pattern teaches you to recognize the *shape* of a new one — which is what actually transfers under interview pressure.

The three-phase approach from your materials is a good structure:

1. **Recognition (per pattern):** solve 3-5 Easy problems in that pattern, then write the template in your own words before moving on.
2. **Application:** solve Mediums *without* being told the pattern first. If you can't identify it, that's the signal to go back — not to push forward.
3. **Mixing:** Hard problems that combine 2-3 patterns, done under a 35-40 minute clock, explaining your approach out loud as you go.

**One caveat on "just these 15":** they cover most of what shows up, but not all of it. Your own 457-problem sheet has real clusters the 15 patterns don't name — "design a class" problems especially (LRU Cache is practically a Google mascot at this point), plus general graph traversal, backtracking-on-a-board, prefix sums, and a few smaller ones. See the **"Beyond the 15"** tab in the tracker — same treatment, 78 more problems, worth working through after the core 15 rather than instead of them.

## A realistic timeline

Your files gave two different numbers (6 weeks vs. 12) because they're answering different questions — one is "how do I learn the patterns," the other is the *full* Google loop including system design and OS topics. Reconciled, and adjusted for the L3/L4-vs-L5 split above:

| Weeks | Focus |
|---|---|
| 1–6 | Work the 15 patterns, phases 1→2→3 as above. This is the core of the plan regardless of level. |
| 7–8 | **Only if you're L5+ track (or unsure):** system design fundamentals. Skip or skim if you're L3/L4 — it's not what gets tested. |
| Throughout | Draft 3-4 behavioral stories in week 1, don't leave this for the end. Revisit and tighten weekly. |
| Final week | Timed mixed-pattern practice + at least one full mock interview, explaining your reasoning out loud. |

## Your pattern-by-pattern plan

`google_prep_tracker.xlsx` has the full checklist (77 curated problems pulled from your own 457-tagged list, sorted into the 15 patterns, each flagged if a solution's already in your files) plus the complete 457 as a second tab for reference. Summary:

| Pattern | Problems in your plan | Already solved in your files |
|---|---|---|
| Two Pointers | 10 | 2 |
| Sliding Window | 7 | 1 |
| Fast & Slow Pointers | 4 | 0 |
| Merge Intervals | 6 | 2 |
| Cyclic Sort | 1 | 1 |
| In-place LinkedList Reversal | 2 | 0 |
| Tree BFS | 2 | 1 |
| Tree DFS | 7 | 2 |
| Two Heaps | 1 | 0 |
| Subsets | 7 | 3 |
| Modified Binary Search | 5 | 2 |
| Top K Elements | 6 | 1 |
| K-way Merge | 3 | 1 |
| Dynamic Programming | 12 | 7 |
| Topological Sort | 4 | 1 |

Two patterns (Cyclic Sort, Two Heaps) are thin in your specific tagged list — that's a real reflection of how often Google asks them lately, not a gap in the curation. One well-chosen problem is enough to internalize the template either way.

## Behavioral prep, condensed

Your guide's framework holds up. The gist: Google asks about past experiences, hypothetical situations, and values — and grades on whether you can explain your reasoning, not just the outcome. Have a real (not rehearsed-sounding) answer ready for each of these themes, ideally 2-3 stories each so you're not reusing the same one:

- Your day-to-day workflow and how you work with a team
- A time you took a risk and it didn't pan out — what you did next
- Something you're genuinely proud of, and what it says about how you work
- Something complex you understand well enough to teach someone else
- How you'd expect to contribute if you joined
- Working in an unstructured or ambiguous situation
- What you'd change about a tool or product you use, and why
- What "fitting the culture" means to you, in your own words, not jargon
- A weak spot or stressor you're self-aware about

Write these down, say them out loud (to a friend or a recording), and focus on *why* you made each call — that's what's actually being graded.

## OS & concurrency — you're closer than the guide assumes

The "week 11" concurrency content in your guide is real interview territory, and you're not starting from zero: deadlocks from blocking on async calls, `lock`/`Monitor` semantics, and where `finally` guarantees break down are the same underlying ideas interviewers probe, regardless of language. The concepts transfer cleanly.

What doesn't transfer automatically is the vocabulary — Google's preferred interview languages are Java, C++, Python, or Go, not C#. Worth doing a handful of concurrency-flavored problems directly in whichever of those you pick, so translating `async`/`await` thinking into that language's idioms isn't happening for the first time under interview pressure.

## A few things that actually matter

- **Say your thought process out loud**, even the parts that seem obvious. It's how they evaluate reasoning, not just the final answer.
- **Ask clarifying questions before coding** on open-ended prompts — treated as a sign of strength, not slowness.
- **Know your Big-O for whatever you just wrote**, and be ready to say it unprompted.
- **If you finish early, don't just sit there** — look for edge cases, optimizations, or bugs.
- Given your production background with distributed systems, event-driven infra, and Kubernetes — if you do end up in a system-design round, that's real material to draw on, not something to build from scratch. Worth confirming with your recruiter early which level they're targeting you for, since that's what determines how seriously to prep design at all.
