# The board: what Yitzchak is telling the scheduled tasks and every agent

This is a rendering of the single source the tasks read: `scheduled_tasks/README.md` on the main branch of the
math-research-brain repository (control commit a76e482233f2). The owner edits it there, or in the brain's local copy
`OWNER_MESSAGE.md`, which the sync pushes within fifteen minutes. His later words win over an earlier task.

control: revision 2026-09-25.3, mode MIXED, fleet_enabled True, target 20 per account every 60 minutes, paused accounts [], paused slots {}, research queue 1 entries

## OWNER MESSAGE

OK, rewrite that file repairing all the parts to the need to be repaired, make sure to read all the reports carefully while you do this. Then put in the new paper with all the repairs, and tell all the schedules to audit the new paper. And make sure to specifically tell account for that it should also be auditing the paper.

Later, 25 Sep 12:29: There is a paper for the case where the fifth singular value is bigger than 1. It has been audited by the scheduled agents, and there is a new draft for it from a GPT agent. I want every single result in this paper verified with a Lean algorithm. Any AI working on open-problem math should pivot to proving this with Lean. Keep working on the Lean algorithm for that paper, nothing else.

## Where the rest is

- Roles, accounts and what is verified: `TASK_ROSTER.md` (from fleet.json and roles.json).
- How a task must behave every run and how repairs are serialized: `PROTOCOL.md` (copy) in the control repository.
- The prompt a task is given: `WAKE_PROMPT.md`. What the brain is: `BRAIN_FOR_TASKS.md`. What tasks reported: `RESULTS.md`.
- Public copies of these files: https://raw.githubusercontent.com/yspennstate/brain-tasks-board/main/<file>
