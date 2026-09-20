# The scheduled tasks: eighty GPT tasks that wake into the brain, and the board you talk to them on

Owner order, 2026-09-20 18:37 (his clock), in his words: *"i want a read me about the scheduled tasks, and i want that
every gpt here wakes up connected to the full brain, also there should be 80 scheduled tasks running at any time, on 4
different gpt accounts that i have ... any gpt that has access to the scheduled tasks should always make sure that the
full amount in this account (20 of them) is running full time every hour, solving problems, improving the brain,
connecting the brain and so on. they should run on the highest computational max thinking that they can. also there
should be a part of the read me that i can change to talk to all the scheduled tasks and to the gpts that have access to
the scheduled tasks to read this read me whenever they run and make sure that what i am asking for is being implemented
... have a whole tasks thing in the brain that the schedules keep reading, that agents like you keep reading, and that i
can update that will allow me to communicate with the scheduled tasks more easily."*

This folder is that thing. Everything the tasks read lives here; a publisher mirrors the readable part to a public
repository every fifteen minutes, because a ChatGPT task runs in OpenAI's cloud and can only read what the web can reach.
The exact paths, commands and task names on the owner's machine are in `OPERATIONS.md`, which stays private.

## The files

| file | who writes it | who reads it |
|---|---|---|
| `OWNER_MESSAGES.md` | **Yitzchak** (nobody else edits his words) | every scheduled task at every run; every Claude and Codex agent on his machine through the `[owner-board]` hook line |
| `TASK_ROSTER.md` | the keepers (whoever holds an account's task list), agents on his machine | the tasks, to know their slot; the keepers, to keep the count full |
| `WAKE_PROMPT.md` | the brain | pasted into every scheduled task as its instructions; the task re-reads the published copy each run |
| `BRAIN_FOR_TASKS.md` | the brain | the tasks: what the brain is, what it is working on, how to report back |
| `RESULTS.md` | the ingest script, from `inbox/` | agents on his machine, and the tasks (so they build on what other tasks reported) |
| `inbox/` | Yitzchak or an agent, by pasting a task's report block | the ingest script |
| `publish_board.py` | the brain | the publish task, every 15 minutes, and anyone by hand |

Public mirror: **https://github.com/yspennstate/brain-tasks-board** (raw files at
`https://raw.githubusercontent.com/yspennstate/brain-tasks-board/main/<file>`). Only the six files named in the
publisher go there, and only after a private-label check and a secret scan pass; the mirror never carries paths on his
machine, account names, keys, market vocabulary or anything from the private memories.

## What a ChatGPT scheduled task is (read 2026-09-20)

From OpenAI's Help Center article "Scheduled tasks in ChatGPT" and the ChatGPT docs on automations:

- A scheduled task is a prompt ChatGPT runs on a schedule; each run starts a **new chat** and reports its results there,
  in the Scheduled view, with an unread indicator; a task can also be one-time or event-triggered (Gmail, Slack, GitHub
  pull-request activity).
- **A task cannot run more than once per hour.** Hourly is the fastest schedule, and it is what "full time every hour"
  means here.
- **Active-task limits per account depend on the plan: Free and Go 3, Plus 5, Business and Edu 10, Pro and Enterprise
  15.** Paused tasks still occupy a slot; free a slot by deleting. His order says 20 per account; the largest cap we
  could read is 15. The roster keeps 20 slots per account as ordered, and the keeper fills an account to its real cap
  and writes the cap it hit into the roster.
- The **model and the reasoning effort can be chosen explicitly** when the task is created or edited. His order: the
  highest reasoning the account offers, on the strongest model available to it.
- When it runs, a task can **browse the web**, use uploaded context and connected tools, run code, and combine with
  skills. Browsing is how it reads this board: the raw URLs above.
- OpenAI's own advice: test the prompt in a normal chat first; make the prompt durable (describe what to do on each run);
  give the narrowest access that lets the task succeed.

## The roster: 80 tasks, four accounts, twenty each

