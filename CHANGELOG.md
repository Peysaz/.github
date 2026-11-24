# Peysaz changelog

What changed in Peysaz for the people who use it. Newest first.

## 6.2.0 — 2026-11-24

### Products & pricing

- The list now opens with the most ordered products first and shows 100 rows per page.

### Delivery

- Staff can now see an order's delivery code, whether it went out and whether the driver entered it, and send it again by hand, on both the order and the transport pages, each with its own permission.
- The customer's delivery code can now go out at a chosen stage of the delivery and can travel inside the order's status message, and staff see the progress and result when they turn it on or off.

### Notifications

- Operators can now see what the SMS provider answered for each text message, and whether it was accepted.
- With several panel tabs open, each message result now shows once, in the tab you are looking at.

### Operator tools

- Admins can open a customer's ledger and an order's transactions straight from the order page.
- The users list now shows at a glance which people have switched newsletter messages off, and which ones.

## 6.1.0 — 2026-11-22

### Stock

- Restoring an order to an earlier version now brings its stock along. Delivered units the restored version no longer has go back on the shelf, and the restore saves fully or not at all.

### Delivery

- Staff can now choose per order whether the customer's delivery code is required, starting from a default for new orders.

### Notifications

- A message sent by hand now says plainly whether it went out or why it did not, and login codes and password-reset links are recorded in the messages list.
- Every order and delivery message now shows who sent it, and a driver's urgent message reaches every dispatch phone.
- Every payment message now shows who sent it: the staff member, the paying customer or the system.
- Invoice, low-stock and support messages now show who triggered them, and a failed one stays in the messages list with its reason.
- Staff now see a toast with the result of the messages their own actions send, and a message stopped by a customer's settings shows as blocked in the message list.

### Operator tools

- Every list table now comes with a refresh button, a grouping menu and a chart of its figures.

### Behind the scenes

- Dashboard pages load faster on slow mobile connections.

## 6.0.0 — 2026-11-20

### Delivery

- An order can now carry a note written just for the driver, which the driver sees on the delivery screen once the load is on board and which also shows on the transportation list.
- The driver's delivery screen keeps its main button in reach on any phone, shows the day the customer asked for and the full load list, asks before a load is marked returned, and can call support straight from its problem button.
- The driver's delivery screen now always shows the weather at the destination until the deadline, as one short line on a calm day and in full when a warning is coming.
- The driver's delivery screen now waits a few seconds after each step is tapped, with a countdown and a cancel button, so a mistaken tap can be taken back before it is recorded.

### Reporting

- The charts under the list pages can now draw a share as a ring, rank the few groups behind most of a total, compare this period with the same days of the last one, count every value of a list column, show the amount beside each percent, chart order quantities in their own unit, and appear on the payments page too.
- The charts under the list pages now understand each column, so they total amounts, average prices and percentages, group by Persian calendar months, follow the rows you select, open with a one-line summary, and let you switch between the chart types that fit the data.
- The per-customer balances list now has the same chart under the table as the orders and payments lists, opening on how much is owed each way.

### Accounts & security

- Access can now be managed as named packs of permissions shared by many roles, with a preview of who gains or loses what before a change is saved, and a record of every access change.

### Platform API

- Products no longer carry the retired warehouse capacity value, so integrations that still read it must use the maximum purchase quantity instead.

### Operator tools

- Deleting a product category or subcategory now shows what still uses it before anything is removed, and an empty one takes its storefront page details with it.
- Roles now have a searchable list like the users and orders pages, and one editor for creating and changing a role, with its capabilities grouped by area, searchable, and selectable a whole group at a time.
- The product category and subcategory pages are redesigned, with item counts, image status, a category filter, and each one's storefront page details on its own page.
- The products list now tucks unavailable products into a fold at the end of each group and shows how many orders each product received in the last 90 days.

## 5.0.0 — 2026-11-11

### Ordering

- Customers now see the products they order most often on their dashboard, and one tap opens a new order with that product and its usual quantity filled in.
- Drivers and customers now open the dashboard to their own day: the load in hand with the cash to collect and what is left today, or the order waiting for payment, the delivery on its way and the account balance.

### Invoicing & payments

