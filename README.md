# Pirate P&L Tracker (working draft) — Storage Auction Pirate
Single-file (`index.html`), vanilla JS, phone-first profit & loss tracker. Data lives only in the browser's localStorage (no server/accounts). Rename via `APP_NAME` constant.

## Features
- Unlimited projects (Storage unit / Job / Other): name, date, location, purchase price + buyer's premium (storage) or job income (others), open/sold-out status
- Per-project expenses (help/labor, gas, dump fees, truck, supplies, storage rent, other) and item-by-item sales (eBay, Whatnot, FB Marketplace, yard sale, other) with net
- Summary: total cost (purchase + premium + expenses + sale fees/shipping), total sales, net profit, ROI %
- Dashboard with totals, filterable by year (by project date)
- Exports: per-project CSV, all-transactions CSV (Date, Account/Category, Description, Amount, Project), QuickBooks-friendly CSV (MM/DD/YYYY, Description, Amount, Category, Memo), JSON backup/restore
- "Load demo data" button (no data preloaded); not-tax-advice disclaimer

## Open questions
- Should sale fees count as cost (current) or be netted off sales? ROI changes slightly.
- Year filter uses project date; should it split by transaction date instead?
- Editing existing expense/sale rows (currently delete + re-add only)
- Mileage tracking, photos per item, inventory of unsold items?
- Exact QuickBooks import format (Online bank-upload 3-column vs 4-column) to confirm with Mike's bookkeeper
- Final name/logo
