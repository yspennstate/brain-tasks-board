# Implement the complete brain in this ChatGPT account

**Owner handoff for an interactive implementation chat and its scheduled workers.**

Prepared: 2026-09-20. This is a deployment guide and acceptance contract, not a report that the complete brain is already operating. Read the current owner controls before using it. The owner’s newer instructions and platform restrictions take precedence.

## 0. Give the receiving GPT an explicit account binding

Use the account-specific edition of this document, or put exactly one of these sentences above this document:

> This is my separate account02. Implement this guide in this account, with account02 as the logical fleet profile.

> This is my separate account03. Implement this guide in this account, with account03 as the logical fleet profile.

> This is my separate account04. Implement this guide in this account, with account04 as the logical fleet profile.

Do not paste all three as an account assignment. These are logical labels, not login identities. Three chats in the same signed-in account are not three separately authorized scheduler accounts. Do not reuse account01, which is already assigned. When the owner supplies the account binding in a chat, perform the implementation using actual tools; do not merely summarize this README or ask for the same binding again.

The requested allocation is twenty hourly tasks in each of four separately authorized accounts. Eighty is the owner’s desired registration total, not an assertion of eighty active executions, eighty independent model contexts, or an entitlement to exceed platform limits. Preserve the requested target and separately report what is permitted and observed.

## 1. Understand what “the full brain” includes

There are three distinct resources. Do not silently collapse them into one.

| Resource | Exact repository | Function |
|---|---|---|
| Mathematical runtime and owner control | `yspennstate/math-research-brain` | The `math_brain` package, mathematical claims, evidence, typed graph, provenance, verification, retrieval, and `scheduled_tasks/` controls. |
| Broader memory and firing engine | `yspennstate/ai-memories-and-functionality` | File-based memories and the recall, spreading activation, reflex, attachment, consolidation and runtime-hook mechanisms described below. Only explicitly permitted technical code and mathematical memory belong in this integration. |
| Published instruction mirror | `yspennstate/brain-tasks-board` | Public owner-board and task summaries. This is not a copy of the complete private corpus or an executable substitute for either runtime. |

The user’s requested result is more than a searchable folder: a request should activate relevant records, propagate through appropriate relationships, surface eligible warnings and useful associations, supply the selected context to the working agent, and preserve authorized learning for later runs. Importing the mathematical package alone does not demonstrate the broader memory system’s node-firing path. [R1–R5]

“Firing” here means a software activation or trigger event. It does not change ChatGPT’s model weights, give access to hidden model neurons, establish biological neural activity, or establish consciousness. The cognitive architecture explicitly describes changing what an agent reads and writes, not its weights. Its historical descriptions of local-machine success are not evidence of execution in this account. [R6]

**Full network availability does not mean all nodes fire on every request.** Selective activation, propagation limits, salience thresholds, negative evidence, deduplication, supersession, context budgets and justified silence are intentional behavior. Loading all permitted records and preserving the graph is the coverage goal; indiscriminately injecting the entire corpus would be a different system. [R3–R5]

## 2. Read the owner’s current instructions first

Resolve the current `main` commit in the mathematical control repository through this account’s authorized GitHub connector. Read these files at that same commit:

```text
AGENTS.md
scheduled_tasks/README.md
scheduled_tasks/fleet.json
scheduled_tasks/roles.json
scheduled_tasks/PROTOCOL.md
scheduled_tasks/ONBOARDING.md
```

Read both the JSON **OWNER CONTROL** and the natural-language **OWNER MESSAGE**, not just one. Record the control commit, directive revision, SHA-256 of the exact README bytes and SHA-256 of the message text extracted using the control helper’s convention. Do not silently normalize newlines when claiming an exact-byte hash.

The control snapshot read for this guide was `517efcdda859abeac0ce3e08196b241e1b72e4b6`, revision `2026-09-20.1`, mode `BRAIN_FIRST`, with no account or slot pauses and an empty research queue. Before delivery, a fresh README read at commit `21979fc03c79c4bcead152bef2a279a4b3979517` showed owner revision `2026-09-20.2`. Its added instruction requires every worker to report its account, slot/task number and current work so caretakers can count actual coverage. This guide requires those fields. Both observations are dated, not permission to skip the next fresh read. The mathematical software baseline is separately pinned in `fleet.json`; changing a live instruction does not require secretly mixing source revisions. [R1–R2]

If controls are unavailable, incomplete or invalid, do not make external mutations under cached permissions. Read the public mirror as orientation and report `PUBLIC_MIRROR_ONLY` when appropriate. The supplied guide allows mirror-based role work; the private protocol is stricter about working without valid control. Accordingly, do not infer new private-data or scheduler-write authority from a mirror. Limit fallback activity to read-only, non-sensitive orientation or work already explicitly authorized in the current conversation; surface the conflict rather than hiding it. [U1, R1–R2]

Useful mirror files are `BOARD.md`, `TASK_ROSTER.md`, `PROTOCOL.md`, `roles.json`, `WAKE_PROMPT.md`, `BRAIN_FOR_TASKS.md` and `RESULTS.md`. Verify which actually exist. A published claim of fifteen-minute synchronization is not a freshness guarantee: compare source commit/revision and timestamp when supplied. Never invent a mirror `fleet.json` if that file is not published. [U1, R7]

