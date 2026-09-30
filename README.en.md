# DPos Kasir Documentation

**English** · [Bahasa Indonesia](README.md)

User guide for **DPos Kasir**, an Android cashier (point of sale) app for shops, cafés, and
restaurants. Applies to version **1.4.3**.

From inside the app, this guide can be opened via **Settings → Help → User Guide**.

![Owner home screen on a tablet](img/tablet/04-owner-beranda.png)

## Choose a guide

| Guide | For |
| --- | --- |
| **[Tablet Guide](tablet-guide.md)** | Android tablets in landscape. The main guide: every role, the permission matrix, language settings, troubleshooting, and release notes for each version. |
| **[Phone Guide](phone-guide.md)** | Android phones in portrait. Same content as the tablet version, plus installation, layout differences on narrow screens, Bluetooth pocket printers, and phone-specific tips. |

The screenshots show the app's Indonesian interface. The app itself is also available in
English — see [App language](tablet-guide.md#14-app-language) for the matching terms.

## The app at a glance

- **Fully offline.** No server and no internet needed. All data — products, stock,
  transactions, customers, reports — is stored on the device. That is why **regular backups are
  the store owner's responsibility**.
- **Five roles** with different permissions: Owner, Manager, Supervisor, Cashier, and Kitchen.
  Menus a role may not open do not appear at all.
- **Bilingual**: Indonesian and English, including receipts and kitchen tickets.
- **Device requirements**: Android 7.0 or later. The camera is used for barcode scanning;
  Bluetooth for thermal receipt and kitchen ticket printers (58 mm or 80 mm) and the cash drawer.

## Quick start

1. Open the app. On first install, tap **Create Sample Data** if you want to try every feature
   with demo data, or sign in directly with PIN **`1234`** (Owner) for a real store.
2. Fill in **Settings → Store Identity**, tax, and service charge.
3. Add products in the **Products** menu, then staff in the **Staff** menu.
4. **Change the default PIN `1234`** before the device is used for selling.
5. Pair the Bluetooth printer in Android, then select it in **Settings → Printer & Cash Drawer**.
6. The cashier signs in, opens a shift with an opening float, and starts selling.

The full steps are in the [Tablet Guide](tablet-guide.md#1-getting-started).

## Daily flow in brief

| Role | What they do | Guide |
| --- | --- | --- |
| Cashier | Open shift → sell → pay → print receipt → close shift & count cash | [Cashier](tablet-guide.md#4-role-guide-cashier) |
| Kitchen | Watch the Kitchen Display, move items Queued → Cooking → Served | [Kitchen](tablet-guide.md#5-role-guide-kitchen) |
| Supervisor | Manage tables, process returns & voids, stock counts | [Supervisor](tablet-guide.md#6-role-guide-supervisor) |
| Manager | Products & prices, purchasing (PO), promos, staff, settings | [Manager](tablet-guide.md#7-role-guide-manager) |
| Owner | Reports & profit, outlets, **backup & restore** | [Owner](tablet-guide.md#8-role-guide-owner) |

## Having trouble?

See [Troubleshooting](tablet-guide.md#9-troubleshooting) in the tablet guide and
[Phone-Specific Tips](phone-guide.md#10-phone-specific-tips) in the phone guide.
