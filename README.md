# Tea Counter — Billing App

A simple, free billing app for a tea shop. It runs entirely in the browser — no
internet connection, server, or account needed once the page is open. Everything
(menu items and past bills) is saved on the computer/tablet it's used on.

## How to put this online (GitHub Pages) — no coding needed

1. Create a free account at https://github.com if you don't have one.
2. Click the **+** icon (top right) → **New repository**. Name it anything,
   e.g. `tea-counter`. Set it to **Public**. Click **Create repository**.
3. On the new repository page, click **Add file → Upload files**.
4. Drag in the `index.html` file from this folder, then click **Commit changes**.
5. Go to the repository's **Settings** tab → **Pages** (left sidebar).
6. Under "Build and deployment", set **Source** to **Deploy from a branch**,
   Branch: **main**, Folder: **/(root)**. Click **Save**.
7. Wait about a minute, then refresh the page — a link will appear like:
   `https://yourusername.github.io/tea-counter/`
8. Open that link on the shop's computer, tablet, or phone. Bookmark it —
   that's the billing app.

## Using it day to day

- **Billing tab** — tap an item to add it to the bill on the right. Use the
  **+ / −** buttons to adjust quantity. Tap **Save & Print** when the customer
  is ready to pay — this saves the bill and opens the print dialog.
- **Menu tab** — add, edit, or delete items and their prices here.
- **History tab** — see every bill ever printed, grouped by day, with each
  day's total. You can reprint any past bill.
- **Settings tab** — set the shop name, address, phone number, currency
  symbol, and the note printed at the bottom of every bill.

## Printing

The print layout is set up for an **80mm thermal receipt printer**. If you
print to a normal printer/PDF instead, the receipt will still print correctly,
just on a narrow strip of the page.

## Important note about saved data

Menu items and bill history are stored in the browser on the device you're
using — not on the internet. That means:
- Always use the **same device and same browser** (e.g. always Chrome on the
  same tablet) for billing, so history isn't split across places.
- Clearing the browser's history/cache/site data will erase saved bills and
  menu items — avoid doing that.
- There's no login and no cloud backup. If you want a backup, you can
  periodically screenshot or note down the day totals from the History tab.

## Customizing further

Everything is in a single file, `index.html`, including the design and logic.
You (or anyone helping you) can open it in any text editor to make changes —
no build tools or installation required.