## 3. Establish this account’s actual capabilities

The interactive implementation chat owns this initial inventory. Call the actual available tools rather than infer capabilities from instructions or another account’s report.

Check authenticated repository reads, a native Python/container execution tool, temporary-file read/write, installed package versions needed for the implementation, and access to the scheduler inventory. A tiny actual calculation and file round-trip establishes native execution only. A GitHub read establishes repository access only. Record them separately.

Do not search for credentials, inspect environment dumps, crawl the owner’s machine, install an external runner, or start paid services. Use only an isolated temporary workspace and authorized connector routes. Dependencies must be already available or obtainable through a permitted, provenance-checked route without new spending. Lack of a particular transport is a specific blocker, not proof that every scheduled environment lacks execution.

An interactive session’s capabilities are not automatically a scheduled invocation’s capabilities. Require the first scheduled run in this account to reproduce native execution, authentic source loading and a real query. Likewise, account01’s success does not establish account02’s success.

## 4. Current platform facts and the supplied guide’s assumptions

**External verification, separate from the uploaded guide:** OpenAI’s Tasks page checked on 2026-09-20 lists active limits of 3 for Free/Go, 5 for Plus, 10 for Business/Edu, and 15 for Pro/Enterprise; other eligible arrangements may vary. Eligible paid plans support hourly recurrence. Supported connected apps include GitHub, subject to permissions. Scheduled tasks do not support custom GPTs, and a task created in a Project cannot access that Project’s uploaded files. External writes can require approval. [W1]

The current account’s actual scheduler inventory showed twenty enabled hourly managed registrations during preparation. Preserve that observation without generalizing it into a universal cap. Do not assume the other accounts allow twenty. The supplied guide’s statement that paused tasks keep an active slot is not supported by the checked help page, which suggests pausing an active task to make room. Native code availability, a fresh isolated model context on every run, and a universal per-task effort selector were not established by that page. [U1 §7, W1]

The scheduler tool exposed in the preparation session has title, prompt, schedule and enable controls, but no model/effort selector. Set the highest supported options only where a real selector is available. Record requested and observed settings separately; unknown is `UNVERIFIED`. A README cannot allocate CPUs or guarantee uninterrupted hourly computation.

## 5. Enroll or repair the scheduler without duplicating workers

Obtain a fresh, complete inventory in the receiving account. Count separately: total enabled tasks; managed tasks with the exact account/slot marker; hourly-valid managed tasks; missing B01–B20 slots; intentional holds; duplicate markers; observed permission/capacity limitations; and evidence of recent runs. Do not commit actual scheduler IDs or account identities.

Use the existing source-verified helper to render specifications, substituting the one bound account:

```sh
python scheduled_tasks/tools/control.py validate --root scheduled_tasks
python scheduled_tasks/tools/control.py render --root scheduled_tasks --repository yspennstate/math-research-brain --account account02
python -m unittest discover -s scheduled_tasks/tests -v
```

The renderer produces specifications; it does not create tasks. Inspect actual output and API schemas, then invoke the receiving account’s authorized scheduler tools. Never send placeholder account names or role identifiers to the scheduler. Enroll B20 first when creating a new fleet so maintenance is not crowded out if capacity is lower than the target; then enroll the other permitted slots. This ordering is deployment guidance, not an additional task.

Before any repair or enrollment, follow the live protocol’s exclusive create-only lease:

```text
scheduled_tasks/leases/<bound-account>/<UTC-hour>.json
```

Include a unique nonsecret run identifier and current control revision. If another writer owns the lease, do not overwrite it. If the connector cannot implement reliable create-only semantics, do not claim a lock exists. Report the blocker and avoid racing.

Update identified managed tasks instead of duplicating them. Preserve valid hourly offsets and unrelated tasks. A disabled or missing task can represent an intentional stop or deletion; inspect the current owner instructions and available evidence before proposing revival or replacement. Stop creation/resume on the first capacity or permission rejection. Do not evade the limit with hidden workers, unbounded loops, or unauthorized accounts. A lower actual total must remain visible, with missing roles explicitly listed. Do not silently collapse twenty roles into fewer tasks; present any such alternative for owner approval.

B20 is the caretaker and independent acceptance worker. Other scheduled workers inspect and report drift; they do not independently race to repair it. An interactive chat directly authorized by the owner may act as caretaker under the same protocol. If all tasks are paused, later interactive owner action is needed; paused workers cannot wake themselves.

## 6. Use the twenty roles as a dependency-driven team

Read `roles.json` live; this table explains how its current roles support the complete integration. The firing-related checks below refine testing and do not overwrite protected role definitions.

