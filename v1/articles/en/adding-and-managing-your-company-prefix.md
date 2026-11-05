## Add and Manage Your Company Prefix

Add your GS1 company prefix to GS1 Assistant, then choose its GTIN type and the range of numbers the app assigns from.

### Before you start

- **Your GS1 company prefix**, from your GS1 certificate or your GS1 account. Not sure you have one? See [Before You Install: Do You Have a GS1 Company Prefix?](https://gs1assistant.crisp.help/en/article/before-you-install-do-you-have-a-gs1-company-prefix-1rhru8v/)
- **A plan that fits your prefix.** Essential supports prefixes up to 100 GTINs, Growth up to 1,000, and Automation any size.

### Add a prefix

1. In the GS1 Assistant menu, click **Settings**.
2. In **Prefixes**, click the arrow next to **Add**.
3. Click **Add Existing Prefix**.

![screenshot:Settings, Prefixes. The arrow next to Add (2) is open, and Add Existing Prefix (3) is outlined in the menu.](QuickStartAddMenu.png)

4. In **Company prefix or name**, type your prefix (numbers only, 6 to 11 digits) or search for your company name as GS1 registered it.
5. Click **Add Prefix**.

![screenshot:The Add your company prefix window. The Company prefix or name field (4) and the Add Prefix button (5) are outlined.](QuickStartAddPrefix.png)

> **GS1 US and GS1 Canada prefixes:** add a leading 0. For example, enter 12345 as 012345. Enter the GS1 Company Prefix from your certificate, not the U.P.C. Company Prefix.

The **Prefixes** table lists each prefix with its **Size**, **Remaining** GTINs, **Member Organization** and **Company**. The **Company** column shows the company GS1 has on record for the prefix. You can add more than one prefix. Each one keeps its own ranges and its own count of remaining GTINs.

### Change the GTIN type

The **GTIN Type** sets the format GS1 Assistant writes to the Shopify barcode field. The options are **EAN** and **GTIN**. With **GTIN**, prefix 5065023978 gives 14-digit barcodes such as 05065023978496.

1. In the GS1 Assistant menu, click **Settings**.
2. In the **Prefixes** table, scroll right and click the pencil icon on the prefix's row. The **Company Prefixes** page opens.

![screenshot:The Prefixes table scrolled right. The pencil icon (2) on the row of prefix 5065023978 is outlined.](PrefixEditIcon.png)

3. In **GTIN Type**, choose **EAN** or **GTIN**.
4. Click **Save** in the bar at the top of the page.

![screenshot:The Company Prefixes page with Prefix Details. The GTIN Type list (3) set to EAN and the Save button (4) in the Unsaved changes bar are outlined.](PrefixGTINType.png)

The new type applies to GTINs assigned from now on. Barcodes already assigned keep their old format. To change them, unassign them and assign them again; see [Assign a GTIN to One Variant](https://gs1assistant.crisp.help/en/article/assign-your-first-gtin-to-a-product-1kpwezj/).

### Change the range the app assigns from

**Ranges** set which numbers in your prefix GS1 Assistant may use. **Minimum** and **Maximum** show the lowest and highest number the prefix allows. The app assigns the next free number from **Start** up to **End**.

1. In the GS1 Assistant menu, click **Settings**.
2. In the **Prefixes** table, scroll right and click the pencil icon on the prefix's row.
3. In **Ranges**, type the **Start** and **End** numbers. To add another range, click the plus icon.
4. Click **Save** in the bar at the top of the page.

![screenshot:The Ranges section with Start 51 and End 89 (3) outlined, and Minimum 0 and Maximum 99 below them.](PrefixRanges.png)

Used GTINs from this prefix outside GS1 Assistant? Set **Start** above the highest number you already used, and list any GTINs to skip under **Exclude**. See [How to Avoid Duplicate GTIN Assignments](https://gs1assistant.crisp.help/en/article/how-to-avoid-duplicate-gtin-assignments-6wuc5a/).

### Get a new prefix from GS1 US

If you sell in the US and do not have a prefix yet, click the arrow next to **Add**, then **Get a New Prefix**. The **License Company Prefix** window lists GS1 US packages by number of GTINs, from 1-10 to 1-100,000, with their prices. To find the GS1 organization for another country, click **Find My GS1 Member Organization**.

![screenshot:The License Company Prefix window from GS1 US Channel Partner, with packages 1-10, 1-100, 1-1,000, 1-10,000 and 1-100,000 and their prices.](PrefixLicenseNew.png)

### Connect your GS1 account

For prefixes from GS1 Germany, Netherlands, Sweden and Brazil, a **Connect** button appears in the **GS1 Connection** column. Connecting needs the **Growth** plan or above. See [Set Up GS1 Assistant: Quick Start](https://gs1assistant.crisp.help/en/article/how-to-install-connect-and-add-your-prefix-17v6vte/) for the steps.

### Troubleshooting

- **"Prefix is not valid" when you add your prefix.** Check the digits, and add the leading 0 for a GS1 US or GS1 Canada prefix. Use the GS1 Company Prefix, not the U.P.C. Company Prefix. A prefix bought or renewed recently can take from a few hours to about a week to reach GS1's registry. If it still fails, click **Help** > **Chat with us**.
- **Your company name finds nothing.** Search for the name GS1 registered, which can differ from your store name. Or type the prefix digits instead.
- **The Company column shows a company that is not yours.** The prefix is registered to that company. A prefix covers only products of the company it belongs to.
- **Every new barcode has an extra leading 0.** The **GTIN Type** is set to **GTIN**. Change it, then unassign and assign the affected barcodes again.

### Related articles

- [Set Up GS1 Assistant: Quick Start](https://gs1assistant.crisp.help/en/article/how-to-install-connect-and-add-your-prefix-17v6vte/)
- [How to Avoid Duplicate GTIN Assignments](https://gs1assistant.crisp.help/en/article/how-to-avoid-duplicate-gtin-assignments-6wuc5a/)
- [Assign a GTIN to One Variant](https://gs1assistant.crisp.help/en/article/assign-your-first-gtin-to-a-product-1kpwezj/)
