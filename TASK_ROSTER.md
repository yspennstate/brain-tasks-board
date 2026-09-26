# Task roster: four accounts, twenty roles each (from the control files, rendered 2026-09-26 10:20)

Order (2026-09-20 18:37): 80 scheduled tasks running at any time, twenty per account, full time every hour, on the
highest reasoning each account offers. Control: `fleet.json` desires 4 accounts x 20 tasks = 80; cadence every 60
minutes; controller slot B20. Capacity and supported cadence depend on the account and task type.
The keeper records the actual inventory, exposed settings and capacity errors separately from this desired allocation.

## Accounts

| account | binding | observed enabled | focus |
|---|---|---|---|
| account01 | CURRENT_NATIVE_SCHEDULER_NOT_OBSERVED_THIS_UPDATE | not observed | Repeated full repaired-manuscript audits; forward derivation and reverse dependency checks |
| account02 | CURRENT_NATIVE_SCHEDULER_NOT_OBSERVED_THIS_UPDATE | not observed | Repeated full repaired-manuscript audits; adversarial and boundary cases |
| account03 | CURRENT_NATIVE_SCHEDULER_NOT_OBSERVED_THIS_UPDATE | not observed | Repeated full repaired-manuscript audits; identities, constants and alternative derivations |
| account04 | CURRENT_NATIVE_SCHEDULER_PROFILE_OBSERVED | 20 | Mandatory repeated full repaired-manuscript audits; old three-value discovery superseded |

An account is enrolled from inside that account with the instruction in `ONBOARDING.md` (the control repository);
a label is not a login. The profile observations above are historical configuration metadata; consult current inventory and run evidence for each account.

## The twenty roles (the same in every account; B20 keeps the account full and accepts the others' work)

| slot | role | what it does |
|---|---|---|
| B01 | Architecture and claims inventory |  |
| B02 | Memory recall engine |  |
| B03 | Association graph and edges |  |
| B04 | Reflexes and instincts |  |
| B05 | Hooks and delivery |  |
| B06 | Dreaming and consolidation |  |
| B07 | The math brain claim graph |  |
| B08 | Brain-on versus brain-off evidence |  |
| B09 | The paper, claim by claim |  |
| B10 | The paper's mathematics |  |
| B11 | Related work and novelty |  |
| B12 | How to test the brain's strengths more |  |
| B13 | Mistakes and scars |  |
| B14 | Owner orders reaching action |  |
| B15 | Coordination |  |
| B16 | Cost and efficiency |  |
| B17 | Privacy, security and sanitisation |  |
| B18 | Portability and reproducibility |  |
| B19 | Synthesis for publication |  |
| B20 | Gap finder and keeper |  |

Task name inside ChatGPT: `NN Bxx <role>` (the rendered specification's title, e.g. `02 B01 Source transfer`);
the prompt carries the marker `BRAIN-FLEET v1 account=accountNN slot=Bxx`, which is how a keeper tells managed
tasks from unrelated ones. Render every account's twenty specifications with
`python scheduled_tasks/tools/control.py render --root scheduled_tasks --repository yspennstate/math-research-brain --account accountNN`
from the control repository's root.
