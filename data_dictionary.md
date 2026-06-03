# Data Dictionary

Descriptions of variables in `sim_data_simple_wide.csv` and `sim_data_full_wide.csv`.

Both datasets contain simulated data from an embodied learning study.
Participants completed a knowledge test (8 items) before and after a learning intervention.
The intervention had two conditions: control and embodied.

---

## Shared variables

Both datasets contain the following variables:

| Variable | Type | Description |
|---|---|---|
| `pid` | character | Participant identifier (e.g. `P001`) |
| `group` | factor | Condition assignment: `control` or `embodied` |
| `pre_score_z` | numeric | Standardised pre-test score (z-scored). One value per participant, repeated across rows where applicable. Used as a covariate to adjust for baseline differences between participants. |
| `item_1` | integer | Response to item 1: `0` = incorrect, `1` = correct |
| `item_17` | integer | Response to item 17: `0` = incorrect, `1` = correct |
| `item_19` | integer | Response to item 19: `0` = incorrect, `1` = correct |
| `item_22` | integer | Response to item 22: `0` = incorrect, `1` = correct |
| `item_23` | integer | Response to item 23: `0` = incorrect, `1` = correct |
| `item_25` | integer | Response to item 25: `0` = incorrect, `1` = correct |
| `item_26` | integer | Response to item 26: `0` = incorrect, `1` = correct |
| `item_28` | integer | Response to item 28: `0` = incorrect, `1` = correct |

Item numbers reflect the original item numbering from the source study.

---

## sim_data_simple_wide.csv

Post-test responses only.
Each row is one participant.

**Dimensions:** 108 rows × 11 columns

---

## sim_data_full_wide.csv

Post-test and one-week delay test responses.
Each row is one participant at one test time.

**Additional variable:**

| Variable | Type | Description |
|---|---|---|
| `test_time` | factor | Test occasion: `post` = immediately after intervention, `delay` = one week later |

Note: `pre_score_z` is constant within participant across `test_time` levels,
as it reflects a single baseline measurement taken before the intervention.

**Dimensions:** 216 rows × 12 columns
