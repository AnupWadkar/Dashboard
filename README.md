# Shree Provision Dashboard

A first-stage React + Vite dashboard for recording daily shop operations.

## Run locally
1. Install Node.js (LTS).
2. Extract this ZIP.
3. Open a terminal in the project folder.
4. Run:
   ```bash
   npm install
   npm run dev
   ```
5. Open the local URL printed by Vite (usually http://localhost:5173).

## Included
- Overview of today's recorded sales, payment split, outstanding udhaar and low-stock items.
- Daily sales/cash entries (cash, UPI, new credit, udhaar collections).
- Customer credit ledger with opening balances, credit limits, due dates and repayment recording.
- Product inventory with minimum stock levels.
- Purchase entry that increases product stock.
- Expense entry and cash drawer closing reconciliation.
- CSV exports and a JSON backup of all records.
- Responsive desktop/mobile layout.

## Important limitations (version 1)
- Data is stored in browser localStorage on this device only. It is not shared between Pune and the shop.
- Export a JSON backup regularly. Clearing browser data can erase records.
- This is a prototype, not audited accounting software. Verify each entry against actual cash, UPI and notebook records.
- The daily entry is a daily summary, not item-by-item POS billing.
- Do not enter sensitive customer information beyond what is needed for the ledger.
- Before using real balances, reconcile all 30 customer accounts against the existing notebook.
- For multi-device access, login/security, shared records and automatic remote monitoring, add a backend (e.g. Node/Express + PostgreSQL) in a later version.

## Suggested first setup
1. Add customers one by one using the verified current notebook balance.
2. Add the 50 fastest-selling products and physically counted stock.
3. Enter purchases and expenses as they happen.
4. Enter one daily sales summary after shop closing.
5. Close cash and compare expected vs counted cash.
6. Export the JSON backup at the end of each week.
