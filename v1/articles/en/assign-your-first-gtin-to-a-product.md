## Assign a GTIN to One Variant

Assign a GTIN from your company prefix to one product variant, check that it reached the variant, and remove it if you picked the wrong variant.

### Before you start

- **Your company prefix is added** under **Settings** > **Prefixes** and shows GTINs under **Remaining**. See [Add and Manage Your Company Prefix](https://gs1assistant.crisp.help/en/article/adding-and-managing-your-company-prefix-6cxy7p/).
- **Used GTINs from this prefix before?** Set where the app should start first, so it does not hand out a number that is already in use. See [How to Avoid Duplicate GTIN Assignments](https://gs1assistant.crisp.help/en/article/how-to-avoid-duplicate-gtin-assignments-6wuc5a/).

### Assign the GTIN

1. In the GS1 Assistant menu, click **GTIN Manager**.
2. Click the **Needs GTIN** tab. It lists every variant without a barcode. To find one product, type its name in the search box.
3. Tick the checkbox next to the variant.

![screenshot:GTIN Manager. The Needs GTIN tab (2) and the checkbox next to the first variant (3) are outlined.](QuickStartNeedsGTIN.png)

4. Click **Assign GTIN** in the bar above the list.

![screenshot:The bar above the list after selecting variants, with the Assign GTIN button (4) outlined.](QuickStartAssignBar.png)

5. In the **Select Company Prefix** window, check that your prefix is selected, then click **Assign**.

![screenshot:The Select Company Prefix window with prefix 5065023978, its Prefix Details, and the Assign button (5) outlined.](QuickStartSelectPrefix.png)

GS1 Assistant takes the next free GTIN from your prefix and writes it to the variant's barcode in Shopify. The row shows the new GTIN straight away, with a **Scan to Refresh** banner. The tab counts change after the next scan.

A row without a barcode also has an **Assign Barcode** button. It opens the same window for that one variant.

> **Tip:** Product not in the list? The **Status** filter shows active products by default. To see a draft product, set **Status** to **Draft** after you click the tab, because clicking a tab resets the filter.

### Check the result

1. Click **Start Scan**. When the scan finishes, the variant appears under **Valid GTINs** instead of **Needs GTIN**.
2. Click the eye icon at the end of the variant's row. The variant's page opens.

![screenshot:A variant row in GTIN Manager with the eye icon (2) at the end of the row outlined.](AssignOneEyeIcon.png)

The top of the page shows the barcode with a **Download Barcode** button. The **GTIN Status** section shows the **GTIN**, the **Company Prefix** it came from, the **Member Organization** and the **Company**.

![screenshot:A variant page with GTIN 05065023978496. The barcode and Download Barcode button sit at the top, and the GTIN Status section below is outlined.](AssignOneVariantPage.png)

At the bottom of the page, **History** lists the assignment, for example "User Assigned GTIN 05065023978496 to barcode".

![screenshot:The History section of a variant page with one row: User Assigned GTIN 05065023978496 to barcode.](AssignOneHistory.png)

### What the variant page shows

| Section | What it contains |
|---|---|
| **GTIN Status** | GTIN, Member Organization, Company Prefix and Company. The button reads **Assign GTIN** when the variant has no GTIN, and **Unassign Barcode** when it has one. |
| **Verified by GS1** | Product description, Brand name, Global product category, Countries of sale and Net content. |
| **GTIN Manager** | Product details: Category, Target Market, Brand Name, Product Name, Net quantity, Unit of measure, Consumer Unit and Packaging Level, saved with **Update**. You do not need to fill these in to assign a GTIN. |
| **Optional Properties** | Color, Size, Net Weight, Width, Height, Depth and their units. |
| **History** | Each GTIN change with its date and time. A variant with no changes shows "No GTIN History found". |

### Remove a GTIN you assigned by mistake

> **Warning:** Only remove a GTIN that was never published: not listed on a marketplace, not sent to GS1 and not printed on packaging. A published GTIN stays linked to its product. Reusing it on a different product can cause listing errors.

1. In **GTIN Manager**, click the **Valid GTINs** tab and tick the checkbox next to the variant.
2. Click **Unassign Barcode** in the bar above the list.

![screenshot:The bar above the list with the Unassign Barcode button (2) outlined.](AssignOneUnassignBar.png)

3. In the **Unassign 1 GTINs?** window, click **Unassign 1 GTINs**.

![screenshot:The Unassign 1 GTINs? window. The text reads: This removes the GTIN from these 1 variants. The Unassign 1 GTINs button (3) is outlined.](AssignOneUnassignConfirm.png)

The GTIN is removed from the variant. Removing it does not add the number back to your free GTINs. To use that number again, click **Help** > **Chat with us** and ask support to reset your prefix's range.

### Troubleshooting

- **The variant is not under Needs GTIN.** It already has a barcode value. Look under **Valid GTINs** or **Not a GTIN**. To replace a value, see [Assign GTINs to Many Variants at Once](https://gs1assistant.crisp.help/en/article/bulk-gtin-assignment-assign-barcodes-to-your-entire-catalogue-at-once-1vrtodi/).
- **The counts did not change after you assigned.** Click **Start Scan**.
- **Assign is greyed out in the Select Company Prefix window.** Choose a prefix in **Company Prefix** first.
- **The prefix has no free GTINs.** Check **Remaining** under **Settings** > **Prefixes**, then add another prefix.

### Related articles

- [Set Up GS1 Assistant: Quick Start](https://gs1assistant.crisp.help/en/article/how-to-install-connect-and-add-your-prefix-17v6vte/)
- [Assign GTINs to Many Variants at Once](https://gs1assistant.crisp.help/en/article/bulk-gtin-assignment-assign-barcodes-to-your-entire-catalogue-at-once-1vrtodi/)
- [What the GTIN Status Counts and Tabs Mean](https://gs1assistant.crisp.help/en/article/understanding-gtin-status-what-ok-invalid-unassigned-and-verified-mean-cieak9/)
