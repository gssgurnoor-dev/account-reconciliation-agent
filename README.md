# Monthly Account Reconciliation Agent

An n8n workflow that automates monthly account reconciliation by comparing
ledger records in Excel/Google Sheets against bank records, flagging
mismatches for review.

## What it does
1. Pulls the ledger and bank data for the period
2. Matches transactions on [amount / date / reference]
3. Flags unmatched or mismatched items
4. Outputs [a reconciliation summary / exceptions sheet / email alert]

## Tools used
- n8n
- Google Sheets / Excel
- [AI model or other integrations]

## How to use
1. Import `monthly-account-reconciliation.json` into n8n (Workflows → Import from file)
2. Connect your own credentials for [Google Sheets, etc.]
3. Point the sheet nodes at your own ledger and bank data
4. Run manually or set a monthly schedule trigger

## Notes
- Sample data only; no real financial records are included
- [Limitations, e.g. tolerance for rounding differences]

![Workflow canvas](screenshot.png)
