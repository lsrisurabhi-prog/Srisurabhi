# Asian Paints — Three-Statement Financial Model & DCF Valuation

## Project Overview

This project presents an integrated three-statement financial model, discounted cash flow valuation and investment thesis for **Asian Paints Limited**.

The model combines four years of historical financial information with a five-year forecast from FY27 to FY31. It was developed to understand the company’s operating performance, working-capital requirements, capital investment, cash generation and potential intrinsic value under different assumptions.

> **Important learning:** A model can be mechanically correct while its valuation remains highly dependent on judgment. My initial base case was moderately optimistic, so I used sensitivity and scenario analysis to demonstrate the uncertainty surrounding the valuation.

---

## Repository Contents

```text
Asian-Paints-Equity-Research/
│
├── README.md
├── Asian_Paints_Equity_Research_Model.xlsx
└── screenshots/
    ├── 01_Cover.png
    ├── 02_Investment_Thesis.png
    ├── 03_Financial_Model.png
    ├── 04_Valuation_Output.png
    └── 05_Sensitivity_and_Scenarios.png
```

---

## Model Components

The workbook includes:

- Four years of historical financial statements
- Five-year forecast income statement
- Five-year forecast balance sheet
- Five-year forecast cash-flow statement
- Revenue, margin, tax and dividend assumptions
- Inventory, receivable and payable-day drivers
- PPE and capital-expenditure schedule
- Working-capital schedule
- Debt and lease-obligation schedule
- Unlevered free-cash-flow calculation
- WACC and Gordon Growth terminal-value calculation
- Enterprise-value-to-equity-value bridge
- WACC and terminal-growth sensitivity analysis
- Bear, base and bull scenarios
- Automated balance-sheet, cash and valuation checks
- Sources and model-audit documentation
- Model-linked investment thesis

---

## Investment Thesis

Asian Paints remains a high-quality paint and décor franchise supported by:

- Strong consumer brand recognition
- Manufacturing and distribution scale
- Broad product portfolio
- Dealer, painter and contractor relationships
- Waterproofing and construction-chemical offerings
- Professional painting services
- An expanding home décor ecosystem

The model assumes that the weakness experienced in recent years is primarily cyclical rather than permanent. Under the base case, decorative-paints demand gradually recovers while operating margins remain broadly stable.

However, this recovery is not assured.

Birla Opus has materially increased competitive intensity through manufacturing capacity, distribution expansion, advertising and dealer acquisition. This creates risks to Asian Paints’ market share, pricing power, product mix, dealer economics and margins.

The resulting thesis is therefore **cautiously constructive**, with meaningful competitive and valuation risk. It is not an unconditional investment recommendation.

---

## Historical Performance

Asian Paints’ consolidated revenue from operations was:

| Fiscal Year | Revenue (₹ Cr) |
|---|---:|
| FY23 | 34,489 |
| FY24 | 35,495 |
| FY25 | 33,906 |
| FY26 | 35,584 |

Recent growth was considerably weaker than the forecast period. Therefore, the base case represents a **recovery assumption**, not a continuation of historical growth.

---

## Forecast Approach

### Revenue

Revenue is forecast using annual growth assumptions that gradually decline across the projection period:

| Fiscal Year | Revenue Growth |
|---|---:|
| FY27 | 9.5% |
| FY28 | 9.5% |
| FY29 | 9.0% |
| FY30 | 8.5% |
| FY31 | 8.0% |

This is the model’s most demanding assumption. It requires:

- Recovery in decorative-paints demand
- Stronger volume growth
- Improved price and product mix
- Continued channel relevance
- Limited permanent market-share loss

### Operating Expenses

Operating expenses are modeled using:

- Gross-margin assumptions
- Employee-cost growth
- Other expenses as a percentage of revenue
- Depreciation as a percentage of revenue
- Finance costs as a percentage of revenue
- An effective tax rate of 26%