| Slot | Main implementation deliverable | Specific connection to the full network |
|---|---|---|
| B01 | Verified resumable source transfer | Transfer genuine activation/reflex code as well as mathematical modules, within the permitted source scope. |
| B02 | Authentic package initialization | Load the real mathematical initializer and the approved cognitive-engine import closure separately. |
| B03 | Reusable package and dependencies | Produce inspectable, reproducible artifacts instead of repeating huge text transfers in every worker. |
| B04 | Portable launcher and adapters | Connect each scheduled invocation and interactive request to actual runtime entry points. |
| B05 | Authentic approved population transfer | Reconcile complete eligible nodes, edges and required sidecar coverage, not just file counts. |
| B06 | Production-store restoration | Preserve IDs, provenance, verification history and typed relationships. |
| B07 | Graph retrieval | Validate actual propagation paths, directionality, negative evidence and rendered results. |
| B08 | Semantic integration | Distinguish mathematical encoder retrieval from the cognitive sidecar/seed-centroid method. |
| B09 | Guarded ingestion | Keep the mathematical boundary and ensure no fixture contaminates production memory. |
| B10 | Evidence verification | Prevent discovery, activation or a copied receipt from becoming unsupported truth authority. |
| B11 | Mistakes and reflexes | Reproduce real trigger behavior with positive and unrelated negative controls. |
| B12 | Consolidation and revisions | Preserve quarantined proposals, supersession and append-only learning history. |
| B13 | Citations and attachments | Validate supporting sources and complete parent-node document reads. |
| B14 | Formal checking | Execute the genuine checker when available, without treating admissions or prose mismatch as proof. |
| B15 | Context/solver integration | Deliver actual fired/retrieved context before reasoning; keep model isolation and evaluation honest. |
| B16 | Export/restore | Preserve graph, indexes and authorized persistent firing state through explicit schemas. |
| B17 | Cross-run memory | Restore an actual prior-run checkpoint, including relevant deduplication/learning state where intended. |
| B18 | Cross-worker handoffs | Make a new worker retrieve, verify and consume artifacts through the repository. |
| B19 | End-to-end assembly | Execute the combined pipeline, not merely collect other workers’ summaries. |
| B20 | Caretaking and acceptance | Check coverage, then independently challenge the assembled runtime and firing behavior. |

The existing focus profiles are account02 independent validation, account03 portability/reproduction, and account04 adversarial acceptance. Preserve those unless the owner changes them. All may implement a missing component when useful, but coordinate by concrete source/module/artifact ownership so sixty workers do not independently retranscribe the same file.

Prioritize removal of the shared bottleneck. A complete verified import closure and a reusable approved corpus handoff are more valuable than twenty repetitions of the same partial smoke test. Preserve substantive negative findings, but do not create receipt-only work and call that implementation progress.

## 7. Transfer complete source; keep control and code versions separate

For each system, freeze an explicit source revision and record every needed path, byte length and Git blob SHA. Read complete source bytes through supported connector operations. Exact connector text copied into the native workspace is an authentic transfer when the whole-file hash matches. Metadata-only responses and truncated previews are not complete files.

The Git blob identity is:

```python
import hashlib

def git_blob_sha(raw: bytes) -> str:
    header = b"blob " + str(len(raw)).encode("ascii") + b"\0"
    return hashlib.sha1(header + raw).hexdigest()
```

For chunked transfer record offsets, expected length, encoding and per-chunk hashes; reject overlap, gaps, truncation and reordering. Decode base64 only where the connector actually returns that representation. Persist resumable progress using the authorized artifact mechanism. Validate the final entire file, not just each chunk.

Prefer an existing authentic source/package handoff after checking its immutable provenance, member hashes and source revision. Inspect archive names before extraction; reject traversal, links escaping the workspace, duplicate/conflicting members, oversized expansion and executable serialized payloads. A downloaded filename or aggregate ZIP hash alone does not establish the identity of every module inside.

The mathematical baseline currently named in fleet configuration is `39cfb28999ea514a8a16be7c7ae2123b5419e96a`. The source manifest historically contains 33 direct package-tree entries, including two backup files; that is not 33 required importable modules. Keep an archive-completeness metric separate from the actual runtime import closure. Do not block a demonstrated normal import solely because an inert backup file was omitted, and do not call the archive complete when it was omitted.

Run a genuine normal import in a clean native process. Do not remove the original initializer, fake its modules or suppress import errors to report complete startup. A proposed modularization or portability fix belongs in a separately labeled patch with baseline comparison and regressions. Record exactly which revision and patch set executed.

## 8. Restore the complete eligible mathematical graph

Fetch the actual export manifest at the pinned data revision. The goal is byte- and record-complete transfer of the approved export, followed by restoration through the production store/deserializer interfaces. Preserve immutable identities, hypotheses, statuses, citations, evidence scope, revisions and graph endpoints.

Maintain four separate measurements: expected/transferred bytes; expected/parsed records by table; endpoint and provenance coverage; and successfully restored/queryable records. An empty manifest table can be valid, but transferring seven empty tables is not seven substantial pieces of the populated brain. Do not describe “eight of fifteen tables” as a percentage of usable mathematical content.

Verify complete file byte counts, Git object identities, any manifest SHA-256 values and exact JSONL row counts. Partial extracted views require their own hashes and scope label. If metadata was sanitized, the resulting bytes are not the original row bytes: retain the original source identity separately and do not claim the old digest authenticates the modified view.

