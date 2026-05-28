# test-repo

## SRR Sales Commission Calculator

An interactive commission calculator for Saddle River Roofing sales reps, based on
the **price per Square** sold using a **marginal-bracket** model:

| Tier        | Default range         | Rate | Who                          |
|-------------|-----------------------|------|------------------------------|
| Floor       | up to $400/sq         | 5%   | rep (top line)               |
| Par         | $400 → $550/sq        | 10%  | rep                          |
| Overage     | anything above $550/sq| 50%  | split 50/50 rep / house      |

Each slice of the price per Square is paid at its own rate (like tax brackets), then
multiplied by the number of squares to get the rep's total commission.

### Use it

Open [`commission-calculator.html`](commission-calculator.html) in any web browser —
no install required. Enter the sale price per Square and number of squares; the
breakdown, effective rate, and house split update instantly. Floor/par thresholds
and all three rates are editable to model different plans.

**Example:** 30 squares at $600/sq (floor $400, par $550) → rep earns **$60/sq =
$1,800** (10% effective), with the house keeping $750 of the overage.
