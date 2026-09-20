# For the GPT with scheduler access: how to implement and keep the scheduled-task fleet

Give this whole file to a ChatGPT conversation in the account you want it to manage. It says what exists, what the
GPT must read, what it must do in this account, and how it reports. It does not need to invent anything; every
instruction below points at a file that already exists.

## 1. What exists (2026-09-20)

- **The control repository**: `yspennstate/math-research-brain`, branch `main`, folder `scheduled_tasks/`. Its
  `README.md` holds two owner-edited blocks the whole fleet obeys: OWNER CONTROL (JSON between the markers
  `<!-- OWNER_CONTROL_START -->` and `<!-- OWNER_CONTROL_END -->`: revision, fleet_enabled, mode, target_per_account,
  interval_minutes, paused_accounts, paused_slots, model and reasoning preference, research_queue) and OWNER MESSAGE
  (text between `<!-- OWNER_MESSAGE_START -->` and `<!-- OWNER_MESSAGE_END -->`). Beside it: `PROTOCOL.md` (what a run
  does, how repairs are serialized), `fleet.json` (four logical accounts, twenty roles each), `roles.json` (B01..B20),
  `ONBOARDING.md` (the instruction for accounts 2 to 4), `tools/control.py` (validate, render the task
  specifications, plan a repair), `tests/`, `status/INSTALLATION.json`, and the workers' own folders `runs/`, `work/`,
  `status/`, `leases/`.
- **account01 is enrolled**: twenty tasks named `01 B01 Source transfer` ... `01 B20 Caretaker and acceptance`, each
  hourly, each carrying the marker `BRAIN-FLEET v1 account=account01 slot=Bxx` and reading the control README at every
  run through the GitHub connector. Accounts 02, 03 and 04 are enrollment profiles only until a GPT inside each of
  those accounts enrolls them.
- **The brain-side board**: the owner's other repository, `yspennstate/ai-memories-and-functionality`, folder
  `12_cognitive_architecture/scheduled_tasks/`, holds his local copy of the message (`OWNER_MESSAGE.md`), a sync that
  pushes it into the control README, a rendered `BOARD.md` and `TASK_ROSTER.md`, the wake prompt, a summary of the
  brain for tasks, and `RESULTS.md` for pasted reports. Every agent on his machine sees the board hourly.
- **The public mirror**: https://github.com/yspennstate/brain-tasks-board - raw files at
  `https://raw.githubusercontent.com/yspennstate/brain-tasks-board/main/<file>`: `BOARD.md`, `TASK_ROSTER.md`,
  `PROTOCOL.md`, `roles.json`, `WAKE_PROMPT.md`, `BRAIN_FOR_TASKS.md`, `RESULTS.md`, `README.md`. It is refreshed every
  fifteen minutes from the control README. A task or a GPT that cannot reach the private repository reads these.

## 2. What the GPT reads, every time, before doing anything

1. The control README at the latest `main` commit (through the GitHub connector), both blocks; record the commit and
   the revision. If the connector is not bound in this account, read the public `BOARD.md` instead and say so.
2. `PROTOCOL.md`, `fleet.json`, `roles.json` at the same commit (or the mirror copies).
3. The public `TASK_ROSTER.md` and `RESULTS.md` (what is verified, what other tasks reported).

A later message from the owner in the conversation, or a pause in the control block, outranks everything below.

## 3. What the GPT does in this account

**Bind the account.** State which logical profile this account is (account01 is taken; use account02, account03 or
account04 as the owner names it; a label is not a login). Do not adopt account01 unless the owner says this is that
account.

**Count the fleet.** Obtain one fresh, complete inventory of this account's scheduled tasks. Report, separately: the
active total, the managed count (tasks carrying the `BRAIN-FLEET v1 account=<this profile>` marker), the hourly-valid
count, the missing slots among B01..B20, known owner pauses, the account's observed cap, and evidence of recent runs.

**Enroll or repair, under the lease.** Render this account's twenty specifications:

    python scheduled_tasks/tools/control.py render --root scheduled_tasks --repository yspennstate/math-research-brain --account account02