Use an explicit approved temporary database path. Do not open an assumed owner-local default, silently invent an empty production store, or rebuild missing evidence authorities from narrative reports. Reject or quarantine malformed rows, duplicate identities, missing mandatory references and incompatible schemas. Test atomic interruption/retry and read-only reopening. Keep engineering fixtures separate from authentic memory.

Whole eligible network coverage and per-query output are different. A selective query can return a few nodes even when the entire approved graph is present. Coverage must come from validated ingestion/manifests, not the apparent size of the returned context.

## 9. Port the actual cognitive firing engine, not its description

The broader memory source inspected for this handoff was revision `3fe378e6b15ed02695cc3e008f2f46a175015d26`. The following are verified navigation targets, not a claim that they executed here:

```text
12_cognitive_architecture/dreaming/brain.py
12_cognitive_architecture/dreaming/spread_recall.py
12_cognitive_architecture/dreaming/BRAIN_NODE_DOCUMENTS.md
12_cognitive_architecture/COGNITIVE_ARCHITECTURE.md
```

Read actual imports and data-loading paths recursively, obtaining only the explicit technical dependency closure and approved mathematical data. `brain.py` imports the spreading engine, node-document handling and supersession support. The spreading source names keyword and embedding artifact helpers. Its inputs include the association edges, salience scores, mistake weights, topic/keyword maps, supersession information, optional embedding artifact and relevant session firing state. Preserve schema and provenance rather than generating substitute tables and calling them the original network. [R4–R6]

The documented read operations include `brain.py recall`, `brain.py node`, `brain.py neighbors`, `brain.py verify-attachments` and `brain.py status`. Inspect the actual CLI before calling them. Its write operations, including remembering or attaching material, have additional validation/coordination requirements; a successful local fixture does not authorize a production write. [R4–R5]

Use explicit safe path configuration. The source includes owner-machine defaults and a documented `BRAIN_MEM_DIR` test seam, but that seam does not prove every other artifact/state path is redirected. Audit each path actually opened. Port missing path injection in a separate adapter/patch without changing the mathematical or firing algorithm. Do not execute local-machine hooks, management scripts, or broad health checks blindly in the sandbox.

The broader repository also contains unrelated private material. Access to it is not a per-file mathematical ingestion grant. Do not ingest the whole general memory index or all personal/trading/company notes merely to claim “full brain.” Inventory the necessary code and obtain an approved mathematical/engineering memory export with its own manifest. State the exact excluded scope; never quietly claim the whole mixed-domain corpus was imported.

## 10. Keep the two activation algorithms distinct

### Mathematical typed-graph propagation

The mathematical engine builds relevance seeds from lexical, symbol, formula and, when genuinely available, semantic channels. Its graph step uses typed edges and bounded paths. Propagated amounts include the incoming score, decay, absolute signed weight and edge-type multiplier. Warning paths are kept in a separate warning channel. Proof mode and discovery mode treat relationships differently. [R3]

Its graph traces identify source nodes, edge identities, edge kinds, polarity and node paths. The engine also awards seed-retention score with a one-node path, even without traversing an edge. Therefore a positive `GRAPH` score is insufficient evidence of graph propagation. Require a real multi-node path and an existing corresponding edge.

### Cognitive spreading and firing

The broader `spread_recall.py` describes prompt- or memory-read seeding, two-hop spreading over association links with fan-out normalization, and selective surfacing of non-obvious nodes. The inspected source contains salience/signal floors, margin thresholds, mistake-related boosts, redundancy checks and per-session deduplication. Its state and sidecars must be restored consistently for faithful behavior. [R4]

The broader recall command’s semantic path is described as using a precomputed embedding sidecar with seed-centroid similarity, without new encoder inference in that path. Do not confuse this with the mathematical package’s optional semantic candidate channel or require the wrong model interface. Test each implementation against its own actual code and artifact contracts.

Neither mechanism promises that every graph-reachable node should appear in the answer. A correct firing decision can be “no eligible node to surface.” Distinguish that from an exception silently disabling an optional component or a missing artifact being mistaken for an empty corpus.

## 11. Preserve strong-node deployment and attachment integrity

The inspected `brain.py` contains an additional strong-node runtime mechanism with content-addressed runtime pins and an enabled-marker check. The associated watch-report path explicitly distinguishes observe-only scanning from firing on memory access. Do not infer active deployment from the presence of a file, documentation, a watch report or a historical generation string. [R4]

Require the genuine compatible runtime generation, complete expected file set, valid hashes and whatever production activation/review authority the implementation requires. Missing human approval or an unactivated deployment remains `BLOCKED` or `OBSERVE_ONLY`. Test-only enabled markers and synthetic keys may exercise isolated tests, but cannot be called production enablement. Never change a pin or create an enabled marker merely to make a readiness matrix green.

For node documents, preserve the parent plus its immutable attachment manifest and actual UTF-8 document bytes. The documented node reader supports numbered parts for complete retrieval; consume every required part before claiming a complete read. Distinguish on-demand searchable documents from bounded automatic context and explicitly wake-marked material. Missing/corrupt existing attachments must not silently become “this node has no attachments.” [R5]

