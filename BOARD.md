# The board: what Yitzchak is telling the scheduled tasks and every agent

This is a rendering of the single source the tasks read: `scheduled_tasks/README.md` on the main branch of the
math-research-brain repository (control commit 4861282421a5). The owner edits it there, or in the brain's local copy
`OWNER_MESSAGE.md`, which the sync pushes within fifteen minutes. His later words win over an earlier task.

control: revision 2026-09-26.1, mode MIXED, fleet_enabled True, target 20 per account every 60 minutes, paused accounts [], paused slots {}, research queue 1 entries

## OWNER MESSAGE

26 Sep 00:31: I made a voice note on how the brain should work. Everything the agents touch - files, folders, memories, readmes, rules, laws, hooks, tools, code, keywords, boxes, volumes, theorems and proofs - is a node; a node grows the more it is used; edges grow along the sequences things are used in; a loop of firing that once led to a mistake, a tool or a way of thinking flows into the agent automatically. The brain is a subconscious graph in the background feeding the context window. Give the scheduled tasks the voice note and have them audit that information, those paths and that methodology: every run reads work/shared/brain-audit-2026-09-25/FOCUS_2026-09-26_BRAIN_GRAPH.md in the control repository and gives it its own section of the report, and each slot reads the mathematics of subconscious-to-conscious flow in its own area. Reports only, no changes.

25 Sep 21:35: I want all the scheduled GPT tasks to start focusing on auditing the brain, and the papers we have been writing about the brain, and writing reports about how it is helping, what its strongest key parts are, what bugs it might have, and how to make it better. They should focus on these audits of the brain exclusively. They should not make any changes, just audit every hour, forever, and write papers on what they are finding, how to make the brain better and how to test the brain's strengths more. And when you give them the prompt, think of more things I might have missed for this research project (I want to publish something soon), and have them focus on those as well.

Earlier the same day (replaced by the message above): OK, rewrite that file repairing all the parts to the need to be repaired, make sure to read all the reports carefully while you do this. Then put in the new paper with all the repairs, and tell all the schedules to audit the new paper. And make sure to specifically tell account for that it should also be auditing the paper.

Later, 25 Sep 12:29: There is a paper for the case where the fifth singular value is bigger than 1. It has been audited by the scheduled agents, and there is a new draft for it from a GPT agent. I want every single result in this paper verified with a Lean algorithm. Any AI working on open-problem math should pivot to proving this with Lean. Keep working on the Lean algorithm for that paper, nothing else.

## Where the rest is

- Roles, accounts and what is verified: `TASK_ROSTER.md` (from fleet.json and roles.json).
- How a task must behave every run and how repairs are serialized: `PROTOCOL.md` (copy) in the control repository.
- The prompt a task is given: `WAKE_PROMPT.md`. What the brain is: `BRAIN_FOR_TASKS.md`. What tasks reported: `RESULTS.md`.
- Public copies of these files: https://raw.githubusercontent.com/yspennstate/brain-tasks-board/main/<file>
