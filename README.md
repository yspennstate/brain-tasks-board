# The scheduled tasks: eighty GPT tasks that wake into the brain, and the one place you talk to them from

Owner order, 2026-09-20 18:37 (his clock), in his words: *"i want a read me about the scheduled tasks, and i want that
every gpt here wakes up connected to the full brain, also there should be 80 scheduled tasks running at any time, on 4
different gpt accounts that i have ... any gpt that has access to the scheduled tasks should always make sure that the
full amount in this account (20 of them) is running full time every hour, solving problems, improving the brain,
connecting the brain and so on. they should run on the highest computational max thinking that they can. also there
should be a part of the read me that i can change to talk to all the scheduled tasks and to the gpts that have access to
the scheduled tasks to read this read me whenever they run ... have a whole tasks thing in the brain that the schedules
keep reading, that agents like you keep reading, and that i can update"* - and, 18:5x: *"build on top of this and the 3
documents"*, the control system a GPT session installed the same day.

## The one place

The tasks read **`scheduled_tasks/README.md` on the main branch of the math-research-brain repository** (the control
repository) at every run: an OWNER CONTROL block (JSON: mode, target per account, cadence, pauses, reasoning
preference, research queue) and an OWNER MESSAGE block (his words to the whole fleet). Twenty tasks in account01 were
enrolled on that file on 2026-09-20 15:4x UTC and read it through the GitHub connector at every invocation.

He edits it in either of two places, and they stay in step:

- **on GitHub**, the control README itself, between the markers (`OWNER_MESSAGE_START/END`; the JSON between
  `OWNER_CONTROL_START/END`, revision bumped);
- **in the brain**, this folder's `OWNER_MESSAGE.md`: plain text, his message only. The sync pushes it into the
  control README as a new revision within fifteen minutes (or at once: `python board_sync.py`). If both changed since
  the last sync, GitHub wins and the local text is kept as `OWNER_MESSAGE.conflict.md`; the log says so.

From the control README the sync renders `BOARD.md` (the control summary and his message), `TASK_ROSTER.md` (the
accounts and the twenty roles from `fleet.json` and `roles.json`), and copies of `PROTOCOL.md` and `roles.json`; the
publisher mirrors these with `WAKE_PROMPT.md`, `BRAIN_FOR_TASKS.md` and `RESULTS.md` to the public repository
**https://github.com/yspennstate/brain-tasks-board** (raw files under `.../main/<file>`) so that a task in an account
without the connector, and any agent anywhere, reads the same words. Every Claude and Codex session on his machine
gets the control line and his message once an hour through the `[owner-board]` hook.

## The full-brain guide (owner, 2026-09-20 20:1x)

