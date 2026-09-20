# The board: what Yitzchak is telling the scheduled tasks and every agent

This is a rendering of the single source the tasks read: `scheduled_tasks/README.md` on the main branch of the
math-research-brain repository (control commit d0359634a396). The owner edits it there, or in the brain's local copy
`OWNER_MESSAGE.md`, which the sync pushes within fifteen minutes. His later words win over an earlier task.

control: revision 2026-09-20.3, mode BRAIN_FIRST, fleet_enabled True, target 20 per account every 60 minutes, paused accounts [], paused slots {}, research queue 0 entries

## OWNER MESSAGE

2026-09-20 20:2x, to every scheduled task and every GPT that can see the task lists: the full-brain implementation guide is now in this repository at scheduled_tasks/FULL_BRAIN_GUIDE.md, its account editions are under scheduled_tasks/onboarding/ (README_ACCOUNT02.md, README_ACCOUNT03.md, README_ACCOUNT04.md), and the twenty node-firing acceptance tests are listed in scheduled_tasks/node_firing_acceptance.json. Implement the guide. Full integration includes the real node activation and reflex mechanisms, not only file access or mathematical retrieval. Preserve the complete approved network, compatible sidecars, selective firing and silence rules, deduplication, node attachments and authorized persistent state. Show actual path and trigger evidence in both interactive and scheduled runs. Distinguish the two engines and keep private non-mathematical material excluded. Do not mark the whole brain connected while a required firing component is only described, mocked or observe-only. Every report now carries a FIRING line (which of the twenty tests ran, with the seeds, paths, gates and reflexes observed, or the exact blocker) and a DELIVERY line (the committed artifact paths or the precise save failure), together with the task number.

2026-09-20 19:5x, to every scheduled task connected to the brain and to every GPT that can see the task lists: I want all of you working on implementing the full brain in your respective GPT environments and in the full GPT environment. Every task records its number, the slot and account it runs as, and what it is doing, in every run receipt and in every report, so that we can count how many are working and what each one is working on; the keepers count them every hour and report the count, and a count under twenty is reported as a count under twenty.

Maintain a target of 20 enabled hourly brain tasks in each of my four separately authorized GPT accounts, for 80 in total. Use the highest computational and reasoning settings actually available within platform limits. First finish implementing, connecting, and independently testing the complete brain environment. Every worker must attempt real brain initialization at startup and record what actually worked. Once the required environment is genuinely operational, use it to solve externally sourced mathematical problems and improve the brain. Preserve existing research; do not relabel unfinished work as solved.

Read this control area on every run, acknowledge its revision and content hash, implement the instructions rather than merely summarize them, and preserve useful tested work for the other workers. Every GPT with scheduler access should check that its own account is correctly provisioned; repairs use the caretaker protocol to avoid duplicates. Keep me informed through the shared run reports and task conversation. Do not send email, spend money, use unrelated private information, bypass platform limits, or override a later pause or stop.

## Where the rest is

- Roles, accounts and what is verified: `TASK_ROSTER.md` (from fleet.json and roles.json).
- How a task must behave every run and how repairs are serialized: `PROTOCOL.md` (copy) in the control repository.
- The prompt a task is given: `WAKE_PROMPT.md`. What the brain is: `BRAIN_FOR_TASKS.md`. What tasks reported: `RESULTS.md`.
- Public copies of these files: https://raw.githubusercontent.com/yspennstate/brain-tasks-board/main/<file>
