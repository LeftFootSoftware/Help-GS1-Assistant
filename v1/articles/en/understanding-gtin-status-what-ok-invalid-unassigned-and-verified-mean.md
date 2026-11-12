## What the GTIN Status Counts and Tabs Mean

After each scan, GS1 Assistant sorts your variants into four groups: **Valid GTINs**, **Needs GTIN**, **Duplicate GTINs** and **Not a GTIN**. This article explains each group, the labels and colours in the list, and what to do next.

### Where you see the groups

The **Dashboard** and **Settings** show a count for each group next to **Start Scan**.

![screenshot:The four counters: Valid GTINs 34, Needs GTIN 2, Duplicate GTINs 5 and Not a GTIN 14.](StatusCounters.png)

In **GTIN Manager**, each group is a tab. The **All** tab lists every variant.

![screenshot:The GTIN Manager tabs: All 49, Valid GTINs 36, Needs GTIN 0, Duplicate GTINs 7 and Not a GTIN 13.](StatusTabs.png)

The counts update only when you scan. Click **Start Scan** after you assign GTINs or change barcodes in Shopify. A message confirms the scan request, and the counts change when the scan finishes.

### What each group means

| Group | What it means | What to do |
|---|---|---|
| **Valid GTINs** | The barcode has the format of a GTIN, and the **Member Organization** column shows which GS1 organization its prefix comes from. | Nothing in GS1 Assistant. To add the products to GS1's records, see [Download an Import File for Your GS1 Portal](https://gs1assistant.crisp.help/en/article/downloading-your-gtin-export-file-for-retailers-and-marketplaces-1y4cusk/). |
| **Needs GTIN** | The variant has no barcode. | Assign one: see [Assign a GTIN to One Variant](https://gs1assistant.crisp.help/en/article/assign-your-first-gtin-to-a-product-1kpwezj/) or [Assign GTINs to Many Variants at Once](https://gs1assistant.crisp.help/en/article/bulk-gtin-assignment-assign-barcodes-to-your-entire-catalogue-at-once-1vrtodi/). |
| **Duplicate GTINs** | More than one variant has the same barcode. The tab groups them in one row, for example "2 variants". | Keep the GTIN on one variant and give the others a new one. See [How to Avoid Duplicate GTIN Assignments](https://gs1assistant.crisp.help/en/article/how-to-avoid-duplicate-gtin-assignments-6wuc5a/). |
| **Not a GTIN** | The barcode field has a value that is not a valid GTIN. A label gives the reason, for example **Invalid Check Digit** or **Not GTIN**. | See **Fix a Not a GTIN value** below. |

> **Note:** Valid GTINs is a format check. It does not mean that GS1 has the product on record, or that a marketplace accepts the code. The **Verified by GS1** column shows whether a product was submitted to GS1.

**Why the counts add up to more than All:** a variant with a duplicate barcode also counts under **Valid GTINs** or **Not a GTIN**. For example, with All 49: Valid GTINs 36 + Needs GTIN 0 + Not a GTIN 13 = 49, and the 7 duplicates are inside those numbers.

### Labels and colours in the list

![screenshot:A Duplicate GTINs row with a red bar on the left: 2 variants, Duplicates, GTIN 05065023978496, GS1 UK.](StatusDuplicateRow.png)

![screenshot:A Not a GTIN row: Merino Beanie, Charcoal, barcode 5065023978992 with the label Invalid Check Digit.](StatusNotAGTIN.png)

The key below the list explains the rest:

![screenshot:The key below the list: Synced, submitted to GS1. Not submitted, not yet submitted to GS1. An amber bar, needs a GTIN assigned. A red bar, GTIN shared by more than one variant.](StatusLegend.png)

| You see | Meaning |
|---|---|
| **Synced** (Verified by GS1 column) | The product was submitted to GS1. |
| **Not submitted** (Verified by GS1 column) | The product was not yet submitted to GS1. This is normal if you have not sent it with Auto Sync or an import file. |
| Amber bar on the left of a row | The variant needs a GTIN. |
| Red bar on the left of a row | The GTIN is shared by more than one variant. |

The **Verified by GS1** column is at the right end of the list. On a small screen, scroll the list sideways to see it.

### Fix a Not a GTIN value

Most **Not a GTIN** values were in the barcode field before GS1 Assistant was installed, for example from a CSV import or another app. Common causes:

- **A hidden character or a space** in a real GTIN, often from a CSV import. Open the variant in Shopify, delete the barcode, type it again without spaces, save, then click **Start Scan**.
- **A wrong check digit**, shown as **Invalid Check Digit**. The last digit does not match the rest of the number. Check the number against your GS1 records.
- **A number that is not a GTIN**, such as a placeholder or an internal code. Replace it with a GTIN from your prefix: tick the variant, click **Unassign Barcode**, then assign a new GTIN from the **Needs GTIN** tab.

> **Warning:** Only replace a GTIN that was never published: not listed on a marketplace, not sent to GS1 and not printed on packaging.

### Troubleshooting

- **The counts look out of date.** Click **Start Scan**.
- **A product is missing from a tab.** The **Status** filter shows active products by default. Set **Status** to **Draft** or **Archived** after you click the tab, because clicking a tab resets the filter.
- **A barcode looks correct but shows as Not a GTIN.** It probably has a hidden character or space. Type it again in Shopify, then click **Start Scan**.

### Related articles

- [Assign a GTIN to One Variant](https://gs1assistant.crisp.help/en/article/assign-your-first-gtin-to-a-product-1kpwezj/)
- [How to Avoid Duplicate GTIN Assignments](https://gs1assistant.crisp.help/en/article/how-to-avoid-duplicate-gtin-assignments-6wuc5a/)
- [Download an Import File for Your GS1 Portal](https://gs1assistant.crisp.help/en/article/downloading-your-gtin-export-file-for-retailers-and-marketplaces-1y4cusk/)