His GPT wrote the implementation guide for the accounts on 2026-09-20 20:0x and he asked (20:1x, *"read all the files
i just downloaded and help the brain and agent implement it"*) that it be implemented. The guide is
`FULL_BRAIN_GUIDE.md` in this folder and `scheduled_tasks/FULL_BRAIN_GUIDE.md` in the control repository; the three
account editions (the same text under a binding header naming account02, 03 or 04 and that account's focus) are under
`onboarding/`; he pastes an account's edition into a conversation in that account, and that conversation enrolls the
account's twenty tasks under the protocol. The guide separates the two engines (the typed claim graph of the math_brain
package and the memory engine of brain.py and spread_recall.py), names the twenty node-firing acceptance tests
(F01-F20, `node_firing_acceptance.json`, every one NOT_TESTED until a run records evidence in its own receipt), adds
FIRING and DELIVERY lines to the report block in `WAKE_PROMPT.md`, and lists the private operational folders the
workers write to (`scheduled_tasks/runs`, `work`, `status`, `leases`). The runtime side (source transport, export
manifests, adapters, tests) is code work owned by the Codex integration thread of the same evening; this folder holds
the control layer only. The guide and the acceptance list are published to the mirror; the account editions are not.

## What a ChatGPT scheduled task is (read 2026-09-20)

From OpenAI's Help Center article "Scheduled tasks in ChatGPT" and the ChatGPT docs on automations: a task is a prompt
ChatGPT runs on a schedule, each run in a **new chat**; **a task cannot run more than once per hour** (hourly is "full
time" here); **active-task limits per account are Free and Go 3, Plus 5, Business and Edu 10, Pro and Enterprise 15**
(paused tasks keep their slot); **the model and the reasoning effort can be chosen explicitly** in the app when a task
is created or edited (the scheduler tool the enrolling GPT used exposed neither selector, so those twenty carry
"requested highest, observed UNVERIFIED"); a task can browse, use connected tools and run code. The order says twenty
per account; the largest cap we could read is fifteen. The control keeps the target at twenty, and the keeper fills an
account to its real cap and reports the cap it hit rather than silently running fewer.

## The fleet: four accounts, twenty roles each

`fleet.json` desires 4 accounts x 20 tasks = 80 hourly registrations; `roles.json` names the twenty roles every account
carries (B01 source transfer ... B19 end-to-end integration, B20 caretaker and acceptance), and gives each account a
focus: account01 implementation, account02 independent validation, account03 portability and reproduction, account04
adversarial acceptance. The mode is `BRAIN_FIRST` until the full math-brain runtime is genuinely operational; `MIXED`
and `RESEARCH` bring in problem solving from the research queue after that gate. Only account01 has been observed (20
enabled, hourly). Accounts 2 to 4 are enrolled from inside each account with the instruction in the control
repository's `ONBOARDING.md`; a label is not a login, and generating specifications creates no task.

## The keeper rule

*"any gpt that has access to the scheduled tasks should always make sure that the full amount in this account (20 of
them) is running full time every hour"*: B20 in each account, and any GPT or person who can see that account's task
list, counts the active tasks against the twenty slots every hour by their `BRAIN-FLEET` markers, creates or resumes the
missing ones from the rendered specifications, and repairs only under the create-only hourly lease `PROTOCOL.md`
describes: never by deleting an unrelated task, never past an observed platform cap, never against a later pause or
stop. A count under twenty is reported as such. A fully paused fleet cannot wake itself; that takes his interactive
action.

## Waking connected to the brain

Three levels. Every task, always: the public mirror. A connected task: the control repository through its GitHub
connector (the tasks of account01 today). The full brain: the brain repository `yspennstate/ai-memories-and-functionality`
through the same connector once he connects it in an account; `WAKE_PROMPT.md` carries the paragraph to add. The GPTs on
his machine (Codex sessions) wake connected through the Codex hooks, which emit JSON for Codex since 2026-09-20 18:0x.

## The way back

A connected task writes its receipt under `scheduled_tasks/runs/<account>/<slot>/<run>/` in the control repository
(PROTOCOL.md section 7). Every task also ends its chat output with the report block in `WAKE_PROMPT.md`; paste it into
`inbox/` here and run the ingest script, which files it into `RESULTS.md` with provenance and prints the command that
makes a checked result a memory. Agents on his machine read `RESULTS.md` and the run folders.

## The files here

| file | written by | read by |
|---|---|---|
| `OWNER_MESSAGE.md` | **Yitzchak** | the sync, which pushes it into the control README |
| `BOARD.md`, `TASK_ROSTER.md`, `PROTOCOL.md`, `roles.json` | the sync, from the control README, fleet.json and roles.json | the hook, the mirror, every agent |
| `WAKE_PROMPT.md`, `BRAIN_FOR_TASKS.md` | the brain | the tasks (mirror), whoever enrolls a task |
| `RESULTS.md`, `inbox/` | the ingest script, from pasted report blocks | agents, the tasks (mirror) |
| `board_sync.py`, `publish_board.py`, `ingest_task_result.py`, `SYNC.log`, `PUBLISH.log` | the brain | operations |

Operations, paths and task names on his machine: `OPERATIONS.md` (private). The GPT's own installation report and
evidence: the control repository's `scheduled_tasks/status/INSTALLATION.json` and his Downloads of 2026-09-20.
Memory: `owner_scheduled_tasks_board_and_the_eighty_task_roster_2026_09_20`.
