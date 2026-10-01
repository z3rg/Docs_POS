# DPos Kasir User Guide — Tablet

**English** · [Bahasa Indonesia](panduan-tablet.md)

A step-by-step guide for every role: **Owner, Manager, Supervisor, Cashier, and Kitchen**.
Applies to **DPos Kasir 1.4.4**. Screenshots were taken on an Android tablet
(Samsung SM-X400, landscape); most of them come from version 1.0.0 and are still
accurate because the layout has not changed.

DPos Kasir works entirely **offline** — there is no server and no internet is needed. All data
is stored on the tablet, so regular backups are the owner's responsibility.

The app is available in **Indonesian and English**. The screenshots in this guide show the
Indonesian interface; see [App language](#14-app-language) for the matching terms in each
language.

Using a phone? See the [Phone Guide](phone-guide.md) — same content, with portrait screenshots
and notes specific to narrow screens.

---

## Contents

1. [Getting Started](#1-getting-started)
2. [Signing In and Out](#2-signing-in-and-out)
3. [Roles and Permissions](#3-roles-and-permissions)
4. [Role Guide: Cashier](#4-role-guide-cashier)
5. [Role Guide: Kitchen](#5-role-guide-kitchen)
6. [Role Guide: Supervisor](#6-role-guide-supervisor)
7. [Role Guide: Manager](#7-role-guide-manager)
8. [Role Guide: Owner](#8-role-guide-owner)
9. [Troubleshooting](#9-troubleshooting)
10. [What's New](#10-whats-new)

---

## 1. Getting Started

### 1.1 First install

The first time the app is opened, the database is empty. The sign-in screen shows a
**"No product data yet"** panel with a *Create Sample Data* button and the list of default PINs.

![Sign-in screen on a fresh install](img/tablet/01-login-baru.png)

Two options:

| Option | When to use it |
| --- | --- |
| **Create Sample Data** | For learning or demos. Fills in products, customers, promos, tables, and sales history so every feature can be tried right away. |
| Sign in directly with PIN `1234` | For a real store. You start from scratch and enter your own products and staff. |

> **Important.** The sample PIN panel only appears while no product has been saved yet.
> As soon as the first data is entered, the panel disappears on its own. Change every default
> PIN in the **Staff** menu before the tablet is used for selling.

### 1.2 After data is entered

The sign-in screen goes back to being clean — just the keypad. The store name above the keypad
follows the **Store Identity** setting.

![Normal sign-in screen](img/tablet/02-login-normal.png)

### 1.3 Sample PINs (demo data only)

| PIN | Name | Role | Outlet |
| --- | --- | --- | --- |
| `1234` | Budi Santoso | Owner | Kopi Nusantara — Pusat |
| `2345` | Siti Rahayu | Manager | Kopi Nusantara — Pusat |
| `3456` | Andi Pratama | Supervisor | Kopi Nusantara — Pusat |
| `4567` | Dewi Lestari | Cashier | Kopi Nusantara — Pusat |
| `5678` | Rizky Maulana | Cashier | Cabang Bandung |
| `9999` | Dapur | Kitchen | Kopi Nusantara — Pusat |

### 1.4 App language

Since version 1.4.0 the entire interface is available in **Indonesian and English** —
including receipts, kitchen tickets, shift reports, and error messages.

![Language setting](img/tablet/42-pengaturan-bahasa.png)

Open **Settings → Language**, then choose one:

| Option | Meaning |
| --- | --- |
| **Follow system language** | Default. A tablet set to English shows the app in English; any other language falls back to Indonesian. |
| **Indonesian** | Always Indonesian, whatever the tablet's language. |
| **English** | Always English, whatever the tablet's language. |

The screen switches as soon as an option is tapped — there is no need to press **Save
Settings** and no need to close the app. The choice is saved and stays in effect after the
tablet is turned off.

![Home screen in English](img/tablet/43-beranda-bahasa-inggris.png)

> **Who can change it.** The language picker is inside the Settings screen, so only the
> **Owner and Manager** can open it. Cashier, Supervisor, and Kitchen use whichever language
> has been chosen. The choice applies to the whole tablet, not per staff member.

#### What stays in Indonesian

A few things deliberately do not switch:

| Stays Indonesian | Reason |
| --- | --- |
| Data you enter yourself: store name, product names, staff names, receipt footer | That is the content of your database, not app text. |
| Stock movement notes, e.g. "Selisih opname OPN-260907-0001" | An audit trail recorded once, when the event happens. If they were translated, old and new history would appear in different languages on the same screen. |
| Rupiah formatting: `Rp 25.000` | The currency is always Rupiah. Only the abbreviations follow the language: `rb`/`jt`/`M` become `K`/`M`/`B`. |

#### Matching terms

The screenshots in this guide show the Indonesian interface. Use this table to match what you
read here with what is on screen:

| English | Indonesian |
| --- | --- |
| Cashier | Kasir |
| Cart | Keranjang |
| Pay / Payment | Bayar / Pembayaran |
| Receipt | Struk |
| Transaction History | Riwayat Transaksi |
| Products / Categories | Produk / Kategori |
| Stock / Stock Count | Stok / Stok Opname |
| Stock Transfer | Transfer Stok |
| Purchasing (PO) | Pembelian (PO) |
| Suppliers | Pemasok |
| Customers / Member Tiers | Pelanggan / Tingkat Member |
| Promos / Vouchers | Promo / Voucher |
| Reports | Laporan |
| Shift & Cash | Shift & Kas |
| Staff / Attendance | Karyawan / Absensi |
| Table Management | Manajemen Meja |
| Kitchen Display | Layar Dapur |
| Settings | Pengaturan |
| Data Backup | Backup Data |
| Open Register | Buka Kasir |

---

## 2. Signing In and Out

### 2.1 Signing in

1. Type your PIN on the keypad (4–8 digits).
2. Press **Sign In**.

What happens automatically after a successful sign-in:

- You are **clocked in** — recorded in the Attendance menu.
- The active outlet follows the outlet assigned to your account.
- If you have Cashier rights and no shift is open, the app goes straight to the
  **Open Cashier Shift** screen. The Kitchen role skips this because it does not handle money.

### 2.2 PIN attempt limit

The sign-in screen deliberately does not say whether a wrong PIN exists or not, so it does not
help anyone guess accounts.

- **4 attempts** free. The remaining attempts are shown on screen.
- The 5th attempt onwards locks the screen: 15 seconds, then doubling with each failure,
  up to 15 minutes. The countdown runs on its own on screen.

### 2.3 Signing out

Tap the **sign-out** icon (↦) in the top-right corner of the home screen, then confirm. You are
automatically **clocked out**. A shift that is still open **stays saved** and can be continued
when you sign in again.

### 2.4 Switching outlets

The **store** icon (🏪) next to the sign-out icon opens the outlet list. Useful when one tablet
is used for more than one branch or warehouse.

---

## 3. Roles and Permissions

Permissions belong to the role, not to the person. Menus a role may not open **do not appear at
all** on the home screen — they are not just marked with a lock.

To see the details of a role's permissions: open **Staff**, then tap the role badge on the
staff member's row.

![Owner permissions](img/tablet/07-hak-akses-pemilik.png)

![Cashier permissions](img/tablet/08-hak-akses-kasir.png)

### 3.1 Permission matrix

| Feature | Owner | Manager | Supervisor | Cashier | Kitchen |
| --- | :-: | :-: | :-: | :-: | :-: |
| Cashier (selling) | ✅ | ✅ | ✅ | ✅ | — |
| Hold & Recall | ✅ | ✅ | ✅ | ✅ | — |
| Open Cash Drawer | ✅ | ✅ | ✅ | ✅ | — |
| Manage Customers | ✅ | ✅ | ✅ | ✅ | — |
| Kitchen Display | ✅ | ✅ | ✅ | ✅ | ✅ |
| Void Transaction | ✅ | ✅ | ✅ | — | — |
| Returns & Refunds | ✅ | ✅ | ✅ | — | — |
| Manual Discount | ✅ | ✅ | ✅ | — | — |
| Manage Stock | ✅ | ✅ | ✅ | — | — |
| Stock Count | ✅ | ✅ | ✅ | — | — |
| Manage Tables | ✅ | ✅ | ✅ | — | — |
| View Reports | ✅ | ✅ | ✅ | — | — |
| Manage Products | ✅ | ✅ | — | — | — |
| Stock Transfer | ✅ | ✅ | — | — | — |
| Purchasing & Suppliers | ✅ | ✅ | — | — | — |
| Manage Promos & Vouchers | ✅ | ✅ | — | — | — |
| Manage Staff | ✅ | ✅ | — | — | — |
| View Profit / COGS | ✅ | ✅ | — | — | — |
| Settings | ✅ | ✅ | — | — | — |
| Manage Outlets | ✅ | — | — | — | — |
| Backup & Restore | ✅ | — | — | — | — |

These restrictions are designed to prevent fraud: a cashier cannot change prices, give
themselves discounts, void transactions, or see profit.

### 3.2 Home screen by role

The difference in permissions is visible straight away from the number of menu cards on the
home screen.

**Owner** — 24 menus, including Outlets and Data Backup.

![Owner home screen](img/tablet/04-owner-beranda.png)

**Manager** — 22 menus; no Outlets and no Data Backup.

![Manager home screen](img/tablet/28-manajer-beranda.png)

**Supervisor** — 12 menus; the **Gross Profit** card is not shown.

![Supervisor home screen](img/tablet/20-supervisor-beranda.png)

**Cashier** — 5 menus; no Gross Profit and no Table Management.

![Cashier home screen](img/tablet/12-kasir-beranda.png)

**Kitchen** — 1 menu, no Open Register button.

![Kitchen home screen](img/tablet/36-dapur-beranda.png)

---

## 4. Role Guide: Cashier

Daily routine: open a shift → serve sales → close the shift and count the cash.

### 4.1 Opening a shift

After signing in, enter the **Opening Float (Float Cash)** — the cash actually in the drawer
before you start selling. There are quick buttons for 100K / 200K / 500K / 1000K.

![Opening a cashier shift](img/tablet/11-kasir-buka-shift.png)

This amount is used to calculate the cash difference when the shift is closed. Press
**Start Shift**.

> The *"Skip, I'm only viewing reports"* link is for when you sign in only to check data and
> will not be taking money.

### 4.2 Making a sale

Press the **Open Register** button at the bottom right of the home screen.

![Register screen](img/tablet/13-kasir-layar-jual.png)

Parts of the screen:

- **Left** — search box (name, SKU, or barcode), category tabs, and the product grid. The green
  number in the corner of a card is the remaining stock; a product without a number is not
  stock-tracked.
- **Right** — the cart, cost summary, and pay button.
- **Top** — 🧾 open bills, ⏸️ held carts, barcode scanner, and ⋮ transaction options.

Tap a product card to add it. Tap again to increase the quantity, or use the − / + buttons in
the cart.

![Filled cart](img/tablet/14-kasir-keranjang.png)

**Promos apply automatically.** The cashier does not need to enter any code — once the
conditions are met, the discount appears in the summary straight away, along with its name.
Service charge, tax, rounding, and customer points earned are calculated there too.

### 4.3 Transaction options (⋮ icon)

![Transaction options](img/tablet/24-kasir-opsi-transaksi.png)

| Option | Description |
| --- | --- |
| **Select Table** | Links the cart to a table (F&B mode). |
| **Save Order & Send to Kitchen** | The bill stays open until the customer pays; items join the kitchen queue. |
| **Hold Cart** | Saves the cart temporarily under a name; recall it later with the ⏸️ icon. |
| **Select Customer** | Links the transaction to a member so points are recorded. |
| **Cart Discount** | Only shown to Supervisor and above. |

### 4.4 Payment

Press **Pay Rp …**.

![Payment screen](img/tablet/15-kasir-pembayaran.png)

- **Cash** — type the amount or use the quick buttons, then **Add Cash Payment**.
- **Other Methods** — QRIS, Debit Card, Credit Card, GoPay, OVO, DANA, ShopeePay, Bank Transfer,
  Paylater, Member Balance.

One transaction can be paid with several methods at once (*split bill*). The remaining amount
is shown at the bottom and goes down each time a payment is added.

![Change calculated](img/tablet/16-kasir-kembalian.png)

Once it is covered, press **Complete Payment**.

### 4.5 Receipt

![Receipt](img/tablet/17-kasir-struk.png)

- **Send Digital Receipt** — WhatsApp, Email, SMS, or Share.
- **Print Receipt** — needs a Bluetooth printer already selected in *Settings → Printer*.
- **Open Drawer** — sends the open-drawer command to the printer.
- **New Transaction** — goes straight back to the register for the next customer.

### 4.6 Closing a shift

Open the **Shift & Cash** menu.

![Cashier shift](img/tablet/18-kasir-shift-kas.png)

This screen shows the shift duration, number of transactions, total sales, opening float,
**Expected Cash**, and a breakdown by payment method.

Press **Close Shift & Count Cash**, then enter the cash you physically counted in the drawer.

![Close shift dialog](img/tablet/19-kasir-tutup-shift.png)

The difference is calculated automatically. Fill in **Notes** if a difference needs explaining,
tick *Print shift report* if needed, then press **Close Shift**.

---

## 5. Role Guide: Kitchen

The Kitchen account has only one menu and cannot open the register or see sales figures other
than the summary cards.

### 5.1 Kitchen Display (KDS)

![Kitchen Display](img/tablet/37-dapur-kds.png)

Each card is one order: invoice number, table number (if any), time received, and **waiting
time** in the right-hand corner.

### 5.2 Changing item status

Tap an item row to advance its status: **Queued → Cooking → Served**.

![Status changed to Cooking](img/tablet/38-dapur-status.png)

The **Mark All Served** button completes every item in an order at once, and the card
disappears from the queue immediately.

---

## 6. Role Guide: Supervisor

The Supervisor has every Cashier capability, plus authority a cashier must not hold:
voiding transactions, processing returns, giving manual discounts, managing tables and stock,
and viewing reports (without profit).

### 6.1 Table management

![Table management](img/tablet/21-supervisor-meja.png)

Tables are grouped by area (Indoor, Outdoor, VIP) with four color-coded statuses:
🟢 Empty · 🔴 Occupied · 🟠 Reserved · 🔵 Billed.

Tap a table to open its actions.

![Table actions](img/tablet/22-supervisor-meja-aksi.png)

| Action | Description |
| --- | --- |
| **Create Order** | Opens the register already linked to that table. |
| **Reserve** | Marks the table as booked. |
| **Clear** | Returns the table to empty. |
| **Edit / Delete** | Changes the name, capacity, or area, or deletes the table. |

On a register linked to a table, the subtitle shows the table number. Note the **Discount**
button — it does not exist on the Cashier account.

![Register with a table](img/tablet/23-supervisor-kasir-meja.png)

After *Save Order & Send to Kitchen*, the table turns red and shows the running bill amount.

![Occupied table](img/tablet/25-meja-terisi.png)

### 6.2 Returns and refunds

Open **Transaction History**, choose a time range, then tap the transaction.

![Transaction history](img/tablet/39-supervisor-riwayat.png)

![Transaction details](img/tablet/40-supervisor-detail-transaksi.png)

Press **Return / Refund**.

![Return screen](img/tablet/41-supervisor-refund.png)

1. Set the quantity of each item being returned (or **Select All**).
2. **Return to stock** — turn it off if the goods are damaged and cannot be sold again.
3. Choose the **refund method**: Cash, Bank Transfer, QRIS, or Member Balance.
4. Fill in the **Return reason**, then press **Process Return**.

Stock, customer points, and financial reports adjust automatically.

The **Void** button on the details screen cancels the whole transaction, not a partial return.
The app asks for a void reason before processing it.

### 6.3 Stock count

**Stock Count** menu → **New Count** → enter a note (e.g. "month-end count") → **Start**.

![Stock count details](img/tablet/27-supervisor-opname-detail.png)

The app loads every stock-tracked product along with its system quantity. Fill in the
**Physical** column with the actual count. The *Show only differences* toggle makes it easier
to re-check items that do not match.

Press **Post Adjustment** to apply the corrections. Once posted, the count can no longer be
changed — so check it before pressing that button.

---

## 7. Role Guide: Manager

The Manager inherits every Supervisor capability, plus control over the catalog, prices,
purchasing, promos, staff, and store settings. The Manager can also see **Gross Profit and
COGS**.

### 7.1 Products and prices

![Product list](img/tablet/35-manajer-produk.png)

The list shows each variant with its SKU, category, price, and status labels
(*No stock*, *F&B*). A star marks favorite products that appear first on the register.

- **New Product** — adds a product with its variants, selling price, COGS, and barcode.
- **Categories** (top right) — sets category names, colors, and order.
- For F&B products, ingredient recipes are set from the product screen so ingredient stock is
  reduced automatically with every sale.

### 7.2 Purchasing (Purchase Order)

**Purchasing (PO)** → **New PO** → choose a supplier → **Create**.

Add items with the **+** button and enter the quantity and unit purchase price. The latest COGS
is shown for reference.

![Adding PO items](img/tablet/31-manajer-po-item.png)

![PO ready to send](img/tablet/32-manajer-po-siap.png)

PO status flow:

1. **Draft** — items can still be added, changed, or the PO cancelled.
2. **Send to Supplier** — the PO is locked and the button changes to *Receive Goods*.
3. **Receive Goods** — stock goes up and the product COGS is recalculated as a weighted average
   of the old stock and the newly received purchase price. Partial receipts are allowed; the PO
   stays *Partial* until the full quantity has arrived.

![PO awaiting receipt](img/tablet/33-manajer-po-terima.png)

### 7.3 Promos and vouchers

![Promo list](img/tablet/34-manajer-promo.png)

Promos apply **automatically** on the register when their conditions are met. Each promo has an
active/inactive toggle and labels describing its type, schedule, and running status.

Available promo types: Buy X Get Y Free, Percentage Discount (with a maximum cap), and Fixed
Amount Off (with a minimum spend). Code-based vouchers are managed on a separate screen via the
**Vouchers** link at the top right.

### 7.4 Staff

![Staff list](img/tablet/06-owner-karyawan.png)

- **New Staff** — enter the name, role, outlet, phone number, commission percentage, and PIN.
- Tap a staff row to edit their details, including **changing the PIN**.
- Tap the **role badge** to see that role's permissions in detail.
- The trash icon deactivates the staff member.

The *PIN saved* label means the PIN has been hashed. The app never shows a saved PIN to anyone —
if it is forgotten, the PIN has to be replaced with a new one.

Related menus: **Attendance** (clock-in/clock-out summary) and **Staff Commission** (commission
from sales).

### 7.5 Store settings

![Settings](img/tablet/09-owner-pengaturan.png)

Available settings groups:

| Group | Contents |
| --- | --- |
| **Store Identity** | Name, address, phone, invoice number prefix. The store name also appears on the sign-in screen and receipts. |
| **Tax & Charges** | Enable tax, tax name and percentage, prices include tax, service charge, rounding. |
| **Points Program** | Spend per 1 point, value of 1 point, minimum points to redeem. |
| **Business Mode** | Restaurant/F&B mode, Kitchen Display (KDS), low-stock warning. Turning off F&B mode hides the Table Management and Kitchen Display menus. |
| **Receipt** | Receipt footer, paper width (58 mm / 80 mm), auto-print after payment. |
| **Other** | Shortcuts to Printer & Cash Drawer, Outlets / Branches, Backup & Restore, and Create Sample Data. |
| **Language** | Interface language: follow system, Indonesian, or English. Takes effect immediately without pressing Save — see [App language](#14-app-language). |
| **Help** | **User Guide** — opens this documentation in the browser. The only part of the app that needs internet, and only for reading the guide. |
| **About** | App version and a note about offline mode. |

Changes to fields and toggles are only saved after pressing **Save Settings**.

> **Good to know.** The **Outlets** and **Data Backup** cards do not appear on the Manager's
> home screen, but both screens can still be opened via **Settings → Other**. Role restrictions
> in this app work by hiding menus, not by locking screens. If Backup and Outlets must truly be
> Owner-only, do not give anyone the Manager role.

---

## 8. Role Guide: Owner

The Owner has every permission without exception. The **Outlets** and **Data Backup** menus
only appear on the Owner's home screen (see the note under [Store settings](#75-store-settings)
about the shortcut through Settings).

### 8.1 Reports

![Reports](img/tablet/05-owner-laporan.png)

Choose a time range (Today, Yesterday, This Week, This Month, 30 Days, This Year), then choose a
tab:

| Tab | Contents |
| --- | --- |
| **Summary** | Net sales, average receipt, total discounts, returns, simple profit and loss, and daily sales trend. |
| **Products** | Best-selling products and their contribution. |
| **Payments** | Payment method breakdown. |
| **Time** | Sales spread by hour, for planning staff schedules. |
| **Customers** | Most active customers. |

The **Simple Profit & Loss** block breaks down gross sales → discounts → service charge → tax →
net sales → COGS → returns → **gross profit**. Operating expenses (rent, wages, electricity) are
not included. The share icon at the top right exports the report.

### 8.2 Outlets

The **Outlets** menu is used to add branches or warehouses. An outlet marked as a warehouse does
not appear as a place to sell, only as a stock transfer destination.

### 8.3 Backup and Restore

![Backup & Restore](img/tablet/10-owner-backup.png)

Because the app stores all data on the tablet, **backup is the only protection if the tablet is
lost, damaged, or stolen.**

- **Save Backup File** — produces a single file containing all products, stock, transactions,
  customers, and settings. Keep a copy on Google Drive or a memory card.
- **Choose Backup File** (Restore) — **overwrites all current data**. The app closes once the
  process finishes and needs to be opened again.

Recommendation: back up at the end of every day, and keep a copy off the tablet.

---

## 9. Troubleshooting

| Symptom | Cause and solution |
| --- | --- |
| The menu you want is not on the home screen | Your role does not have the permission. See the [permission matrix](#31-permission-matrix); ask the Owner or Manager to change your role in the Staff menu. |
| "Too many attempts" | Wrong PIN more than 4 times. Wait for the countdown to finish; the screen unlocks on its own. |
| "Shift not opened" banner on the home screen | Open the **Shift & Cash** menu, or sign out and back in to get the Open Shift screen. |
| "No printer selected" when printing a receipt | Pair the Bluetooth printer in Android, then select it in **Settings → Printer**. |
| Promo does not appear in the cart | Check the **Promos** menu: its toggle is on, its schedule runs today, and the minimum spend has been met. |
| Table Management and Kitchen Display menus are missing | F&B mode is turned off in **Settings → Business Mode**. |
| Stock does not match the physical goods | Run a **Stock Count**, enter the physical quantities, then Post Adjustment. |
| Orders do not appear on the Kitchen Display | Orders only join the queue via the **Save Order & Send to Kitchen** option, not via direct payment. |
| Staff member forgot their PIN | PINs cannot be viewed again. The Owner or Manager opens **Staff**, taps that staff member, and enters a new PIN. |
| App is in English but you want Indonesian | By default it follows the tablet's language. Choose **Settings → Language → Indonesian** to keep it Indonesian whatever the tablet's language. |
| The Language menu is missing | The language picker is inside the Settings screen, which only the Owner and Manager can open. Ask them. |
| APK file fails to install over the Google Play version ("app not installed" / package conflict) | The Play version and the APK version are signed with different keys, so one cannot replace the other. Update through Google Play only. If you really must switch channels, back up first, uninstall, install the other version, then restore the backup. |
| English is selected but product names are still Indonesian | Only the app's own text is translated. Product names, the store name, and the receipt footer are data you entered yourself — change them in their respective menus. |

---

## 10. What's New

This guide was first written for version 1.0.0. This section explains what has changed since
then and what you need to do. The running version can be seen in **Settings → About**.

| Version | Change | Action needed? |
| --- | --- | --- |
| **1.4.4** | **Help (?)** icon at the top right of the sign-in screen, linking to the English guide | No |
| **1.4.3** | **Help** menu in Settings, with a link to this guide | No |
| **1.4.2** | Fixes to shift cash and report return calculations | No — see [10.0](#100-shift-cash-and-return-calculations-142) |
| **1.4.1** | Internal fixes, no feature changes | No |
| **1.4.0** | Bilingual app: Indonesian and English | No — by default it follows the tablet's language |
| **1.3.1** | New app icon | No |
| **1.3.0** | Sign-in screen and sample data panel fixes | No |
| **1.2.0** | Android 16 adjustments, network permission removed | No |
| **1.1.0** | App identity changed | **Yes** — see [10.4](#104-moving-from-version-100) |

---

### 10.0 Shift cash and return calculations (1.4.2)

Two number fixes, no new features:

**Expected Cash no longer includes change.** Previously, the money handed over by the customer
was recorded in full — if a customer paid Rp 100,000 for a Rp 75,000 bill, Rp 100,000 went into
the cash calculation, even though Rp 25,000 went straight back out as change. As a result,
**Expected Cash** at shift close was too high and every shift appeared to be short. Change is
now subtracted, so the cash difference shows the real shortage or surplus. The per-method
breakdown in Shift & Cash and the payment breakdown in Reports are now correct as well.

**Full returns are no longer deducted twice.** A transaction whose items were all returned used
to be removed from sales *and* still have its return subtracted, so gross profit in Reports and
Expected Cash in the shift dropped by twice the return amount. Full returns are now treated the
same as partial returns: the sale stays recorded and the return is subtracted once.

These fixes also apply to existing data, so report figures for past periods may change (to the
correct values) after updating the app. There is nothing you need to do.

---

### 10.1 Indonesian and English (1.4.0)

The entire interface now has two languages. How to choose one, and the matching terms, are in
[App language](#14-app-language).

What to know specifically about printouts:

- **Customer receipts, kitchen tickets, and shift reports follow the active language.** If the
  tablet is set to English, receipts print with "TOTAL", "Change", "Cashier".
- **Receipts already printed do not change.** The language is chosen at print time, not when the
  transaction is created. Changing the language today does not change yesterday's receipts.
- **Product names on receipts stay exactly as you typed them.** If a product is named "Kopi
  Susu", that is what prints in English mode too.

If you serve foreign customers and want their receipt in English, just switch the language
before pressing Print, then switch it back afterwards — the change is instant and does not
disturb the transaction in progress.

---

### 10.2 New app icon (1.3.1)

The icon on the Android home screen changed from a cash register image to a green **POS**
emblem. Nothing needs to be done and nothing about how the app works has changed.

If the old icon is still showing after updating, the Android launcher is holding on to the old
image. Restart the tablet, or remove the home-screen shortcut and drag it out again from the app
drawer.

---

### 10.3 A more honest sign-in screen (1.3.0)

Three fixes, all automatic:

**PIN dots.** The sign-in screen used to draw only six dots even though a PIN may be up to eight
digits — the last two digits were typed with no feedback at all, so it felt like the buttons were
not working. The number of dots now follows the allowed PIN length.

**Sample data panel.** The **Create Sample Data** panel with its list of default PINs used to
stay on the sign-in screen after the first staff member was added — meaning PINs `1234` to
`9999` were still readable by anyone holding the tablet. The panel now disappears as soon as the
store is actually in use: there are products, transactions, customers, tables, promos, vouchers,
POs, or staff other than the default owner.

> **This does not replace changing the PIN.** Hiding the panel only hides the list;
> PIN `1234` stays valid until you change it in the **Staff** menu. Do that before the tablet is
> used for selling.

**The Create Sample Data menu in Settings** is also hidden on stores that are already in use.
The reason is not tidiness: running sample data **overwrites staff members 1 to 6 along with
their PINs**, so your real accounts would be wiped. If you do want to try features with sample
data, do it on another tablet or after a backup.

**The version on the About screen** is read directly from the app. The number was stuck at 1.0.0
for a while even though the app was much newer, so do not use old notes to guess the version —
open **Settings → About**.

---

### 10.4 Moving from version 1.0.0

This is the only change that **requires action from you.**

This section is only for those who installed version 1.0.0 from an APK file. If your app came
from Google Play, skip this section.

Since 1.1.0 the app identity changed from `com.dpos.kasir` to `id.dpos.kasir`. Android treats
them as **different apps**, so the new version does not replace the old one: both are installed
side by side, each with its own data, and the data does not move over on its own.

Symptoms: installing the new APK fails with `INSTALL_FAILED_UPDATE_INCOMPATIBLE`, or it installs
but the app is empty like a fresh install while the old icon is still in the app drawer.

**Steps to move your data — do them in order:**

1. **Open the old app** and sign in as Owner.
2. **Owner → Data Backup → Save Backup File.** Choose a destination **off the tablet** —
   Google Drive, or a memory card. Do not save it in the app's own folder; that folder is
   deleted along with the app when it is uninstalled.
3. **Make sure the file really exists** at the destination before continuing. Open the Files or
   Drive app and check that its size is not zero.
4. **Uninstall the old app.** Long-press its icon → Uninstall. This deletes all of its data —
   which is why step 3 must not be skipped.
5. **Install the new version** from Google Play or the APK file you received.
6. **Open the new app.** The sign-in screen will look like a fresh install. Sign in with the
   default PIN `1234`.
7. **Owner → Data Backup → Choose Backup File**, and point it to the file from step 2.
8. The app **closes itself** once the restore finishes. Open it again — all products, stock,
   transactions, customers, and settings are back.
9. Sign in with **your old PIN**, not `1234` anymore.

![Backup & Restore](img/tablet/10-owner-backup.png)

**Reassurances:**

- **Old PINs still work.** The way PINs are stored was tightened, and the app converts old PINs
  to the new format by itself the first time it opens after a restore. You do not need to reset
  anything.
- **The database structure did not change** between 1.0.0 and 1.4.2, so old backups are read in
  full — no transactions or stock are lost along the way.
- **The printer does not need to be selected again.** The printer choice is stored in the
  settings, so it comes back with the backup, and the Bluetooth pairing in Android is not touched
  at all. Still do a **Test Print** in **Settings → Printer** before selling.

> **If in doubt, do not uninstall yet.** As long as the old app is still installed, its data is
> safe. You can install the new version first, try it with empty data, and only move your data
> once you are confident. The two apps side by side do not interfere with each other.

---

### 10.5 Android 16 and scanner permission (1.2.0)

The app was adjusted for Android 16 and the **network access permission was removed**. The
barcode scanner uses a model built into the app, so that permission was never used.

This means that on the App Permissions screen, DPos Kasir no longer asks for internet access at
all — in keeping with the promise of an offline app. The only permissions still requested are
**Camera** (barcode scanning) and **Nearby devices / Bluetooth** (thermal printer). Both are only
requested the first time the feature is used, and can be denied if you do not use the scanner or
printer.
