# Task roster: four accounts, twenty roles each (from the control files, rendered 2026-09-25 07:51)

Order (2026-09-20 18:37): 80 scheduled tasks running at any time, twenty per account, full time every hour, on the
highest reasoning each account offers. Control: `fleet.json` desires 4 accounts x 20 tasks = 80; cadence every 60
minutes; controller slot B20. Capacity and supported cadence depend on the account and task type.
The keeper records the actual inventory, exposed settings and capacity errors separately from this desired allocation.

## Accounts

| account | binding | observed enabled | focus |
|---|---|---|---|
| account01 | CURRENT_NATIVE_SCHEDULER_NOT_OBSERVED_THIS_UPDATE | not observed | Exclusive repeated full-manuscript line audits: forward derivation and reverse dependency checks |
| account02 | CURRENT_NATIVE_SCHEDULER_NOT_OBSERVED_THIS_UPDATE | not observed | Exclusive repeated full-manuscript line audits: adversarial falsification and boundary cases |
| account03 | CURRENT_NATIVE_SCHEDULER_PROFILE_OBSERVED | 20 | Exclusive repeated full-manuscript line audits: exact identities, constants and alternative derivations |
| account04 | CURRENT_NATIVE_SCHEDULER_NOT_OBSERVED_THIS_UPDATE | not observed | Exclusive repeated full-manuscript line audits: independent reconstruction and disagreement resolution |

An account is enrolled from inside that account with the instruction in `ONBOARDING.md` (the control repository);
a label is not a login. The profile observations above are historical configuration metadata; consult current inventory and run evidence for each account.

## The twenty roles (the same in every account; B20 keeps the account full and accepts the others' work)

| slot | role | what it does |
|---|---|---|
| B01 | Theorem and dependency audit |  |
| B02 | Fourier and half-potential audit |  |
| B03 | Conditioning and independence audit |  |
| B04 | Heat-flow proof audit |  |
| B05 | Product-projection proof audit |  |
| B06 | Holder and entropy audit |  |
| B07 | Crossing-volume identity audit |  |
| B08 | Complex-measure and Jensen audit |  |
| B09 | Mollification and convergence audit |  |
| B10 | Exact numerical-constant audit |  |
| B11 | Schur and singular-value audit |  |
| B12 | Scalar and potential-kernel audit |  |
| B13 | Two-coordinate chart and tail audit |  |
| B14 | Measurability and rough-law audit |  |
| B15 | Density existence and inversion audit |  |
| B16 | Random-sign spectral proof audit |  |
| B17 | Final cases and threshold-boundary audit |  |
| B18 | Imported-hypothesis and reference audit |  |
| B19 | Independent end-to-end reconstruction audit |  |
| B20 | Independent audit and own-account coordination |  |

Task name inside ChatGPT: `NN Bxx <role>` (the rendered specification's title, e.g. `02 B01 Source transfer`);
the prompt carries the marker `BRAIN-FLEET v1 account=accountNN slot=Bxx`, which is how a keeper tells managed
tasks from unrelated ones. Render every account's twenty specifications with
`python scheduled_tasks/tools/control.py render --root scheduled_tasks --repository yspennstate/math-research-brain --account accountNN`
from the control repository's root.