The model assumes broadly stable profitability rather than substantial margin expansion.

### Working Capital

Operating working capital is forecast using:

- Inventory days: 105
- Receivable days: 46
- Payable days: 71

The change in net working capital affects both the cash-flow statement and unlevered free cash flow.

### Capital Expenditure

Capital expenditure is forecast at approximately 5% of revenue.

Property, plant and equipment is modeled using the following roll-forward:

```text
Closing PPE = Opening PPE + Capital Expenditure − Depreciation
```

### Equity

Shareholders’ equity is rolled forward using:

```text
Closing Equity = Opening Equity + Profit After Tax − Dividends
```

### Cash

Closing cash is calculated through the cash-flow statement:

```text
Closing Cash = Opening Cash + CFO + CFI + CFF
```

The resulting closing cash balance is linked back to the balance sheet.

---

## DCF Methodology

The valuation uses **unlevered free cash flow**, also referred to as FCFF or UFCF.

```text
UFCF = EBIT × (1 − Tax Rate)
       + Depreciation & Amortisation
       − Capital Expenditure
       − Change in Net Working Capital
```

### Why these adjustments are made

- **EBIT × (1 − tax rate):** measures after-tax operating profit before financing decisions.
- **D&A is added back:** it reduces accounting profit but is not a current-period cash outflow.
- **Capital expenditure is deducted:** it represents real cash invested in long-term operating assets.
- **Increase in NWC is deducted:** it represents cash tied up in inventory and receivables, net of operating liabilities.

---

## Discounting the Cash Flows

Future cash flows are worth less than equivalent cash received today.

Each forecast UFCF is multiplied by a discount factor:

```text
Discount Factor = 1 ÷ (1 + WACC)^t
```

```text
Present Value of UFCF = UFCF × Discount Factor
```

The weighted average cost of capital represents the required return of the company’s debt and equity capital providers.

---

## WACC Assumptions

| Assumption | Base Case |
|---|---:|
| Risk-free rate | 6.6% |
| Equity risk premium | 5.5% |
| Levered beta | 0.65 |
| Cost of equity | 10.2% |
| Pre-tax cost of debt | 8.0% |
| Equity weight | 95.0% |
| Debt weight | 5.0% |
| WACC | Approximately 10.0% |

Cost of equity is calculated using CAPM:

```text
Cost of Equity = Risk-free Rate + Beta × Equity Risk Premium
```

The 0.65 beta is a judgment-based defensive-business proxy and represents a limitation of the current model. A future improvement would be to calculate beta using a market regression or peer unlevering and relevering analysis.

---

## Terminal Value

Cash flows beyond FY31 are represented through a Gordon Growth terminal value:

```text
Terminal Value =
Final-Year UFCF × (1 + Terminal Growth Rate)
÷ (WACC − Terminal Growth Rate)
```

The base case uses a terminal growth rate of 5%.

This assumption is optimistic and has a significant effect on valuation. More conservative analysis may use a terminal growth rate of approximately 4%–4.5%.

Terminal value is discounted to the valuation date using the same WACC applied to forecast UFCF.

---

## Enterprise Value to Equity Value

Discounting FCFF produces enterprise value because FCFF belongs to both debt and equity capital providers.

```text
Enterprise Value =
PV of Forecast UFCF + PV of Terminal Value
```

Enterprise value is converted into equity value using:

```text
Equity Value =
Enterprise Value
− Borrowings and Lease Obligations
+ Cash and Current Investments
− Non-Controlling Interests
```

Finally:

```text
Implied Value per Share =
Equity Value ÷ Diluted Shares Outstanding
```

---

## Valuation Summary

| Scenario | UFCF Multiplier | WACC | Terminal Growth | Implied Value per Share |
|---|---:|---:|---:|---:|
| Bear | 0.85x | 11.0% | 4.5% | ₹674 |
| Base | 1.00x | 10.0% | 5.0% | ₹1,004 |
| Bull | 1.15x | 9.0% | 5.5% | ₹1,612 |

