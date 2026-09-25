# Task roster: four accounts, twenty roles each (from the control files, rendered 2026-09-25 17:06)

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
| B01 | Repaired theorem and dependency audit |  |
| B02 | Fourier and negative moment audit |  |
| B03 | Conditioning and independence audit |  |
| B04 | Heat-flow proof and limits audit |  |
| B05 | Projection and zero-density domain audit |  |
| B06 | Integrated Fourier powers audit |  |
| B07 | Gram and padded singular-index audit |  |
| B08 | Entropy and row-promotion audit |  |
| B09 | Complex measure and L2 measurability audit |  |
| B10 | Random-sign extraction audit |  |
| B11 | Schur threshold and singular-limit audit |  |
| B12 | Scalar critical-value density audit |  |
| B13 | Definite-pair chart and null seam audit |  |
| B14 | Hyperbolic tails and critical level audit |  |
| B15 | Rearrangement and extended kernels audit |  |
| B16 | Full half-potential dependency audit |  |
| B17 | Constants final cases and scaling audit |  |
| B18 | All-report reconciliation and reference audit |  |
| B19 | Independent repaired-source end-to-end audit |  |
| B20 | Whole-paper audit and own-account coordination |  |

Task name inside ChatGPT: `NN Bxx <role>` (the rendered specification's title, e.g. `02 B01 Source transfer`);
the prompt carries the marker `BRAIN-FLEET v1 account=accountNN slot=Bxx`, which is how a keeper tells managed
tasks from unrelated ones. Render every account's twenty specifications with
`python scheduled_tasks/tools/control.py render --root scheduled_tasks --repository yspennstate/math-research-brain --account accountNN`
from the control repository's root.
