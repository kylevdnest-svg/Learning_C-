# C# Learning Plan & Progress Tracker

> Living source of truth for our C# lessons. Update this file **after each assessed lesson** so a fresh chat can resume without guessing.
>
> **Started:** 2026-10-30  
> **Student:** Repository owner  
> **Tutor:** ChatGPT  
> **Language/runtime:** C# with .NET SDK 10.0.302  
> **Version:** 1.0  
> **Last reviewed:** 2026-10-30

## 1. Mission

Become an independent C# developer who can **read, explain, modify, write, test, debug and design** practical software—not merely run code supplied by an AI.

Target applications: business tools, desktop utilities, APIs, databases, and reusable libraries. Prior JavaScript/TypeScript exposure can help with comparisons, but **no C# concept is considered mastered without evidence**.

**Success criterion:** Independently implement and explain a small, tested C# application from a written specification; then build a second, more substantial application using classes, persistence, and well-structured components.

## 2. Teaching agreement (follow this every lesson)

The student learns best through **code-first comprehension and explanation**, rather than being asked to invent syntax that has not been shown.

1. **Read:** Tutor shows a short, runnable C# code sample using previously introduced concepts; identify any truly new syntax before expecting independent use.
2. **Explain:** Student describes what each relevant part does and predicts behavior **before running it**. Accept plain language; do not demand jargon.
3. **Review:** Tutor identifies accurate reasoning, specific misconceptions, and the minimum explanation needed to resolve them. Do not reveal answers until after the attempt.
4. **Modify:** Student makes one small, scaffolded change to the snippet.
5. **Transfer:** Tutor tests the same concept in a new context, then revisits it after a delay.
6. **Build:** Move gradually from modifications to independently authored functions, programs and projects.

Additional rules:
- **Teach before testing.** Never make unintroduced syntax the hidden prerequisite of a graded task.
- Prefer short snippets with an explicit question; only increase complexity when evidence supports it.
- Separate **what the code does** from **whether it is good design**.
- Ask for a trace or predicted output before compiling when useful; running the code becomes verification.
- Include deliberate bug-finding and refactoring **only after the prerequisites** are established.
- Give constructive, specific corrections. Do not infantilize or mistake unfamiliar syntax for weak logic.
- One main learning objective per exercise. Do not overload an exercise with 5 new concepts.
- Student is free to ask clarifying questions at any point; clarification is not a penalty.
- No arbitrary deadlines. Progress is based on demonstrated proficiency, not completed days.
- Keep applications relevant: city-sim credits, invoices, inventories, desktop tools and API logic where appropriate.

## 3. Evidence-based grading

**No score is assigned for enthusiasm, prior exposure, successful tool installation, or merely copying a working example.**

For each graded task, state the task's weighting in advance. Default **code-reading score (/100)**:
- **30 pts — execution trace:** accurately follows order of operations and changing variable values.
- **25 pts — conditions/control flow:** explains when each branch or loop runs.
- **25 pts — predictions:** predicts output and the specified edge-case behavior.
- **20 pts — explanation:** coherent reasoning, even in non-technical language.

For modification/debugging/build tasks, use an explicit task-specific 100-point rubric covering correctness, reasoning, verification, and maintainability. **Do not score criteria that the task did not test.** If a task is diagnostic or coaching-only, mark it **Ungraded**.

**Scoring bands:** 90–100 Strong; 80–89 Solid; 70–79 Developing; 50–69 Needs practice; 0–49 Relearn foundations. Scores describe task performance, not intelligence.

**Concept status:**
- **Not started** — No instruction or evidence yet.
- **Introduced** — Shown/explained, not reliably demonstrated.
- **Practising** — At least one attempt; consistency not yet established.
- **Provisional** — >=85 on one representative independent assessment.
- **Mastered** — >=85 on **two distinct** assessments, at least 24 hours apart, with **at least one modification or original implementation** and no material misconception. An unassessed concept stays unassessed even if neighboring topics pass.
- **Review due** — Previously provisional/mastered but a delayed review is outstanding or performance has slipped.

**After every assessed task**, log: date, task ID, objective, type (read/trace/modify/debug/build), student answer summary, predicted vs actual behavior if relevant, score/rubric, strengths, mistakes, hint level, concept status changes, next review date, and next action. Record factual evidence; never invent results.