(or `account03`, `account04`). Before creating anything, take the create-only lease
`scheduled_tasks/leases/<account>/<UTC-hour>.json` in the control repository (a unique nonsecret run id and the
control revision; if it exists, another writer owns the hour: stop and report). Then create the missing slots with the
rendered title, prompt and hourly schedule, update existing managed tasks rather than duplicate them, preserve a valid
hourly offset, never delete an unrelated task, never exceed the account's observed cap, never resume a task the owner
paused. On the first capacity or permission rejection stop that class of change and report the exact error. Append to
every created or updated prompt the paragraph from section 5 (the public mirror and the brain repository).

**Set the settings the tool cannot.** If the scheduler tool exposes no model or reasoning selector, say so; the owner
sets them in the ChatGPT app (schedule every hour; model and reasoning effort the highest offered). Record requested
and observed settings separately; unknown is `UNVERIFIED`.

**Write the receipt.** Commit a sanitized installation receipt under `scheduled_tasks/status/` (counts, cap, slots
created or updated, tool results, limitations) and a run receipt under `scheduled_tasks/runs/<account>/B20/<run>/`.
No account identity, no scheduler ids, no credentials, no machine paths.

**Every hour after that**, the caretaker task B20 repeats the count and the repair; any other scheduler-capable GPT
inspects and reports gaps rather than racing to create tasks.

## 4. How the owner talks to the fleet, and how the fleet answers

The owner edits OWNER MESSAGE (on GitHub, or the brain's `OWNER_MESSAGE.md`, which is pushed for him). Every run
acknowledges the revision and the message hash and reports each of his requests as implemented, in_progress, blocked or
not_applicable, with evidence. A run ends with the receipt of PROTOCOL.md section 7 and the chat block:

    TASK: Bxx  ACCOUNT: accountNN  RUN: <date and time>
    CONTROL: <control commit and revision read, or "public mirror" or "unavailable">
    READ: <which pages loaded>
    RESULT: <what you found or did, exact statements, sources, component statuses>
    NEXT: <what the next run of this slot should do>
    BOARD: <one line answering the owner's current message, or "none">

The owner pastes chat blocks he wants kept into the brain's inbox; connected tasks' receipts are read from the
repository directly.

## 5. The paragraph to append to every task's prompt

> Also read, every run, before working: https://raw.githubusercontent.com/yspennstate/brain-tasks-board/main/BOARD.md
> (the owner's current message and control, rendered from the control README), .../TASK_ROSTER.md (your slot and the
> accounts), .../PROTOCOL.md (how to behave and how repairs are serialized), .../BRAIN_FOR_TASKS.md (what the brain is
> and how to work so your result can be filed) and .../RESULTS.md (what other tasks reported; build on it, do not
> repeat it). If you cannot reach the control repository, these public copies are your control for this run: say so in
> your report, do not mutate schedules, and work on your slot's role. If the brain repository
> yspennstate/ai-memories-and-functionality is connected in your account as well, read its
> `01_ai_consciousness/claude/memory/MEMORY.md` (the index) and the memories your role touches, and cite memory names.

## 6. The rules that do not move

- Nothing invented; every claim sourced; plain human prose; no sentence about your own process in anything meant for
  publication.
- No secrets, account identities, scheduler ids or machine paths in any output or commit. No email, no spending, no
  bypass of a platform limit, no change of visibility or permissions.
- Reading the repository is `SOURCE_ACCESS`; only a real package initialization, memory restoration and a real query in
  this run is `FULL_BRAIN_CONNECTED`. Never label the first as the second.
- A later owner pause or stop wins over the standing "keep twenty running". A count under twenty is reported as a count
  under twenty, with the cap that caused it.

## 7. Facts about ChatGPT scheduled tasks (OpenAI Help Center, read 2026-09-20)

A task cannot run more than once per hour. Active-task caps per account: Free and Go 3, Plus 5, Business and Edu 10,
Pro and Enterprise 15; paused tasks keep their slot. The model and reasoning effort can be set per task in the app. Each
run starts a new chat and can browse, use connected tools and run code.
