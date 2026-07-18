# Tea Counter — Billing App

A simple, free billing app for a tea shop. It runs entirely in the browser — no
internet connection, server, or account needed once the page is open. Everything
(menu items and past bills) is saved on the computer/tablet it's used on.

## How to put this online (GitHub Pages) — no coding needed

If you're setting this up for the first time, follow the steps below.

If you already have this app live on GitHub Pages and just want to push this
**updated** `index.html` (with the new WhatsApp and Google Pay options) live:

1. Open your repository on github.com (e.g. `github.com/yourusername/tea-counter`).
2. Click on `index.html` in the file list, then click the pencil (✏️) **Edit**
   icon at the top right of the file view.
3. Select all the text in the editor (Ctrl/Cmd + A) and delete it.
4. Open the new `index.html` from this download, select all its content,
   copy it, and paste it into the GitHub editor.
5. Scroll down and click **Commit changes**.
6. Wait about a minute, then refresh your live site link — the new options
   will appear automatically for every customer who visits it. There's
   nothing else to install or configure.

(Alternatively: **Add file → Upload files**, drag in the new `index.html`,
and GitHub will ask to replace the existing one — either method works.)

If this is your first time hosting it, here's the full setup:

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

## Accepting Google Pay / UPI payments

This app can't process payments itself — a plain GitHub Pages site has no
server or bank connection, so there's no real "checkout" possible here.
Instead it uses the same method most small Indian shops already use:

1. In **Settings**, enter your shop's **UPI ID** (the one linked to your
   Google Pay, PhonePe, Paytm, or bank app — looks like `yourname@okaxis`).
2. On the **Billing tab**, once items are added, tap **Google Pay / UPI**
   instead of Cash. A QR code appears for the exact bill amount.
3. The customer scans it with Google Pay (or any UPI app — they all read the
   same code) and pays you directly. The money goes straight to your bank
   account; nothing passes through this app or GitHub.
4. Tap **Save & Print** as usual once you've confirmed the payment came in.
   The receipt notes whether the bill was paid by Cash or UPI.

## Sending receipts on WhatsApp

Like the payment option, this uses WhatsApp's free "click to chat" link — there's
no WhatsApp Business account, API key, or backend needed.

- On the **Billing tab**, type the customer's 10-digit mobile number into the
  **"Send receipt on WhatsApp"** field, then tap the **Send** button next to
  it. WhatsApp opens in a new tab/app with the bill details already filled
  in — just tap **Send** inside WhatsApp to deliver it.
- This works independently of **Save & Print** — you can send the WhatsApp
  message, print, both, or neither, in any order, before saving the bill.
- You can also send (or re-send) any past bill from the **History tab** using
  the **💬 WhatsApp** button next to it.
- This sends a text summary of the bill (items, total, payment method), not
  a photo of the printed slip — WhatsApp's link-based sending doesn't support
  attaching files automatically.
- Numbers are assumed to be Indian mobile numbers (10 digits). To use a
  different country's number, type it with a `+countrycode` prefix, e.g.
  `+14155552671`.

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
