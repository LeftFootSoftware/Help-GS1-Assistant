## Assign GTINs to Many Variants at Once

Bulk Assign gives every variant you select the next free GTIN from your company prefix and writes it to that variant's barcode in Shopify.

### Before you start

- **A company prefix in the app.** It appears under **Settings** > **Prefixes**. To add one, see [Adding and Managing Your Company Prefix](https://gs1assistant.crisp.help/en/article/adding-and-managing-your-company-prefix-6cxy7p/).
- **Enough free GTINs.** The **Remaining** column shows how many GTINs the prefix has left. Each variant uses one.
- **The right starting point.** If you used GTINs from this prefix before (by hand, in a spreadsheet, in another store or in another system), set the **Start** of the prefix's range past those numbers first. Otherwise the app can assign a GTIN that is already in use. See [How to Avoid Duplicate GTIN Assignments](https://gs1assistant.crisp.help/en/article/how-to-avoid-duplicate-gtin-assignments-6wuc5a/).

![screenshot:Settings, Prefixes table. The Remaining column for prefix 5065023978 is outlined and shows 39.](BulkPrefixRemaining.png)

> **Bulk Assign only fills empty barcodes.** It skips every variant that already has a barcode value, whether the value is valid or not. To replace existing barcodes, see **Replace barcodes a variant already has** below.

### Assign GTINs to every variant that needs one

1. In the GS1 Assistant menu, click **GTIN Manager**.
2. Click the **Needs GTIN** tab. The list now shows only variants with no barcode.

![screenshot:GTIN Manager tabs. The Needs GTIN tab is outlined and numbered 2.](BulkNeedsGTINTab.png)

3. Optional: narrow the list. Type a product name in **Search and filter**, or click **Add filter** and choose **Collection** or **Company Prefix**. The **Status** filter shows active products by default. To include draft products, change **Status** to **Draft**.
4. Tick the checkbox at the top of the list. This selects the variants on the current page.
5. Click **Select all [number]+ variants**. This extends the selection to every variant in the list, on every page.
6. Click **Assign GTIN**.

![screenshot:The bar above the list after selecting. The top checkbox (4), the Select all 2+ variants link (5) and the Assign GTIN button (6) are outlined.](BulkSelectAllAssign.png)

7. In the **Select Company Prefix** window, check that the right prefix is selected, then click **Assign**.

![screenshot:The Select Company Prefix window with prefix 5065023978, its Prefix Details (Remaining 41, GS1 UK, Block Size 100) and the Assign button outlined (7).](BulkSelectCompanyPrefix.png)

> **Important:** If you skip step 5, only the variants on the current page get GTINs. Moving to another page clears the selection.

### What happens next

GS1 Assistant takes the next free GTINs from the prefix, one per variant, and writes each one to the variant's barcode in Shopify. Click **Start Scan** to update the counts. The variants then appear under **Valid GTINs** with their new number in the **GTIN** column.

Shopify limits how fast apps can update products, so a large catalog takes time. On one large store, assignment ran at about 2,000 variants an hour. Do not click **Assign GTIN** again while a run is in progress.

If the prefix runs out of GTINs, assignment stops. The variants that did not get one stay under **Needs GTIN**.

### Replace barcodes a variant already has

Bulk Assign never overwrites a barcode. To replace barcodes, for example values listed under **Not a GTIN**, remove them first:

1. In **GTIN Manager**, click the tab that lists the variants, such as **Not a GTIN** or **Duplicate GTINs**.
2. Tick the variants to change. To select the whole list, tick the top checkbox, then click **Select all [number]+ variants**.
3. Click **Unassign Barcode**.
4. Click the **Needs GTIN** tab and follow the steps above.

> **Warning:** Only remove a GTIN that was never published: not listed on a marketplace, not sent to GS1 and not printed on packaging. A published GTIN stays linked to its product. Reusing it on a different product can cause listing errors.

### Assign GTINs to new products automatically

Bulk Assign covers the products you have today. To give new variants a GTIN as they are created, use Auto Assign. Auto Assign runs through Shopify Flow and needs the **Automation** plan. See [Using Shopify Flow to Assign GTINs to New Products](https://gs1assistant.crisp.help/en/article/using-shopify-flow-to-assign-gtins-to-new-products-1qol6ru/).

### Troubleshooting

- **Only some of the selected variants got a GTIN.** The selection covered one page only. Repeat the steps and click **Select all [number]+ variants** (step 5).
- **Some variants were skipped.** They already had a barcode value. Look for them under **Not a GTIN** or **Valid GTINs**. To replace the values, see **Replace barcodes a variant already has** above.
- **The counts did not change.** Click **Start Scan**. The counts do not update by themselves after a run or after a Shopify Flow assignment.
- **Assignment stopped before the end.** The prefix has no free GTINs left. Check **Remaining** under **Settings** > **Prefixes**, then add another prefix.
- **A new GTIN is already used somewhere else.** The prefix's range started too low. Follow [How to Avoid Duplicate GTIN Assignments](https://gs1assistant.crisp.help/en/article/how-to-avoid-duplicate-gtin-assignments-6wuc5a/).

### Related articles

- [Assign Your First GTIN to a Product](https://gs1assistant.crisp.help/en/article/assign-your-first-gtin-to-a-product-1kpwezj/)
- [How to Avoid Duplicate GTIN Assignments](https://gs1assistant.crisp.help/en/article/how-to-avoid-duplicate-gtin-assignments-6wuc5a/)
- [Understanding GTIN Status](https://gs1assistant.crisp.help/en/article/understanding-gtin-status-what-ok-invalid-unassigned-and-verified-mean-cieak9/)
- [Using Shopify Flow to Assign GTINs to New Products](https://gs1assistant.crisp.help/en/article/using-shopify-flow-to-assign-gtins-to-new-products-1qol6ru/)
