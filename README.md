# Order-to-Cash Process Analysis

## Project overview
An end-to-end business process analytics project that examines the order-to-cash (O2C) lifecycle: order placement, approval, fulfilment, invoicing and payment. The notebook creates a reproducible synthetic dataset, calculates operational KPIs, highlights process bottlenecks and proposes data-led improvements.

## Business questions
- How long does it take for an order to move from placement to fulfilment?
- Which process stage consumes the most time?
- Do fulfilment performance and delays vary by channel, region or product category?
- What proportion of orders meet the illustrative seven-day fulfilment target?
- How much order value remains outstanding, and how old are those invoices?

## Key analysis
- Data quality checks and order-level process timestamps
- Order cycle time, on-time fulfilment, invoice cycle time and days-to-payment
- Stage duration and channel/region performance comparisons
- Monthly performance trends
- Outstanding invoice ageing
- Practical improvement opportunities

## Repository structure
```text
order-to-cash-process-analysis/
├── README.md
├── requirements.txt
└── notebooks/
    └── order_to_cash_process_analysis.ipynb
```

## Run locally
1. Clone this repository.
2. Create and activate a Python virtual environment (recommended).
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Launch Jupyter:
   ```bash
   jupyter notebook
   ```
5. Open `notebooks/order_to_cash_process_analysis.ipynb` and run all cells.

The notebook generates the sample data and writes CSV outputs to an `outputs/` folder relative to the notebook's working directory.

## Tools
Python, pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook.

## Dataset
The notebook generates 1,200 synthetic order records. No confidential or real customer/company data is used.

## Important assumptions
- The seven-day on-time fulfilment threshold is illustrative, not an industry standard.
- Process durations are measured using timestamps generated for this portfolio exercise.
- Outstanding invoices are identified using a fixed reporting cut-off date in the notebook.
- Findings are examples for demonstrating analytical methods, not claims about a real organisation.

## Suggested next steps
- Add actual business calendars and working-hour calculations.
- Include partial shipments, cancellations, returns and credit notes.
- Compare actual performance with agreed SLA/contractual targets.
- Build a Power BI dashboard using the exported CSV files.
