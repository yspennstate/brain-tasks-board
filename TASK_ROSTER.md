# Task roster: four accounts, twenty roles each (from the control files, rendered 2026-09-25 01:06)

Order (2026-09-20 18:37): 80 scheduled tasks running at any time, twenty per account, full time every hour, on the
highest reasoning each account offers. Control: `fleet.json` desires 4 accounts x 20 tasks = 80; cadence every 60
minutes; controller slot B20. Capacity and supported cadence depend on the account and task type.
The keeper records the actual inventory, exposed settings and capacity errors separately from this desired allocation.

## Accounts

| account | binding | observed enabled | focus |
|---|---|---|---|
| account01 | CURRENT_AUTHENTICATION_NOT_OBSERVED_IN_THIS_UPDATE | not observed | Quadratic-form bounded density: analytic derivation and exact structural identities |
| account02 | CURRENT_AUTHENTICATION_NOT_OBSERVED_IN_THIS_UPDATE | not observed | Quadratic-form bounded density: complementary constructions and source-valid counterexamples |
| account03 | CURRENT_AUTHENTICATION_NOT_OBSERVED_IN_THIS_UPDATE | not observed | Quadratic-form bounded density: quantitative inequalities and rigorous computations |
| account04 | CURRENT_NATIVE_CONNECTION_OBSERVED | 20 | Quadratic-form bounded density: alternative proof mechanisms and complete-argument integration |

An account is enrolled from inside that account with the instruction in `ONBOARDING.md` (the control repository);
a label is not a login. The profile observations above are historical configuration metadata; consult current inventory and run evidence for each account.

## The twenty roles (the same in every account; B20 keeps the account full and accepts the others' work)

| slot | role | what it does |
|---|---|---|
| B01 | Oscillatory replacement |  |
| B02 | Integrated Fourier estimate |  |
| B03 | Decoupled time integral |  |
| B04 | Product Fourier rearrangement |  |
| B05 | Quadratic coarea bound |  |
| B06 | Curved fiber integration |  |
| B07 | Coordinate minor selection |  |
| B08 | Diffuse eigenvector case |  |
| B09 | Bilinear block mechanism |  |
| B10 | Rank-three coupled case |  |
| B11 | Indefinite signatures |  |
| B12 | Additional eigenvalue control |  |
| B13 | Extremal product laws |  |
| B14 | Translations and localization |  |
| B15 | Absolute continuity and regularity |  |
| B16 | Projection-product interaction |  |
| B17 | Sharp constant and witnesses |  |
| B18 | Literature-to-proof transfer |  |
| B19 | Universal proof assembly |  |
| B20 | Proof closure and keeper |  |

Task name inside ChatGPT: `NN Bxx <role>` (the rendered specification's title, e.g. `02 B01 Source transfer`);
the prompt carries the marker `BRAIN-FLEET v1 account=accountNN slot=Bxx`, which is how a keeper tells managed
tasks from unrelated ones. Render every account's twenty specifications with
`python scheduled_tasks/tools/control.py render --root scheduled_tasks --repository yspennstate/math-research-brain --account accountNN`
from the control repository's root.