Full integration must preserve these budgets and integrity errors. It must not bypass them by dumping all documents into an enormous prompt. Test output completeness, rejection of altered attachments, and truthful degraded-state reporting.

## 12. Make node-firing acceptance an explicit deliverable

The companion `node_firing_acceptance.json` contains these proposed tests. They are requirements for the receiving implementer, all initially `NOT_TESTED`, not claims of execution or replacements for the live fleet’s existing gates.

| Test | Required observation |
|---|---|
| F01 — Genuine seed selection | Actual production input produces identified seeds and scores with source/configuration hashes. |
| F02 — Real edge propagation | A non-seed result is connected by an actual recorded edge/path; seed-retention alone cannot pass. |
| F03 — Bounded multi-hop behavior | Controlled chain exercises supported path depth; removing a necessary edge changes the actual output. |
| F04 — Correct typed direction | Proof-dependency traversal does not turn arbitrary similarity or reversed relationships into proof support. |
| F05 — Negative evidence | A counterexample/refutation relation surfaces a warning, not positive evidence of truth. |
| F06 — Engine-specific weighting | Decay, fan-out rules and seed aggregation match the particular engine, not a blended substitute. |
| F07 — Cycles and malformed edges | No runaway traversal; missing references and malformed data have documented safe outcomes. |
| F08 — Salience and margin gates | Suitable controlled cases pass or fail the real surfacing thresholds; no forced firing by lowering production thresholds. |
| F09 — Non-obviousness/redundancy | Cognitive surfacing distinguishes associative results from already-obvious lexical hits. |
| F10 — Deduplication and state | Repeated requests and distinct session/run identities exercise the intended suppression and reset/persistence rules. |
| F11 — Mistake/reflex path | A stored scoped failure triggers the relevant warning; an unrelated input is a negative control. |
| F12 — Real semantic channel | Compatible authentic vectors/encoder or documented sidecar method execute; fallback-only operation is clearly marked. |
| F13 — Supersession | Current corrections replace eligible historical endpoints as implemented, without deleting source history. |
| F14 — Node attachments | Parent plus required multipart documents are read fully and verified; corruption raises a visible integrity error. |
| F15 — Strong-node gate | Observe-only, disabled, invalid generation and genuinely authorized active modes are distinguished. |
| F16 — Actual context delivery | Fired/retrieved content is supplied to the working agent before the relevant reasoning step, with no claimed hidden neuron access. |
| F17 — Cross-run restoration | A later scheduled invocation loads the same real checkpoint and relevant persistent firing/learning state by hash. |
| F18 — Cross-account handoff | Another enrolled account reads and consumes the exact permitted artifact using its own authorized connection. |
| F19 — Complete eligible graph | Manifest-complete permitted nodes/edges/sidecars are loaded; deliberate samples are identified separately. |
| F20 — Legitimate silence versus failure | A no-fire decision with evaluated gates is distinguishable from missing data, disabled components or exceptions. |

Use small controlled fixtures to establish precise expectations, then repeat representative cases on the real approved saved graph. Fixtures are engineering tests, not proof that the original full corpus has been restored. Freeze data/configuration when comparing runs. Do not equate more frequent firing with improved mathematical usefulness; false positives and distraction are separate performance questions.

## 13. Wire the runtime into both scheduled and interactive work

For each scheduled invocation, the desired implemented sequence is:

```text
read current owner controls
→ validate runtime/corpus/checkpoint identities
→ initialize genuine mathematical and approved cognitive components
→ run recall/activation/reflex evaluation on the allowed task input
→ render eligible context and integrity/availability warnings
→ perform the mathematical or engineering work
→ validate proposed memory/evidence changes
→ write the authorized checkpoint and execution receipt
```

This sequence is an orchestration design, not the name of an already-existing API. The adapter should call inspected production entry points with their real signatures. Keep an explicit capability report and a test showing context actually reached the solver. A fabricated memory packet or a prose description of a call is not execution.

For an interactive chat, invoke the same verified runtime before relevant brain-dependent work and after material new information when useful. A repository rule cannot intercept every user message at the platform layer. If the available environment has no genuine pre-prompt hook, label the implementation an explicit per-request orchestration step rather than claiming hook installation. Local-machine Claude/Codex hooks described in the broader repository are not ChatGPT hooks. [R4, R6]

For ordinary chats, account Custom Instructions can carry a brain-first preference; put the same preference into the relevant Project instructions because those override the global instructions. Existing custom GPTs have their own instructions and do not inherit account custom instructions. These are guidance/configuration routes, not an installed runtime or guaranteed tool invocation. [W2–W4]

A reusable plugin/app connection may eventually provide a cleaner callable runtime, but no such Brain plugin is established by this handoff. Discover actual available tools and test them. A remote service requires separate owner authorization and a disclosed architecture; it cannot silently substitute for the current goal of native scheduled-environment execution.

## 14. Preserve learned state across real invocations

