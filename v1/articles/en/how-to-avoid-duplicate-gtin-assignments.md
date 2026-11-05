## How to Avoid Duplicate GTIN Assignments

Stop GS1 Assistant from assigning a GTIN you already used outside the app, and fix duplicates that already exist.

### Why duplicates happen

GS1 Assistant sees only the barcodes in your Shopify store. It does not know about a GTIN from your prefix that is used somewhere else, for example:

- GTINs you assigned before you installed GS1 Assistant, in a spreadsheet or in your GS1 portal
- GTINs used in another Shopify store or another sales system
- GTINs of products you deleted from Shopify. After you delete a product, the app can assign its GTIN again.

To prevent this, set where the app starts in your prefix, and give it a list of GTINs to skip.

### Before you start

- **Find the GTINs you already used.** Your GS1 portal can usually export a list of the GTINs issued from your prefix. If you are not sure, leave a bigger gap rather than risk reusing a number.

### Set where the app starts

The app assigns the next free number from **Start** up to **End** in your prefix's range. Set **Start** above the highest number you already used.

1. In the GS1 Assistant menu, click **Settings**.
2. In the **Prefixes** table, scroll right and click the pencil icon on the prefix's row.

![screenshot:The Prefixes table scrolled right. The pencil icon (2) on the row of prefix 5065023978 is outlined.](PrefixEditIcon.png)

3. In **Ranges**, type the **Start** and **End** numbers. **Minimum** and **Maximum** show the lowest and highest number your prefix allows.

![screenshot:The Ranges section with Start 51 and End 89 (3) outlined, and Minimum 0 and Maximum 99 below them.](PrefixRanges.png)

4. Click **Save** in the bar at the top of the page.

**Example:** your prefix allows 0 to 99, and you already used 0 to 36. Set **Start** to 37 and **End** to 99.

To keep a block of numbers back, add a second range with the plus icon. For example, the ranges 37 to 49 and 60 to 99 leave 50 to 59 unused.

### Skip GTINs you already used

If your used GTINs are spread across your prefix, import them as a list to skip.

1. In the GS1 Assistant menu, click **Settings**.
2. In the **Prefixes** table, scroll right and click the pencil icon on the prefix's row.
3. Under **Exclude**, click **Import GTINs to Exlude** and choose the file of used GTINs, for example the export from your GS1 portal.

![screenshot:The Exclude section with the Import GTINs to Exlude button (3) outlined.](DuplicatesExclude.png)

GS1 Assistant skips those GTINs from then on, even if no Shopify product uses them.

### Fix duplicates that already exist

The **Duplicate GTINs** tab in **GTIN Manager** lists every GTIN that more than one variant uses. Each GTIN is one row, for example "2 variants".

![screenshot:A Duplicate GTINs row with a red bar on the left: 2 variants, Duplicates, GTIN 05065023978496, GS1 UK.](StatusDuplicateRow.png)

1. Set **Start** or import an **Exclude** list first (see above), so the replacement GTINs do not collide again.
2. On the **Duplicate GTINs** tab, click **[number] variants** in the row to see which variants share the GTIN.
3. Decide which variant keeps the GTIN. If the GTIN is already on a marketplace listing or printed packaging, that product keeps it.
4. Click the **All** tab, search for each other variant's product, tick the variant, click **Unassign Barcode**, then click **Unassign 1 GTINs**.

![screenshot:The Unassign 1 GTINs? window with the Unassign 1 GTINs button outlined.](DuplicatesUnassignConfirm.png)

5. Click the **Needs GTIN** tab and assign new GTINs to those variants. See [Assign a GTIN to One Variant](https://gs1assistant.crisp.help/en/article/assign-your-first-gtin-to-a-product-1kpwezj/).
6. Click **Start Scan**. The GTIN leaves the **Duplicate GTINs** tab.

> **Warning:** Only remove a GTIN that was never published: not listed on a marketplace, not sent to GS1 and not printed on packaging. A published GTIN stays linked to its product.

### If you used GS1 Assistant before

If you used the app on another store, or before you reinstalled it, check the **History** section of your variants or your earlier import files to find the highest GTIN you assigned. Then set **Start** above it. If you cannot find your earlier data, click **Help** > **Chat with us** before you assign new GTINs.

### Troubleshooting

- **A new GTIN is already in use in your GS1 portal.** The app could not see that use. Import the used GTINs under **Exclude**, or raise **Start**, then replace the duplicate.
- **A deleted product's GTIN came back on a new product.** Raise **Start** above the highest GTIN you ever used.
- **The Duplicate GTINs count did not go down.** Click **Start Scan**.

### Related articles

- [Add and Manage Your Company Prefix](https://gs1assistant.crisp.help/en/article/adding-and-managing-your-company-prefix-6cxy7p/)
- [What the GTIN Status Counts and Tabs Mean](https://gs1assistant.crisp.help/en/article/understanding-gtin-status-what-ok-invalid-unassigned-and-verified-mean-cieak9/)
- [Assign GTINs to Many Variants at Once](https://gs1assistant.crisp.help/en/article/bulk-gtin-assignment-assign-barcodes-to-your-entire-catalogue-at-once-1vrtodi/)
