# Supply Chain BI — Delivery Performance Dashboard

A Power BI portfolio project exploring supply-chain delivery performance and the business metrics associated with delayed orders. The report is designed to help users compare delay patterns across markets, customer segments, shipping methods, and product categories.

## Dashboard preview

![Supply Chain BI dashboard preview](SUPPLY%20CHAIN%20DASHBOARD.png)

## Business questions

- How many orders are delayed, and what share of orders does that represent?
- How long are deliveries delayed on average?
- How do delay patterns differ across markets, customer segments, and shipping methods?
- Which product categories and markets are associated with the most revenue and profit among delayed orders?
- Where should a supply-chain team investigate potential delivery-performance issues first?

## Report contents

The Power BI report includes KPI cards and interactive views for exploring delivery delays, market-level patterns, product categories, revenue, and profit. Filters allow users to investigate subsets of the data rather than relying only on top-level totals.

The measures displayed in the report include:

- Delayed-order count and delayed-order percentage
- Average delivery delay
- Value associated with delayed orders
- Profit associated with delayed orders

**Metric interpretation:** revenue or profit associated with delayed orders is not automatically a financial loss caused by the delay. Establishing a causal financial impact would require additional evidence, such as cancellation, refund, penalty, or customer-retention data.

## Tools

- **Microsoft Power BI Desktop** — report authoring and interactive visualisation
- **Power BI measures and filters** — KPI calculation and report exploration
- **Data visualisation** — KPI cards, comparison charts, and category-level breakdowns

## Repository files

- `Optymalizacja łańcucha dostaw — Supply Chain BI.pbix` — Power BI report
- `SUPPLY CHAIN DASHBOARD.png` — static dashboard preview

## How to explore the report

1. Download the `.pbix` file from this repository.
2. Open it in Microsoft Power BI Desktop.
3. Use the report filters to compare delivery performance across the available business dimensions.
4. Select individual charts or categories to explore related details.

The PNG file is a static preview; interactions are available in Power BI Desktop.

## Data notes and limitations

- A separate source-data file is not included in this repository.
- The original dataset source, time period, currency, and usage licence are not documented in the repository yet. These details should be verified and added before the project is presented as a fully reproducible case study.
- Before relying on the displayed KPI values, validate the underlying measure definitions. In particular, confirm that order counts use unique order identifiers where appropriate and that percentage denominators remain correct when report filters are applied.
- Document the exact definition of “average delay” (for example, whether it is calculated only for late deliveries) so that users can interpret the KPI consistently.

## Possible next improvements

- Document the dataset source, time range, and definitions for every KPI.
- Validate the DAX measures against a small set of manually checked records.
- Keep late-delivery rate separate from each market's share of all late deliveries; these answer different business questions.
- Add a concise executive summary with the three strongest findings supported by the data.
- Improve the report's visual hierarchy so the main KPIs and comparisons are easy to scan.

## Author

Created as a data analytics portfolio project by [MaciejK-ops](https://github.com/MaciejK-ops).