Prefer the authorized private GitHub artifact folders over assuming an earlier sandbox survives. Use immutable run folders, per-artifact hashes, logical account/slot labels and source/data revision metadata. Separate raw unreviewed source data from sanitized engineering artifacts allowed to be committed.

The cross-run test has two real stages. A creation invocation stores a harmless randomly parameterized mathematical fixture through the actual store, queries it and exports its state. A later scheduled invocation retrieves that exact committed checkpoint, verifies its bytes, restores through the real interfaces and queries the stored record. Preserve origin and consumer run identifiers and evidence of both executions.

Do not regenerate the fixture from its expected answer or embed the complete record into the next prompt as a fake persistence mechanism. Two subprocesses in a single invocation prove local restart only. Reading the same unchanging source files again proves source availability, not learned-state recovery.

For cognitive firing state, identify which values should be shared across sessions and which should remain per-session. Do not globally suppress a warning for every account because one session already received it. Persist schema-versioned permitted state through explicit interfaces; test concurrency, replay and idempotency. Authenticated GitHub transport is not a shared live Python process or instantaneous synchronization.

## 15. Give the other workers usable artifacts, not only reports

A handoff should identify its producing account/slot/run, original source revisions, approved patch set, file sizes and hashes, required dependencies, compatible data generation, exact command to run, tested behavior and unresolved prerequisites. Include actual scripts/configuration and admissible checkpoints, not just a sentence that they exist.

Write to the current owner-authorized private operational locations:

```text
scheduled_tasks/runs/<account>/<slot>/<unique-run>/
scheduled_tasks/work/<account>/<slot>/
scheduled_tasks/status/<account>/
```

Use the exact live protocol for shared leases and status paths. Do not overwrite another account’s artifact. For an immutable new file use a true create-only operation; for a permitted update use the current content identity and retry only after reconciling conflicts. Never force-push a tree based on an old main. Read back successful delivery at the returned commit.

Keep one useful receipt with the substantive artifact instead of repeatedly generating receipt-of-receipt commits. A self-check remains a self-check. Account02 can reproduce implementation artifacts, account03 can exercise portability and restoration, and account04 can challenge failing/negative cases; a peer reading the report is not an independent rerun.

Before each write inspect the precise changed-file allowlist for private data, credentials, account identities, scheduler IDs, machine paths and unreviewed excerpts. Run applicable repository checks; if a full suite is unavailable, state the limited fallback checks actually run. A privacy scan is not a grant to publish a private mathematical corpus. Do not change repository visibility or publish the cognitive corpus to the public mirror.

## 16. Use explicit runtime status, not one overloaded “connected” flag

Report these proposed supplemental states alongside the existing fleet component matrix:

| State | What must be observed |
|---|---|
| `SOURCE_ACCESS` | Authorized source/control retrieval worked. |
| `NATIVE_EXECUTION` | Actual code execution worked in this invocation. |
| `MATH_QUERY_EXECUTED` | Genuine package/store/retrieval call executed against the declared data scope. |
| `MATH_FULL_ACCEPTANCE` | The live `fleet.json` full-required set has current, independently checked evidence. |
| `COGNITIVE_RECALL_EXECUTED` | Actual broader recall code and the declared approved memory inputs executed. |
| `NODE_FIRING_VALIDATED` | Actual activation, gating, reflex and state tests passed for the declared engine/configuration/data. |
| `COMPLETE_BRAIN_INTEGRATION` | Both required runtime scopes, complete eligible network, context delivery and required persistence/backends passed. |

These are additional reporting names, not claims that the production API already emits them. Do not overwrite the live fleet schema or protected controls just to add a convenient label. Store supplemental evidence in your own receipt and propose any schema extension for owner review.

The uploaded guide uses initialization + restoration + query as a concise connection criterion. The current fleet definition is stricter and names semantics, formal backend, isolated model evaluation and cross-scheduled-run restoration. This handoff further separates the broader firing engine. A narrow query success is useful and should be used honestly, but must not erase any unfinished required scope. [U1 §6, R2]

An observe-only strong-node module, missing backend, an unexecuted external model, or a partial corpus remains visible. Distinguish implementation defects from unavailable external prerequisites. Do not wait to deliver working components until every optional feature is available; provide the usable partial runtime with precise capability flags while continuing toward the requested full scope.

## 17. Receipt template

Write a concise readable report plus a machine-readable record such as this. The following is a template, not a completed execution receipt:

```json
{
  "schema_version": 1,
  "account": "BOUND_ACCOUNT",
  "slot": "B19",
  "run_id": "ACTUAL_UNIQUE_RUN",
  "execution_context": "interactive_or_scheduled",
  "control": {
    "commit": "ACTUAL_CONTROL_COMMIT",
    "revision": "ACTUAL_REVISION",
    "readme_sha256": "ACTUAL_DIGEST",
    "owner_message_sha256": "ACTUAL_DIGEST"
  },
  "owner_requests": [],
  "code_and_data_manifests": [],
  "model_requested": "highest eligible available",
  "reasoning_requested": "maximum supported",
  "model_observed": "UNVERIFIED",
  "reasoning_observed": "UNVERIFIED",
  "components": {},
  "node_firing_tests": [],
  "artifact_refs": [],
  "full_brain_connected": false,
  "blockers": [],
  "next_unmet_stage": "TO_BE_FILLED_FROM_REAL_RESULTS"
}
```