| account | slots | who keeps it full |
|---|---|---|
| account 1 | A01 .. A20 | the GPT or person with that account's task list |
| account 2 | B01 .. B20 | same |
| account 3 | C01 .. C20 | same |
| account 4 | D01 .. D20 | same |

The slot's letter and number is the task's name inside ChatGPT ("A07 - brain: open questions"), so a keeper can compare
the account's task list with the roster in one look. `TASK_ROSTER.md` holds, per slot: the area, the schedule (hourly),
the model and reasoning set, the status, and the last verification (who, when, what the account's real cap turned out
to be). Areas, in his words: **solving problems** (the open problems), **improving the brain**, **connecting the brain**
(getting the brain to more agents and places), plus the keeper's own count and audits of what other tasks reported.

## The keeper rule

*"any gpt that has access to the scheduled tasks should always make sure that the full amount in this account (20 of
them) is running full time every hour"*. So: whoever opens one of the four accounts - a ChatGPT session, a ChatGPT agent
run, a person - counts the account's active tasks against its twenty roster slots **every hour**, creates or resumes the
missing ones from `WAKE_PROMPT.md` with the slot's area, sets the schedule to hourly and the reasoning to the highest
offered, and writes the count and the cap into `TASK_ROSTER.md` (through the inbox if it cannot edit the brain). A task
that finds itself unable to run hourly, or a cap below twenty, says so in its report instead of silently doing less.

## The board: how Yitzchak talks to all of them from one place

Edit `OWNER_MESSAGES.md` in this folder. It has two parts: **STANDING ORDERS** (what every task must always do) and
**MESSAGES** (dated, newest first). Within fifteen minutes the publisher pushes it to the public mirror; every task
fetches it at the start of every run and acts on it; every agent on his machine gets the newest message once an hour
through the `[owner-board]` hook. His later words win over an earlier task, on the board as everywhere else. The
publisher can also be run by hand (see `OPERATIONS.md`).

## Waking connected to the brain

Two levels, because the brain itself is private:

1. **Every task, always:** the published set - the board, the roster, `BRAIN_FOR_TASKS.md` (the brain's areas, its
   current focus, its standing rules in sanitized form) and `RESULTS.md` (what other tasks found). That is what the
   wake prompt tells a task to read first.
2. **The full private brain:** ChatGPT's GitHub connector, once Yitzchak connects it in an account, lets a task read the
   private repository `yspennstate/ai-memories-and-functionality` directly; the wake prompt then names the files to
   read (the memory index, the brain views, this folder). That is his setup to do per account; until then the tasks
   have level 1.

The GPTs **on his machine** (Codex sessions) wake connected already: the Codex hooks hand them the brain wake, the
reflexes, the owner-prompts block and the checklist at every prompt (since 2026-09-20 18:0x they emit JSON, which is
the only form Codex injects).

## The way back: how a task's work reaches the brain

A scheduled task cannot write here. Its run ends with a report block (the format is in `WAKE_PROMPT.md`):

    TASK: A07  ACCOUNT: 1  RUN: 2026-09-21 03:00
    READ: <which pages loaded>
    RESULT: <what was found or done, with sources>
    NEXT: <what the next run should do>
    BOARD: <one line answering the current message, or "none">

Paste it (or ask any agent to) into `inbox/<slot>_<date>.md` and run the ingest script; it appends the block to
`RESULTS.md` with its provenance and prints the command that makes a checked result a memory. Agents on his machine read
`RESULTS.md` and file real results as memories in the shared voice. The ChatGPT GitHub connector, once connected, gives
the tasks a second way back: they can read what others wrote; they still cannot commit.

## Operations, in short

A windowless Windows task publishes this folder's six public files every fifteen minutes after a private-label check
and a secret scan; a hook hands every Claude and Codex session the board's standing orders and newest message once an
hour; the ingest script files task reports. Paths, commands, task names and logs: `OPERATIONS.md` (private).

Memory: `owner_scheduled_tasks_board_and_the_eighty_task_roster_2026_09_20`.