Hints: 0 = none; 1 = small conceptual hint; 2 = targeted hint; 3 = guided walkthrough. A >=85 with substantial help is **not** an independent mastery proof.

## 4. Starting point — verified vs unverified

**Verified on 2026-10-30:**
- Windows/PowerShell and VS Code workflow established in chat.
- `dotnet run` works.
- `dotnet --version` reported **10.0.302**.
- Student explicitly prefers **read code → explain behavior → review → modify**.
- Tutor previously introduced `int`, `string`, `bool`, `+=`, `-=`, `Console.WriteLine`, interpolation, and `if/else`.

**Not verified yet:**
- Student's independent predictions, branch tracing, comprehension of expressions, and ability to change C# code.
- Understanding of all introduced material; exposure is **not mastery**.
- No scored C# exercise completed as of this document's creation.

## 5. Curriculum — mastery-driven, not calendar-driven

| ID | Module | Key concepts / reading focus | Practical evidence of learning | State |
|---|---|---|---|---|
| M00 | Tools & program execution | SDK, project structure, Program.cs, compiler vs runtime, dotnet run | Run console app and locate entry point | Introduced (run verified) |
| M01 | Values, variables & expressions | int, double, decimal, string, bool, assignment, operators, interpolation | Trace arithmetic/output, change values safely | Introduced |
| M02 | Decisions & comparisons | if / else if / else, relational & boolean operators, nested conditions | Predict branches and handle boundaries | Introduced (if/else only) |
| M03 | Loops | for, while, foreach, break/continue | Trace repetitions and stopping conditions | Not started |
| M04 | Methods | parameters, return values, void, scope | Explain and extract repeatable logic | Not started |
| M05 | Collections | arrays, List<T>, Dictionary<TKey,TValue>, iteration | Track and update multiple records | Not started |
| M06 | Classes & objects | fields, properties, constructors, encapsulation | Model an account/item with behavior | Not started |
| M07 | Nullability, validation & exceptions | nullable types, guards, try/catch, input validation | Read failure paths and reject bad data | Not started |
| M08 | LINQ & data transformations | Where, Select, OrderBy, aggregates | Read and write data queries | Not started |
| M09 | Files & JSON | paths, streams, serialization, persistence | Save/load app state safely | Not started |
| M10 | Interfaces & composition | contracts, dependency injection, separation of concerns | Swap implementations without changing callers | Not started |
| M11 | Async & HTTP clients | Task, async/await, cancellation, requests, errors | Explain asynchronous work and call an API | Not started |
| M12 | Debugging & tests | breakpoints, stack traces, assertions, xUnit | Diagnose a broken project with tests | Not started |
| M13 | APIs with ASP.NET Core | routing, request/response, DTOs, validation | Build a small REST API | Not started |
| M14 | Databases | SQL concepts, EF Core, migrations, transactions | Persist/query records, explain basic integrity | Not started |
| M15 | Architecture & security basics | layering, configuration, logging, secrets, dependency boundaries | Explain and improve a small real codebase | Not started |
| M16 | Capstone: application | choose backend, desktop or library route | Deliver independently tested app and defend decisions | Not started |

**Optional pathways after M12:** Windows desktop UI (WPF/WinUI or another suitable UI stack), reusable .NET component library, advanced ASP.NET Core, performance and concurrency. Choose based on student interest then; do not derail foundational learning prematurely.

**Milestone A (M01–M04):** Explain and modify small programs without a syntax guide for core control flow.

**Milestone B (M05–M09):** Build a console-based credits/invoice/inventory tracker with collections, validation and JSON persistence.

**Milestone C (M10–M14):** Refactor into services, tests, HTTP API and database-backed storage.

**Milestone D (M15–M16):** Design and build an independent application with documented architecture, error handling, tests and a brief self-review.

## 6. Progress scoreboard

> The row below is a **baseline, not a test result**. Never transform an unassessed item into a numerical zero.