Each component needs `PASS`, `PARTIAL`, `BLOCKED`, `FAILED` or `NOT_TESTED`, its exact scope, the invocation in which it was observed, and actual evidence references. A nonempty string called “evidence” is not authentication: inspect the referenced bytes and command outputs. A directive acknowledgment should say `implemented`, `in_progress`, `blocked` or `not_applicable`, with a reason.

Use the uploaded guide’s chat report shape so the owner can follow progress:

```text
TASK: Bxx  ACCOUNT: accountNN  RUN: actual UTC timestamp
CONTROL: actual commit, revision and hashes, or explicit degraded status
READ: actual files retrieved
RESULT: newly executed behavior, metrics, code/data scope, failures
FIRING: seeds/paths/gates/reflexes actually tested; or exact blocker
NEXT: one concrete unmet implementation stage
BOARD: response to each current owner request
DELIVERY: actual committed artifact references, or precise save failure
```

Preserve useful failures and measured before/after movement. Do not call source reading implementation, a checker count mathematical progress, or a scheduled registration a currently executing process.

## 18. Ready-to-use scheduled prompt supplement

Generate the live prompt for the actual role/account first. Append this supplement to make the fuller firing requirement explicit, preserving the owner-control and safety instructions. Replace the two binding placeholders before enrollment.

> BRAIN-FLEET v1 account=BOUND_ACCOUNT slot=BOUND_SLOT
>
> Read the latest authenticated owner controls and this account’s live role. The objective is the complete permitted brain environment, not only the mathematical package or README. When the role touches retrieval, reflexes, context delivery or persistence, distinguish the mathematical typed graph from the broader cognitive recall/spreading engine. Recover their actual source and required approved data/sidecars, preserve strong-node activation/review gates, and test real propagation, selective surfacing, warnings, deduplication, attachments and state restoration. Reading a memory description is not running its firing mechanism. Follow the full-brain handoff’s acceptance checklist as supplementary scope, not permission to edit protected controls or ingest mixed private archives. Execute a useful next stage now, save sanitized code/checkpoints and a precise receipt, and coordinate through existing roles. Never create a twenty-first role, evade capacity, override an owner stop, fake a backend or report more connection than the evidence supports.

Do not duplicate the ownership marker twice in one task prompt: replace its existing marker or append only the paragraph after the marker. The existing planner rejects ambiguous multiple markers. This guide’s template is for final prompt construction, not blind concatenation.

## 19. Owner controls and instructions for ordinary chats

For a message to all enrolled workers, edit the live OWNER MESSAGE and commit. Keep JSON valid and increase its revision when changing structured controls. The next successful fresh read should record the new text hashes and an acknowledgment. A task already in progress is not synchronously interrupted by a repository edit. The known pause/stop rules remain binding.

A proposed owner message to make the fuller scope explicit is:

> Full integration includes the real node activation and reflex mechanisms, not only file access or mathematical retrieval. Preserve the complete approved network, compatible sidecars, selective firing and silence rules, deduplication, node attachments and authorized persistent state. Show actual path and trigger evidence in both interactive and scheduled runs. Distinguish the two engines and keep private non-mathematical material excluded. Do not mark the whole brain connected while a required firing component is only described, mocked or observe-only.

This is a suggested message for the owner to adopt, not an assertion that protected controls were edited during preparation.

A compact account/Project instruction the owner can install is:

> For my mathematical research and brain-development chats, read the latest owner controls in my authorized brain repository before brain-dependent work. Attempt the genuine runtime and approved memory retrieval, including available graph activation and reflex mechanisms. Distinguish source access, working queries, validated firing and full integration. Use actual tools and cite records; do not pretend a README installs a runtime or exposes model neurons. Preserve the math-only boundary, permission limits and all later stops. With scheduler access inspect only this account’s enrolled fleet and coordinate authorized repair through B20. Keep my other chats and private non-mathematical material out of the brain.

This is not a tool for editing account settings from code. State whether the setting was actually changed or merely supplied as text. Do not assume a custom GPT or another signed-in account inherits it. [W2–W4]

## 20. The receiving implementation chat’s first session must deliver work

After reading fresh controls and identifying the bound account, do the capability/inventory checks, enroll or repair the permitted hourly tasks under the protocol, and execute one meaningful runtime step in the current chat. Recover the best existing handoff rather than beginning source transcription from zero. Record what the local environment can actually import and query, what is missing, and which worker owns that dependency.

Produce a concrete source/data acquisition map for BOTH engines and a package/launcher or executed component test. Route firing tests to B07/B08/B11/B13/B15/B17/B19/B20 without adding roles. Publish a sanitized installation receipt and usable engineering artifacts in the receiving account’s authorized folders. Report actual registrations separately from completed tests. Do not promise guaranteed completion later or an uninterrupted computation duration.

