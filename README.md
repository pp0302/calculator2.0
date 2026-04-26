# PWM Retirement Planner

A single-file retirement compensation calculator for PWM advisors. Open `index.html` in any modern browser — no build step or server required.

## Features

- **Overview** — KPI cards, compensation summary (working phase / retirement phase / grand total), income timeline charts, and payout multiple display
- **Working Phase** — annual compensation schedule with grid bonus breakdown and deferred comp grant schedule
- **Retirement** — 5-year PWM benefit schedule, deferred comp delivery tail, and combined income waterfall
- **Scenario Analysis** — retirement timing sensitivity table and domicile tax comparison

## Inputs

| Input | Description |
|---|---|
| Current Revenue | Starting book revenue |
| Current Tenure | Years of service at present |
| Years Until Retirement | Working years remaining |
| Working Phase Rev Growth | Annual revenue growth rate during working years |
| Retirement Benefit Growth | Annual growth applied to PWM benefit payments |
| GS Share Price | Live-fetched from Yahoo Finance; falls back to manual entry |
| Annual Stock Growth Rate | Projected GS share price appreciation |
| Existing Unvested Shares | Up to 3 upcoming gross share deliveries |
| Working / Retirement State | State income tax rates applied to each phase |
| Alt. Comparison State | Used in domicile tax comparison (Section 5.3) |

## Tax Toggle

Switch between **Pre-Tax** and **Post-Tax** views using the toggle in the header. All tables, KPI cards, and charts update simultaneously.

## Export

- **CSV** — exports working phase compensation table with inputs
- **PDF** — prints all panels with a clean letterhead layout (A4 landscape)
- **Save / Restore Inputs** — persists inputs to localStorage for the current browser
