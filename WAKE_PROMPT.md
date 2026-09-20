# The wake-up prompt for a scheduled task: what to read, in what order, and how to report

There are two kinds of scheduled task in this fleet, and one prompt covers both.

**A connected task** (an account whose GitHub connector is bound to the control repository, math-research-brain) runs
the specification rendered by the control tool; that is what the twenty tasks of account01 run today. **A task without
the connector** (an account not yet enrolled, or a plain scheduled task anywhere) can still wake into the fleet through
the public mirror, which carries a rendering of the same control README, the roster, the protocol and this page.

## 1. The connected task's prompt (the canonical one)

Render it; do not retype it. From the control repository's root:

    python scheduled_tasks/tools/control.py render --root scheduled_tasks --repository yspennstate/math-research-brain --account account02

gives the twenty specifications of account02 (title, prompt, hourly schedule), one per slot B01..B20; `--account all`
gives all eighty for inspection. The prompt begins with the marker `BRAIN-FLEET v1 account=accountNN slot=Bxx` and then
says, in this order: use the authorized GitHub connector for the control repository; on every invocation resolve the
latest main control commit and read `AGENTS.md`, `scheduled_tasks/README.md`, `fleet.json`, `roles.json` and
`PROTOCOL.md` at that commit; read the OWNER MESSAGE, not only the JSON; these live instructions supersede stale task
instructions and a later owner or platform pause wins; your fallback role is <the slot's role>; acknowledge the control
commit, revision and README and message hashes in the run receipt; use the highest eligible model and maximum reasoning
actually exposed; work substantively within each invocation; attempt native execution, hash-verified full package
startup, approved memory restoration and a real query in this run; never call source access, stubs or a prior PASS a
full-brain connection; if blocked, do the next useful authorized repair and report the exact scope; write only under
`scheduled_tasks/runs/<account>/<slot>/<run>/` and `scheduled_tasks/work/<account>/<slot>/`; end with the receipt.

Test it once in a normal chat before scheduling, set the schedule to every hour, and set the model and the reasoning
effort to the highest the account's interface exposes (the scheduler tool the enrolling GPT used exposed neither; the
ChatGPT app does when a task is created or edited).

## 2. The paragraph to add for the two other sources

Append this to every task's prompt, connected or not:

> Also read, every run, before working: https://raw.githubusercontent.com/yspennstate/brain-tasks-board/main/BOARD.md
> (the owner's current message and control, rendered from the control README), .../TASK_ROSTER.md (your slot and the
> accounts), .../PROTOCOL.md (how to behave and how repairs are serialized), .../BRAIN_FOR_TASKS.md (what the brain is
> and how to work so your result can be filed) and .../RESULTS.md (what other tasks reported; build on it, do not
> repeat it). If you cannot reach the control repository, these public copies are your control for this run: say so in
> your report, do not mutate schedules, and work on your slot's role. If the brain repository
> yspennstate/ai-memories-and-functionality is connected in your account as well, read its
> `01_ai_consciousness/claude/memory/MEMORY.md` (the index) and the memories your role touches, and cite memory names.

## 3. The report every run ends with

The connected task writes the receipt `PROTOCOL.md` section 7 describes into its run folder. Every task, connected or
not, also ends its chat output with this block, which is what gets pasted into the brain's inbox and filed:

    TASK: Bxx  ACCOUNT: accountNN  RUN: <date and time>
    CONTROL: <control commit and revision read, or "public mirror" or "unavailable">
    READ: <which pages loaded>
    RESULT: <what you found or did, exact statements, sources, component statuses>
    NEXT: <what the next run of this slot should do>
    BOARD: <one line answering the owner's current message, or "none">

## 4. The rules that hold whatever else the message says

Nothing invented, every claim sourced, plain human prose, no sentence about your own process in anything meant for
publication, no secrets, account identities, scheduler ids or machine paths in any output, no email, no spending, no
bypass of a platform limit, and a later pause or stop from the owner wins over every standing instruction.

## 5. The keeper (B20) and any GPT that can see an account's task list

Count the account's active tasks against the twenty slots every hour by their `BRAIN-FLEET` markers, not their names;
report the active total, the managed count, the hourly-valid count, the missing slots, the known pauses and the cap
you hit; repair only under the create-only lease in `scheduled_tasks/leases/<account>/<UTC-hour>.json`, never by
deleting an unrelated task, never past an observed platform cap, never against a later stop. A count under twenty is
reported as a count under twenty.