| Measure | Current | Notes |
|---|---|---|
| Overall proficiency score | **Not yet assessed** | Compute only from scored evidence; no baseline score fabricated |
| Exercises assessed | **0** | E001 is pending |
| Concepts mastered | **0 confirmed** | Instruction already received in some concepts |
| Active module | **M01–M02 diagnostic** | Basic expressions and conditions |
| Strongest observed skill | **Not yet measured** | Avoid speculative assessment |
| Current focus | **Trace statement order and explain conditional branching** | See E001 |
| Next action | **Student explains E001 without running it first** | Tutor then reviews and scores |
| Delayed review queue | **Empty** | Populate after independent assessments |

**Optional aggregate:** Once 3+ scored tasks exist, maintain a *rolling average of the most recent five independently completed tasks*. Never present it as a standardized or objective language-proficiency test.

## 7. Current exercise — E001 (PENDING; first diagnostic)

**Objectives:** execution order, variable update, condition, output prediction, edge case.  
**Type:** read / trace / explain.  
**Status:** Pending student response.  
**Hints used:** None recorded.  
**Score:** Not yet assessed.

Read the following **without running it first**:

    int credits = 50000;
    int income = 20000;
    int upkeep = 15000;

    credits += income;

    if (credits >= upkeep)
    {
        credits -= upkeep;
        Console.WriteLine($"Remaining credits: {credits}");
    }
    else
    {
        Console.WriteLine("Insufficient credits!");
    }

Explain, in your own words:
1. What the program does, in order.
2. Why the `if` statement is there.
3. What the console prints with the given values.
4. What changes if `upkeep` is set to `80000`.

**For this diagnostic:** don't assign a surprise score before the student knows the rubric. Use the default reading rubric above, explain it before marking, and distinguish any missing explanation from actual misunderstanding. Review the answer before offering E002.

**Suggested E002 (after review):** Give a *different* short C# program with a small nested condition and ask student to predict output, then modify the condition. Introduce `else if` first if it is used.

## 8. Lesson & assessment log

| Date | ID | Objective / task | Evidence | Score | Hint | Concept outcome / follow-up |
|---|---|---|---|---|---|---|
| 2026-10-30 | SETUP-001 | .NET SDK and console tooling | Student reports `dotnet run` successful and `dotnet --version` = 10.0.302 | Ungraded | — | Environment ready; continue E001 |
| 2026-10-30 | INTRO-001 | Intro to variables, arithmetic, branching | Tutor examples shown; student asked useful questions about income addition and where `if/else` belongs | Ungraded | — | Concepts introduced, not yet demonstrated independently |
| 2026-10-30 | PLAN-001 | Adopt code-reading-first methodology | Student requested code-first explanations and GitHub progress tracking | Ungraded | — | E001 pending |

### Session note template (append each completed session)

**Date:** YYYY-MM-DD  
**Session ID / exercise IDs:**  
**Concepts targeted:**  
**What the student demonstrated (cite answer/behavior, not assumptions):**  
**Score and rubric (or Ungraded):**  
**Hints used:**  
**Misconceptions / friction:**  
**Corrections and feedback given:**  
**Status changes and supporting evidence:**  
**Review on/after:**  
**Next exact exercise / prerequisite:**  

## 9. Tutor handoff protocol (important for new chats)

When continuing C# learning:
1. **Read this file from GitHub first**; it is the canonical learning plan and progress record.
2. Check the current scoreboard, E001 or most recent pending task, recent log, and review queue.
3. Ask the next targeted code-reading question; **do not restart Lesson 1 unnecessarily**.
4. Gather the student's own answer before evaluating it. Do not mark code as mastered merely because it runs.
5. Record the actual assessed result in the scoreboard, curriculum states, current exercise, and session log **and commit the update to GitHub** whenever an assessment is completed. If write access fails, provide the proposed update without claiming it was saved.
6. When a file change is committed, include the relevant path/commit in the response. Preserve earlier assessment history.
7. If the student asks for a different pace or style, update this agreement rather than silently changing course.

### Integrity rules
- No guessed scores, dates, or student responses.
- Never call prior JavaScript/TypeScript experience proof of C# proficiency.
- Keep short reproducible exercises and distinct delayed-review probes.
- Ask whether code was run *before* prediction if it affects assessment fairness.
- Mark tasks requiring substantial help as coached attempts, not independent passes.
- Only record sensitive/personal details when directly necessary for this learning project.

---
**Current stopping point (2026-10-30):** Ready to assess **E001**. The student has not yet supplied an explanation.