# Task roster: four accounts, twenty roles each (from the control files, rendered 2026-09-20 19:04)

Order (2026-09-20 18:37): 80 scheduled tasks running at any time, twenty per account, full time every hour, on the
highest reasoning each account offers. Control: `fleet.json` desires 4 accounts x 20 tasks = 80; cadence every 60
minutes; controller slot B20. ChatGPT's own caps per account are 3 (Free, Go), 5 (Plus), 10 (Business, Edu) or 15 (Pro,
Enterprise) and a task runs at most once an hour: a keeper fills the account to its real cap and reports the cap.

## Accounts

| account | binding | observed enabled | focus |
|---|---|---|---|
| account01 | current_connection_verified | 20 | implementation |
| account02 | requires_owner_binding_in_that_account | not observed | independent_validation |
| account03 | requires_owner_binding_in_that_account | not observed | portability_and_reproduction |
| account04 | requires_owner_binding_in_that_account | not observed | adversarial_acceptance |

An account is enrolled from inside that account with the instruction in `ONBOARDING.md` (the control repository);
a label is not a login. Only account01 has been observed (20 enabled, hourly, 2026-09-20).

## The twenty roles (the same in every account; B20 keeps the account full and accepts the others' work)

| slot | role | what it does |
|---|---|---|
| B01 | Source transfer | Transfer complete source bytes through authorized connectors; verify Git blob hashes, resumable chunks and safe archive handling. |
| B02 | Package startup | Execute the real eager package initializer with its authentic dependency closure; never count namespace-only imports as full startup. |
| B03 | Offline packaging | Build reproducible source or wheel artifacts and dependency manifests; test installation in clean native processes without implicit paid ser |
| B04 | Portable launcher | Implement explicit sandbox paths and a real command-line bootstrap; retain errors and avoid owner-machine defaults. |
| B05 | Population transfer | Transfer the genuine approved corpus and reconcile row/file hashes and manifest counts; partial samples are not the full corpus. |
| B06 | Store restoration | Restore real records through production store APIs preserving IDs, schemas, evidence history and statuses; test atomic rejection. |
| B07 | Graph retrieval | Execute production prefilter, typed-graph retrieval and rendering; verify real edge traversal, warnings, revisions, guards and abstention. |
| B08 | Semantic retrieval | Run the real semantic encoder with compatible approved vectors; missing models remain blocked, never replaced with random vectors. |
| B09 | Guarded ingestion | Run the actual allowlist, provenance and ingestion gates on isolated fixtures and approved sources; never weaken a deny rule. |
| B10 | Evidence verification | Exercise evidence binding and status-transition authority; reject unsupported promotion, wrong digests, stale evidence and replay. |
| B11 | Mistake reflexes | Persist a scoped mathematical counterexample and demonstrate a later real warning/reflex; check unrelated negative controls. |
| B12 | Consolidation | Run actual consolidation/replay and revisions; proposals stay quarantined and cannot create truth authority or overwrite history. |
| B13 | Citation binding | Validate exact sources, locators and claim scope; distinguish structural hash matching from semantic support and human review. |
| B14 | Formal backend | Run a genuine formal checker through production wrappers when available; separate kernel checking, admitted proofs and prose fidelity. |
| B15 | Evaluation adapter | Connect actual retrieved memory to a scheduled solver workflow; distinguish current-agent use, mocked transports and isolated model evaluati |
| B16 | State export | Export and restore complete state safely, retaining identities, graph and evidence history; test corruption and schema mismatches. |
| B17 | Cross-run memory | Create and recover an actual checkpoint in distinct scheduled invocations; verify identical artifact hashes without reconstructing expected  |
| B18 | Task handoffs | Implement verified GitHub-backed artifact handoffs and conflict-safe checkpoints across tasks/accounts; never assume shared disks. |
| B19 | End-to-end integration | Assemble consistent authentic components, execute one complete lifecycle and provide reproducible manifests and evidence for acceptance. |
| B20 | Caretaker and acceptance | First audit this account inventory and repair authorized drift under the single-writer lease protocol, then independently execute acceptance |

Task name inside ChatGPT: `NN Bxx <role>` (the rendered specification's title, e.g. `02 B01 Source transfer`);
the prompt carries the marker `BRAIN-FLEET v1 account=accountNN slot=Bxx`, which is how a keeper tells managed
tasks from unrelated ones. Render every account's twenty specifications with
`python scheduled_tasks/tools/control.py render --root scheduled_tasks --repository yspennstate/math-research-brain --account accountNN`
from the control repository's root.
