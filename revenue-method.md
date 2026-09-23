# How the revenue numbers were measured

*Last checked: September 23, 2026. This page exists because chapter 4 says a number without a method is a belief, and the front page carries four numbers.*

## What the front page says

Completed-job revenue for the six weeks after the phone agent went live (August 9 to September 18, 2026) was 56 percent above the same six weeks of 2025 and 62 percent above 2024. The six weeks before it went live were up 11 percent over 2025. Year to date the shop was 14 percent over 2025.

## Where those came from

The owner pulled them from the CRM's own reports screen on September 19, 2026. That export is not published; it holds customer names.

## An independent re-pull, September 23, 2026

To check the owner's reading, the same windows were re-pulled straight from the CRM's API with a short script (kept in the shop's private booking repository; it prints totals only and never customer data). Definition used:

- **A job counts** when its status is complete and it has a completion timestamp; the date is the completion date, not the booking date.
- **Revenue** is the job's total as invoiced, including parts, labor, and tax.
- **Windows** are the same calendar dates in each year. 5,901 completed jobs from May 2020 to September 22, 2026 were in the pull.

| Window | Owner's reading (9/19) | Re-pull (9/23) | Jobs in window, 2026 vs prior year |
|---|---:|---:|---|
| Six weeks since go-live vs same weeks 2025 | +56% | +57% | 114 vs 85 |
| Same, vs 2024 | +62% | +62% | 114 vs 68 |
| Six weeks before go-live vs 2025 | +11% | +14% | 117 vs 104 |
| Year to date through September 19 vs 2025 | +14% | +13% | 594 vs 552 |

The two readings differ by a point or three because the dashboard report and the API pull do not define "completed" and "date" identically; neither definition is wrong, and the story is the same under both.

## What the numbers do not prove

- Six-week windows are small for a one-truck shop. A few large jobs move them.
- The phone agent was not the only thing that changed in August 2026: the owner also worked the Google listing and the ads. The number is the shop's result, not the agent's alone.
- "Year to date" includes seven months before the agent existed, so it says less about the agent than the six-week line does.
- Dollar totals are not published. Percentages and job counts are.