The primary DCF produces an implied value of approximately **₹1,012 per share** because it uses the calculated WACC of approximately 9.96%, while the scenario table uses a rounded 10% WACC.

The wide valuation range demonstrates the sensitivity of DCF results to cash-flow, WACC and perpetual-growth assumptions.

---

## Key Risks

### Competitive Intensity

Birla Opus and other competitors may increase pressure through:

- Dealer incentives
- Promotional spending
- Aggressive pricing
- Product launches
- Distribution expansion
- Manufacturing-capacity additions

### Demand Weakness

Consumers may continue postponing discretionary repainting activity, particularly if urban demand and household sentiment remain weak.

### Downtrading

Customers may move toward economy products, causing volume growth to exceed revenue growth while reducing profitability per litre.

### Raw-Material Inflation

Paint production is raw-material intensive. Crude-linked input inflation may compress gross margins if price increases cannot be passed on to customers.

### Forecast Risk

The model assumes revenue growth of 8%–9.5%, considerably above recent historical growth. Failure to achieve this recovery would reduce UFCF and valuation.

### Terminal-Value Risk

A significant portion of enterprise value comes from terminal value. Small changes in WACC or terminal growth can materially change the final output.

---

## Potential Catalysts

- Recovery in decorative-paints demand
- Improvement in urban consumer sentiment
- Stronger volume growth
- Better price and premium-product mix
- Stable gross and EBITDA margins
- Growth in waterproofing and construction chemicals
- Expansion of professional painting services
- Stronger B2B and institutional demand
- Reduced competitive or promotional intensity
- Improved cash conversion

---

## Key Learning Outcomes

This project strengthened my understanding of:

- Forecast-line-item selection
- Three-statement integration
- Balance-sheet roll-forwards
- Cash-flow derivation
- Working-capital forecasting
- Supporting-schedule construction
- Unlevered free cash flow
- Time value of money
- WACC and CAPM
- Terminal value
- Enterprise value versus equity value
- Sensitivity and scenario analysis
- Model auditing and balance checks
- The effect of judgment and bias on valuation

The most important lesson was:

> A formula can be mechanically correct while its output remains highly dependent on judgment.

---

## Skills Demonstrated

- Financial-statement analysis
- Three-statement financial modeling
- Forecast-driver development
- Working-capital modeling
- Supporting schedules
- DCF valuation
- WACC estimation
- Scenario analysis
- Sensitivity analysis
- Investment-thesis development
- Excel model auditing
- Financial presentation

---

## Data Sources

The project primarily uses publicly available information from:

- Asian Paints annual reports
- Asian Paints investor disclosures and financial results
- Reserve Bank of India market information
- Public equity-risk-premium and valuation references
- Grasim Industries disclosures relating to Birla Opus

Detailed links and assumption notes are included in the workbook’s **Sources & Audit** and **Investment Thesis** tabs.

---

## Use of AI Tools

I independently developed the project’s historical financial statements and forecast-model foundation.

AI tools were used to assist with:

- Formula diagnostics
- Accounting-link review
- Balance-sheet reconciliation
- Supporting-schedule development
- DCF framework construction
- Scenario and sensitivity analysis
- Source research
- Investment-thesis structuring
- Model checks and presentation formatting

I reviewed the resulting calculations and used the process to strengthen my understanding of three-statement modeling and valuation.

---

## Disclaimer

This project was prepared solely for educational and portfolio purposes using publicly available information.

It does not constitute investment advice or a recommendation to buy, sell or hold Asian Paints Limited or any other security.

Forecasts, assumptions and valuation outputs are illustrative estimates and may differ materially from actual results.

---

## Connect

**GitHub:** [lsrisurabhi-prog](https://github.com/lsrisurabhi-prog)  
**LinkedIn:** [Insert LinkedIn profile URL]
