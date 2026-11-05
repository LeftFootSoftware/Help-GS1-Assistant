## Why Do My GTIN Counts Look Wrong?

Find out why a count in GS1 Assistant differs from what you expect, and how to correct it. Most differences come from how each count is calculated, not from lost GTINs.

### The counts GS1 Assistant shows

| Count | Where | What it counts |
|---|---|---|
| **Size** (or **Block Size**) | **Settings** > **Prefixes**, and the prefix page | All the numbers your prefix holds, for example 100 |
| **Remaining** | Same places | The free numbers inside your **Ranges** (from **Start** to **End**) that GS1 Assistant can still assign |
| **Available GTINs** | **Dashboard** | The **Remaining** numbers of all your prefixes added together |
| Tab counts: **All**, **Valid GTINs**, **Needs GTIN**, **Duplicate GTINs**, **Not a GTIN** | **Dashboard**, **Settings** and **GTIN Manager** | Variants in your Shopify store, from the last scan |

![screenshot:A row of the Prefixes table: prefix 5065023978 with Size 100 and Remaining 39 outlined, GS1 UK, Left Foot Software.](CountsPrefixRow.png)

### Common reasons and fixes

- **The tab counts did not change after you assigned or edited barcodes.** The counts update only when GS1 Assistant scans your store. Click **Start Scan** and wait for it to finish.
- **Remaining is lower than Size minus the GTINs you used.** **Remaining** counts only the numbers inside your ranges. For example, with **Start** 51 and **End** 89, a prefix of 100 shows **Remaining** 39. To use more of the prefix, widen the range. See [Add and Manage Your Company Prefix](https://gs1assistant.crisp.help/en/article/adding-and-managing-your-company-prefix-6cxy7p/).
- **Remaining is higher than you expect.** GS1 Assistant sees only the barcodes in your Shopify store. GTINs you used elsewhere, or on products you deleted, look free to the app. Raise **Start**, or import the used GTINs under **Exclude**. See [How to Avoid Duplicate GTIN Assignments](https://gs1assistant.crisp.help/en/article/how-to-avoid-duplicate-gtin-assignments-6wuc5a/).
- **Remaining did not go up after you removed a GTIN.** Removing a GTIN from a variant does not return the number to your free GTINs. Click **Help** > **Chat with us** and ask support to reset your range. Reuse a number only if it was never published.
- **The highest number in your prefix is 99 or 999, not 100 or 1,000.** The numbers in a prefix start at 0. A prefix of 100 runs from 0 to 99, which is why the range shows **Minimum** 0 and **Maximum** 99. All 100 numbers are there.
- **The tabs add up to more than All.** A variant with a duplicate GTIN also counts under **Valid GTINs** or **Not a GTIN**. For details, see [What the GTIN Status Counts and Tabs Mean](https://gs1assistant.crisp.help/en/article/understanding-gtin-status-what-ok-invalid-unassigned-and-verified-mean-cieak9/).
- **The counts are higher than your number of products.** The counts are per variant. A shirt in 3 sizes counts 3 times.
- **A list shows fewer rows than its tab count.** The tab counts include every variant. The list shows only the variants that match your search and **Status** filter. Clear the search, or set **Status** to **Draft** or **Archived**.
- **A barcode you typed counts under Not a GTIN.** It has a wrong check digit, a hidden character or a space. Type it again in Shopify, then click **Start Scan**.

### Still wrong?

Click **Start Scan**, then compare again. If a count still looks wrong, click **Help** > **Chat with us** and include the count you see and the count you expect.

### Related articles

- [What the GTIN Status Counts and Tabs Mean](https://gs1assistant.crisp.help/en/article/understanding-gtin-status-what-ok-invalid-unassigned-and-verified-mean-cieak9/)
- [How to Avoid Duplicate GTIN Assignments](https://gs1assistant.crisp.help/en/article/how-to-avoid-duplicate-gtin-assignments-6wuc5a/)
- [Add and Manage Your Company Prefix](https://gs1assistant.crisp.help/en/article/adding-and-managing-your-company-prefix-6cxy7p/)