For continuing work, a worker with three unchanged results should change the authorized approach, seek a reusable artifact from another worker, or work on a different unblocked dependency. Do not endlessly print the same missing-module error. Never treat a difficult mathematical problem as solved merely to move the queue, and do not silently revive a research assignment the owner replaced with brain integration.

### Completion standard

A successful deployment is a demonstrated callable runtime with complete eligible data coverage, genuine graph/cognitive firing behavior, useful context delivery, safeguarded learning and verified restoration across actual invocations, with the live required backends and account-specific tests accounted for. It is not twenty configured prompts, an imported initializer alone, a bundle of empty tables, or eighty desired specifications.

## 21. Evidence basis and source map

This guide preserves the supplied document’s account binding, control-read, caretaker, lease, handoff, privacy and report structure. The two-engine distinction, firing acceptance suite and platform-verification caveats are explicit extensions based on the sources below. Proposed tests and adapter design are implementation requirements, not claims that those components were run during preparation.

**U1.** Owner-supplied `GPT_README_scheduled_tasks_implementation_2026-09-20.md`, especially §§1–6; §7 is treated as a set of platform assertions requiring current verification, not an unqualified authority.

**R1.** Control repository at `517efcdda859abeac0ce3e08196b241e1b72e4b6`: `AGENTS.md`, `scheduled_tasks/README.md`, `scheduled_tasks/PROTOCOL.md`. Owner revision `2026-09-20.1`. Initial README blob `a96970ecdd0dc453b21cd7325785fb01925b27c1`. Pre-delivery README recheck at `21979fc03c79c4bcead152bef2a279a4b3979517` returned revision `2026-09-20.2`, blob `42d8bd3d8853f1eef8d2b6e86fce6500cee89cc4`; other control files in this guide were inspected at the initial pinned control commit.

**R2.** Same control revision: `scheduled_tasks/fleet.json` (blob `e647d5d2479749f80ce7bb4862bee0f28513c7d9`) and `scheduled_tasks/roles.json` (blob `650cc98028c9b3adbaf2a4e4569286f09d6cdb69`).

**R3.** Mathematical baseline `39cfb28999ea514a8a16be7c7ae2123b5419e96a`: `src/math_brain/retrieval.py`, blob `c3a89d5af1a00594b770b3951cd333bc59b4f4e9`; inspected normalization, scoring, `_graph_spread`, retrieval/abstention and dependency-closure portions. Partial source inspection is not a new whole-file execution claim.

**R4.** Memory-engine revision `3fe378e6b15ed02695cc3e008f2f46a175015d26`: `12_cognitive_architecture/dreaming/brain.py` (blob `c07eeec8e5a2cdc108ac34cf6bfd781b864e4a39`, initial 200 source lines inspected) and `spread_recall.py` (blob `cffdc28a850e0ebd1f22634b4271df1e534cbf1b`, initial 190 source lines inspected). These identify the actual recall/spreading interfaces and gating inputs; they do not certify current local deployment or every transitive implementation detail.

**R5.** Same memory-engine revision: `12_cognitive_architecture/dreaming/BRAIN_NODE_DOCUMENTS.md`, blob `d090bc682ec36ba28475fcd8dbd2630c57647a26`; full document inspected.

**R6.** `12_cognitive_architecture/COGNITIVE_ARCHITECTURE.md`, blob `6345f96a4c66e1f780f1df9ca4e01e62f8bcafc6`, initial 180 lines inspected. Architectural descriptions and historical performance claims are not independently rerun evidence.

**R7.** Public mirror `BRAIN_FOR_TASKS.md`, blob `aeba53b6c6cf1f88b9a5fb64e030e14140461d98`, retrieved on 2026-09-20. Treat historical corpus counts and local hook/sync claims as documentation, not verified present runtime state.

**W1–W4.** Official OpenAI pages fetched on 2026-09-20, used only for the explicitly separated platform notes:

```text
W1 https://help.openai.com/en/articles/10291617-chatgpt-tasks
W2 https://help.openai.com/en/articles/8096356-custom-instructions-for-chatgpt
W3 https://help.openai.com/en/articles/10169521-projects-in-chatgpt
W4 https://help.openai.com/en/articles/8554407-gpts-in-chatgpt
```

Fresh account inventory is stronger evidence about that account’s observed registrations than an assumed universal allowance. Neither a help-page limit nor a successful registration proves that a particular runtime, permission or firing backend is operational. Recheck current documentation and tool behavior when deploying.

### Durable integration handoff delivered with this guide

A sanitized technical counterpart, `NODE_FIRING_INTEGRATION_HANDOFF.md`, is included in this bundle and was committed to `scheduled_tasks/work/account01/B19/full-brain-node-firing-handoff-2026-09-20/README.md` at `ef1dcdf904d67e273ff53dd5293ede4cab322b00`. Its readback Git blob `709fbc1cf9ef58b72114f2503d2746d55e716b1a` matched the locally reviewed bytes. It preserves the source discoveries and supplemental firing tests for workers. This documentation delivery did not enroll other accounts, modify schedules, activate strong-node gates or complete the runtime.