- Each business can now choose at which order steps its customer invoices are issued, and an invoice amount must be greater than zero.
- The home page now shows your balance as your statement, and the amount takes the same colour as its owed or in-credit badge.

### Notifications

- A broadcast limited to active customers can now also reach everyone who joined recently, within a join window you choose.
- Broadcasts skip blocked people and unverified numbers, and the preview shows who is left out and why.
- Delivery messages to drivers now greet each driver by title and full name.
- Price announcements can go to just the customers you choose by how active they are. Pick a time window and a range, such as the top 30% or from the top 10% to the top 40%, and see who receives it and why.

### Accounts & security

- Staff set an account to active, suspended or blocked from one control on the user page, and the users list shows and filters by that state.
- A suspended person can still sign in but cannot place new orders, and staff cannot book new orders for them either.
- Blocking a person keeps new orders and deliveries off them, and the reason and every past block stay on record. A blocked person receives no broadcasts or automatic messages, and on signing in sees only that the account is blocked, how to reach support and, for a customer, their balance. Integrations that sign people in must handle this new blocked state.
- Deleting a customer now clears their personal details and signs them out everywhere, while their payment history stays on record.

### Operator tools

- The home page now shows staff what is waiting on them, today's orders and deliveries, the latest orders, on-time delivery and recent activity, for a period they choose.
- The integrity page now also checks stored user accounts, phone numbers, notification settings and sent notifications, and lists every one that breaks a rule.
- The orders, invoices, deliveries, notifications and products lists now let you choose how many rows a page shows, with the page controls above and below the table.

### Behind the scenes

- The panel now runs on the latest security releases of the software it is built on.

## 4.3.0 — 2026-10-09

### Ordering

- Operators see how much each order earns over its stock cost while they write it and in the orders list, and saving an order below the minimum first asks them for a reason.

## 4.2.0 — 2026-10-08

### Invoicing & payments

- Orders are now invoiced when payment is due — on delivery, or earlier for prepaid and pay-on-arrival orders — so an order can still be adjusted while it is on the way.

### Behind the scenes

- Every business's data is backed up automatically, encrypted, and test-restored every week.
- Every business on Peysaz runs in its own isolated environment, with its data kept apart from every other business.

## 4.1.0 — 2026-10-07

### Stock

- Warehouses can be counted shelf by shelf, with each difference posted to stock in one step and the expected quantities hidden from whoever does the counting.

## 4.0.0 — 2026-10-07

### Ordering

- Customers now have to give a delivery address before they can place an order.
- Every line of an order can choose which location it is supplied from.
- The simple order view shows complete running totals for products, delivery and the invoice, and the same product can be added on more than one line.
- The simple order view walks through four steps and picks products from a visual catalog.

### Products & pricing

- Catalog prices keep a complete history, and a new price can be scheduled to take effect later.

### Stock

- Each location on the product page shows whether it is ready to sell, and flags stock that has no purchase cost recorded.
- Every stock adjustment records a reason: damage, theft, expiry, count difference, data-entry correction or sample.
- Operators can mark stock as damaged, then later restore it to sale or write it off.
- Stock tracks damaged, quality-control and safety-stock quantities separately, returned goods go to quality control first, and moving stock between locations carries its cost with it.
- The product page lists each location once, with its stock and sale offer side by side.
- Warehouses can be paused at any time, retired once empty and deleted if created by mistake, and removing a location from a product asks for confirmation.

### Invoicing & payments

- Account statements can be exported as PDF or spreadsheet using the page's current filters and a pinned date range.
- Invoices show order-level tax on every line, together with its rate.
- Permanently deleting an order keeps its financial records archived and asks the operator to confirm the money involved first.

### Notifications

- A step-by-step composer for customer messages and price announcements, with an exact preview of the text, who receives it and who is left out.
- Drivers no longer get automatic texts when an order is loaded, arrives or is delivered; operators can still send them on demand.

### Reporting

- Management reports and KPI pages trace order and delivery totals down to the products and customers behind them, with Persian-calendar date ranges and PDF export.

### Accounts & security

- Deleting a user account requires a reason and keeps the account's financial records archived.

### Operator tools

- The panel feels more native on phones, with full-screen iPhone layout, a page-loading indicator and optional haptic feedback.
