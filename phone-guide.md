# DPos Kasir User Guide — Android Phone

**English** · [Bahasa Indonesia](panduan-ponsel.md)

This guide is the **phone** version of the [Tablet Guide](tablet-guide.md). Both cover every
role — **Owner, Manager, Supervisor, Cashier, and Kitchen** — but all the screenshots here were
taken directly on a phone in **portrait** orientation, and each section highlights what is
**different from the tablet**.

Test device: **Samsung Galaxy S20+ (SCV45), Android 12, 1440 × 3040 screen (411 dp)**.
Screenshots were taken from DPos Kasir 1.0.0 with the Indonesian interface; the layout has not
changed up to 1.4.3. Features added since then — the language picker, sign-in screen fixes,
cash calculation fixes — are described in the
[Tablet Guide, What's New section](tablet-guide.md#10-whats-new). For the matching English and
Indonesian terms on screen, see [App language](tablet-guide.md#14-app-language).

DPos Kasir works entirely **offline** — there is no server and no internet is needed. All data
is stored on the phone, so regular backups are the owner's responsibility.

---

## Contents

1. [Installing on a Phone](#1-installing-on-a-phone)
2. [What Is Different from the Tablet](#2-what-is-different-from-the-tablet)
3. [Signing In and Out](#3-signing-in-and-out)
4. [Role Guide: Cashier](#4-role-guide-cashier)
5. [Role Guide: Kitchen](#5-role-guide-kitchen)
6. [Role Guide: Supervisor](#6-role-guide-supervisor)
7. [Role Guide: Manager](#7-role-guide-manager)
8. [Role Guide: Owner](#8-role-guide-owner)
9. [Bluetooth Thermal Printer](#9-bluetooth-thermal-printer)
10. [Phone-Specific Tips](#10-phone-specific-tips)

---

## 1. Installing on a Phone

### 1.1 Installing the app

Minimum requirement: **Android 7.0** or later.

**From Google Play** — the recommended way. Updates arrive automatically through the Play Store.

**From an APK file** — if you received an APK file directly from the developer:

| File | Used for |
| --- | --- |
| `…-arm64-v8a.apk` | Almost every phone made in 2017 or later (64-bit). **The main choice.** |
| `…-armeabi-v7a.apk` | Older 32-bit phones. |
| `…-universal.apk` | When in doubt — the largest file, but it runs on everything. |

How to install an APK file:

1. Copy the APK file to the phone (USB cable, memory card, or send it to yourself via chat).
2. Open the file with the **Files** app.
3. Android will block the install and offer **"Allow from this source"** — turn it on,
   then go back and choose **Install**.
4. The "app not scanned by Play Protect" warning is normal for apps from outside the Play Store.
   Choose **Install anyway**.

> **Do not mix channels.** The Google Play version and the APK version are signed with
> different keys, so an APK file cannot update an app installed from Play, and vice versa. If
> you need to switch channels, **back up first**, uninstall the app, install the other version,
> then restore the backup (see [Backup and restore](#83-backup-and-restore)).

### 1.2 First launch

When opened for the first time the database is still empty. The sign-in screen shows a
**"No product data yet"** panel with a *Create Sample Data* button.

![Sign-in screen on a fresh install](img/ponsel/01-login-baru.png)

| Option | When to use it |
| --- | --- |
| **Create Sample Data** | For learning or demos. Fills in products, customers, promos, tables, and sales history. |
| Sign in directly with PIN `1234` | For a real store. Start from scratch and enter your own products and staff. |

Once data has been entered, the sign-in screen goes back to being clean — just the keypad, with
the store name above it.

![Normal sign-in screen](img/ponsel/02-login-normal.png)

> **Important.** On a narrow phone screen, the sample PIN list sits below the
> *Create Sample Data* button and you need to scroll to see it. The panel disappears on its own
> once the first product is saved. Change every default PIN in the **Staff** menu before the
> phone is used for selling.

### 1.3 Sample PINs (demo data only)

| PIN | Name | Role | Outlet |
| --- | --- | --- | --- |
| `1234` | Budi Santoso | Owner | Kopi Nusantara — Pusat |
| `2345` | Siti Rahayu | Manager | Kopi Nusantara — Pusat |
| `3456` | Andi Pratama | Supervisor | Kopi Nusantara — Pusat |
| `4567` | Dewi Lestari | Cashier | Kopi Nusantara — Pusat |
| `5678` | Rizky Maulana | Cashier | Cabang Bandung |
| `9999` | Dapur | Kitchen | Kopi Nusantara — Pusat |

---

## 2. What Is Different from the Tablet

The app switches layout automatically at a **screen width threshold of 720 dp**. A phone in
portrait (±411 dp) is below that threshold, so:

| Area | Tablet (≥ 720 dp) | Phone, portrait (< 720 dp) |
| --- | --- | --- |
| Register screen | Catalog and cart side by side | Catalog fills the screen, the cart becomes a **slide-up panel** |
| Order total | Always visible in the right panel | In the **bottom bar**: item count, total, *Cart* and *Pay* buttons |
| Home summary cards | 3 columns | **2 columns** |
| Home menu | Fits on one screen | Needs **scrolling** down |
| Register product grid | 4–5 columns | **3 columns** |
| Table grid | 4–6 columns | **3 columns** |

Every function is still there — no features are missing on the phone, only the arrangement
stacks downward.

### 2.1 Turning the phone to landscape

A phone in **landscape** orientation passes the 720 dp threshold, so the display switches to
the tablet layout — the cart appears as a fixed panel on the right.

![Register screen on a phone in landscape](img/ponsel/46-kasir-mendatar.png)

Useful during rush hour. The downside: little screen height is left, so the visible product
list is shorter. Make sure the phone's **auto-rotate** is on if you want to use this.

---

## 3. Signing In and Out

### 3.1 Signing in

Tap your PIN on the keypad and press **Sign In**. The app takes you straight to the home screen
for your role. Cashiers and other roles are asked about **opening a shift** first.

### 3.2 PIN attempt limit

The sign-in screen deliberately does not say whether a wrong PIN exists or not.

- **4 attempts** free. The remaining attempts are shown on screen.

  ![Remaining PIN attempts](img/ponsel/44-login-sisa-percobaan.png)

- The 5th attempt onwards locks the screen: 15 seconds, then doubling with each failure,
  up to 15 minutes. The countdown runs on its own.

  ![Sign-in screen locked](img/ponsel/45-login-terkunci.png)

### 3.3 Signing out

Tap the **sign-out** icon (↦) in the top-right corner of the home screen, then confirm. You are
automatically **clocked out**. A shift that is still open **stays saved** and can be continued
when you sign in again.

![Sign-out confirmation](img/ponsel/13-keluar-aplikasi.png)

### 3.4 Switching outlets

The **store** icon (🏪) next to the sign-out icon opens the outlet list.

![Choose outlet](img/ponsel/43-pindah-outlet.png)

---

## 4. Role Guide: Cashier

### 4.1 Opening a shift

After signing in, the cashier is asked to record the cash in the drawer as the **opening float
(float cash)**. This amount is used to calculate the cash difference when the shift is closed.
Shortcuts are available: *100K / 200K / 500K / 1000K*.

![Opening a cashier shift](img/ponsel/03-kasir-buka-shift.png)

The **"Skip, I'm only viewing reports"** link is for when you only want to look at data without
selling.

### 4.2 Cashier home screen

Summary cards are laid out in **two columns**, the menu is below them, and a large **Open
Register** button floats in the bottom-right corner.

![Cashier home screen](img/ponsel/04-kasir-beranda.png)

### 4.3 Sales screen

Products are shown in **three columns**. At the top are the search box (name, SKU, barcode) and
a category row you can swipe sideways. Icons in the header: 🧾 open bills, ⏸️ held transactions,
barcode scanner, and ⋮ more options.

![Sales screen](img/ponsel/05-kasir-layar-jual.png)

Tap a product to add it to the cart. The **bottom bar** immediately updates the item count and
total — this replaces the tablet's cart panel.

![Bottom bar after adding an item](img/ponsel/06-kasir-bar-bawah.png)

### 4.4 Cart

Tap **Cart** in the bottom bar to open the slide-up panel. Drag its handle up so the panel fills
the screen — there you can see the item details, promos applied automatically, service charge,
tax, rounding, and customer points.

![Cart panel](img/ponsel/07-kasir-keranjang.png)

- The **−** and **+** buttons change the quantity; the ⋮ icon on each row adds a note or item
  discount.
- **Select Customer** at the top right of the panel attaches a member.
- **Voucher** to enter a code; **Clear** to cancel the whole cart.

### 4.5 Payment

Press **Pay** to open the payment screen: the bill summary at the top, cash in the middle
(with quick amount shortcuts), and **Other Methods** — QRIS, debit card, credit card, and so on —
below.

![Payment screen](img/ponsel/08-kasir-pembayaran.png)

Enter the amount, press **Add Cash Payment**, and the change appears in the bottom bar. Payments
can be combined (for example, part cash and the rest by QRIS).

![Change calculated](img/ponsel/09-kasir-kembalian.png)

Press **Complete Payment** to close the transaction.

### 4.6 Receipt

The receipt screen offers three choices: send a digital receipt (WhatsApp, Email, SMS, Share),
print to a thermal printer, and preview the receipt. The **New Transaction** button opens an
empty cart straight away.

![Receipt screen](img/ponsel/10-kasir-struk.png)

> If a *"No printer selected"* warning appears, set it up first in
> [Settings → Printer](#9-bluetooth-thermal-printer).

### 4.7 Shift and cash

The **Shift & Cash** menu shows the current shift: opening time, duration, number of
transactions, total sales, opening float, and **expected cash**.

![Cashier shift](img/ponsel/11-kasir-shift-kas.png)

### 4.8 Closing a shift

Press **Close Shift & Count Cash** and enter the cash actually counted in the drawer. The app
calculates the **difference** immediately. A note is optional, and the shift report can be
printed straight away.

![Close shift dialog](img/ponsel/12-kasir-tutup-shift.png)

---

## 5. Role Guide: Kitchen

The Kitchen role has only one menu: **Kitchen Display**. Well suited to a second phone placed
in the cooking area.

![Kitchen home screen](img/ponsel/14-dapur-beranda.png)

### 5.1 Kitchen Display

Each order appears as a card with the invoice number, waiting time, and the list of items with
their status.

![Kitchen Display](img/ponsel/15-dapur-layar.png)

### 5.2 Changing item status

Tap the status badge on an item row to cycle it: **Queued → Cooking → Served**.
The **Mark All Served** button completes a whole card at once.

![Item status changed to Cooking](img/ponsel/16-dapur-status.png)

> If the kitchen uses a **Bluetooth ticket printer** instead of a screen, set up the kitchen
> printer in [Settings → Printer](#9-bluetooth-thermal-printer). The Kitchen Display can stay on
> as a backup.

---

## 6. Role Guide: Supervisor

The Supervisor home screen adds Table Management, Stock, Ingredients, and Stock Count. If no
shift has been opened, an orange warning banner appears.

![Supervisor home screen](img/ponsel/17-supervisor-beranda.png)

### 6.1 Table management

Tables are grouped by area (Indoor, Outdoor, VIP) with status colors: green empty, red
occupied, orange reserved, blue billed. On a phone the grid has **three columns**.

![Table management](img/ponsel/18-supervisor-meja.png)

Tap a table to open the action panel: **Create Order**, *Reserve*, *Clear*, *Edit*,
and *Delete*.

![Table actions](img/ponsel/19-supervisor-meja-aksi.png)

### 6.2 Returns and refunds

Open **Transaction History**, filter by period or search for an invoice number.

![Transaction history](img/ponsel/21-supervisor-riwayat.png)

Tap a transaction to see its details. At the bottom of the screen are **Return / Refund** and
**Void**.

![Transaction details](img/ponsel/22-supervisor-detail-transaksi.png)

On the return screen, set the quantity of each item being returned, whether the goods are
**returned to stock**, and the refund method. Stock, points, and financial reports adjust
automatically.

![Returns and refunds](img/ponsel/23-supervisor-retur.png)

### 6.3 Stock count

**Stock Count → New Count** creates a draft containing every stock-tracked product. Fill in the
**Physical** column with the counted amounts; the *Show only differences* toggle speeds up the
check. Press **Post Adjustment** to apply it.

![Stock count](img/ponsel/20-supervisor-opname.png)

---

## 7. Role Guide: Manager

The Manager home screen adds the **Gross Profit** card and a much longer menu — on a phone this
menu needs scrolling.

![Manager home screen](img/ponsel/24-manajer-beranda.png)

![Manager menu after scrolling](img/ponsel/25-manajer-menu-lanjutan.png)

### 7.1 Products and prices

The product list includes SKU, category, price, stock indicator, and a star for favorite
products that appear first on the register.

![Product list](img/ponsel/26-manajer-produk.png)

### 7.2 Purchasing (Purchase Order)

The flow has four steps:

1. **New PO** → choose a supplier, add a note, press *Create*.

   ![New PO dialog](img/ponsel/27-manajer-po.png)
2. Add items with the **+** button and enter the quantity and unit purchase price.

   ![Adding PO items](img/ponsel/28-manajer-po-tambah-item.png)

3. Once all items are in, press **Send to Supplier**.

   ![PO ready to send](img/ponsel/29-manajer-po-siap.png)

   The PO status changes to awaiting goods, and the button changes to *Receive Goods*.

   ![PO awaiting delivery](img/ponsel/30-manajer-po-terima.png)

4. When the goods arrive, press **Receive Goods** and enter the quantity actually received.
   Stock goes up and **COGS is updated using a moving average**.

   ![Receiving goods](img/ponsel/31-manajer-po-diterima.png)

Partial receipts are allowed — the remainder stays recorded as outstanding.

### 7.3 Promos and vouchers

Active promos apply **automatically** on the register when their conditions are met; the cashier
does not need to enter any code. Code-based vouchers are managed on a separate tab at the top
right.

![Promo list](img/ponsel/32-manajer-promo.png)

### 7.4 Staff and permissions

Each staff member has a PIN stored as a **hash** — an old PIN cannot be read back, only
replaced.

![Staff list](img/ponsel/33-manajer-karyawan.png)

Tap the role badge to see the details of the features that role can open.

![Cashier permissions](img/ponsel/34-hak-akses.png)

### 7.5 Store settings

Store identity (name, address, phone, invoice number prefix), tax, service charge, business
mode, and receipt format are all on one scrolling screen. The **Save Settings** button sticks
to the bottom.

![Store settings](img/ponsel/35-manajer-pengaturan.png)

![Business mode and receipt](img/ponsel/36-pengaturan-printer.png)

For phone receipts, **58 mm (32 columns)** is the most common pocket printer size;
80 mm is used by desktop printers.

---

## 8. Role Guide: Owner

The Owner has every Manager menu plus **Outlets** and **Data Backup**.

![Owner home screen](img/ponsel/38-pemilik-beranda.png)

![Full Owner menu](img/ponsel/39-pemilik-menu.png)

### 8.1 Reports

Reports have a period filter (Today, Yesterday, This Week, This Month, 30 days) and four tabs:
**Summary, Products, Payments, Time**. On a phone, the tabs and periods are swiped sideways.
The share icon at the top right exports the summary as text.

![Reports](img/ponsel/40-pemilik-laporan.png)

Gross profit is calculated as net sales − tax − COGS − returns. Operating expenses (rent, wages,
electricity) are **not** included.

### 8.2 Outlets

Each outlet has its own stock. Goods are moved between outlets via **Stock Transfer**, not by
editing stock directly.

![Outlet list](img/ponsel/42-pemilik-outlet.png)

### 8.3 Backup and restore

Because all data exists only on the phone, **backup is the only safeguard** if the phone is
lost, damaged, or stolen.

![Backup and restore](img/ponsel/41-pemilik-backup.png)

- **Save Backup File** produces a single file containing products, stock, transactions,
  customers, and settings. Keep a copy on Google Drive or a memory card.
- **Choose Backup File** restores the data and **overwrites all current data**.
  The app closes itself once the process finishes and needs to be opened again.

> Phones are far easier to lose than a register tablet. Make a habit of backing up every time
> the store closes.

---

## 9. Bluetooth Thermal Printer

This is the most frequently used section in phone-based setups, because a Bluetooth pocket
printer is the natural partner for a mobile cashier.

The steps:

1. **Pair the printer first through Android's built-in Bluetooth Settings** — not from inside
   the app. The app only reads the list of devices that are already paired.
2. Open **Settings → Printer & Cash Drawer** in DPos Kasir.
3. Press **Grant Bluetooth Permission** and approve Android's permission request.
4. Choose the printer from **Paired Devices**. The *For receipts* button sets whether that device
   is used for cashier receipts or kitchen tickets.
5. Test it with **Test Print**, and **Open Drawer** if a cash drawer is connected to the printer.

![Printer and cash drawer](img/ponsel/37-printer-bluetooth.png)

Notes:

- **USB or LAN** printers are not supported directly; use the printer's own app.
- The **kitchen printer** can be left on *Same as receipt printer* if there is only one printer.
- The **Auto-print after payment** toggle in the *Receipt* section saves one tap on every
  transaction.

---

## 10. Phone-Specific Tips

| Situation | Advice |
| --- | --- |
| Screen turns off while serving a queue | Set Android's *Screen timeout* to 5 minutes or more, or turn on "stay awake while charging" in Developer Options. |
| Rush hour, you want to see the cart all the time | Turn the phone to landscape — the layout changes to two columns like the tablet. |
| Bottom buttons are covered by the navigation bar | Drag the cart panel all the way up; the *Pay* button moves up into the safe area. |
| The phone is shared between shifts | Always **Sign Out** (not just lock the screen) so attendance and shifts are recorded against the right person. |
| Battery critical mid-shift | Transaction data is saved as soon as payment is completed; a sudden shutdown does not lose receipts that have been paid, but an unpaid cart will be lost. |
| Phone lost or stolen | There is no server, so data cannot be wiped remotely. Recovery is only possible from the latest backup file — make sure you back up regularly. |

### Common problems

| Symptom | Cause and fix |
| --- | --- |
| "App cannot be installed" | The APK does not match the processor — use the `universal` variant. Or the same app is already installed from Google Play; see [Do not mix channels](#11-installing-the-app). |
| Sign-in screen locked | Too many wrong PINs. Wait for the countdown to finish; the duration doubles up to 15 minutes. |
| Printer does not appear in the list | It has not been paired in Android's Bluetooth Settings, or Bluetooth permission has not been granted in the app. |
| Printed receipt is cut off | Wrong paper width. Change it in **Settings → Receipt → Paper width**. |
| The menu you want is not visible | The phone home screen is longer than the tablet's — scroll down. |
| Cash difference is always negative | The opening float was entered higher than the cash actually in the drawer when the shift was opened. |
