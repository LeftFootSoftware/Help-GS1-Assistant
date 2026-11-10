## Set Up GS1 Assistant: Quick Start

Set up GS1 Assistant in three short tasks: scan your store, add your GS1 company prefix, and assign your first GTIN.

### Before you start

- **A GS1 company prefix.** GS1 Assistant assigns GTINs from a prefix you already own. Not sure you have one? See [Before You Install: Do You Have a GS1 Company Prefix?](https://gs1assistant.crisp.help/en/article/before-you-install-do-you-have-a-gs1-company-prefix-1rhru8v/)
- **A plan that fits your prefix.** Essential supports prefixes up to 100 GTINs, Growth up to 1,000, and Automation any size.
- **GS1 Assistant installed** from the Shopify App Store. Open it from **Apps** > **GS1 Assistant** in your Shopify admin.

The Dashboard's **Setup guide** lists the same tasks and ticks each one off as you finish it.

### 1. Scan your store

1. Open **GS1 Assistant**. The **Dashboard** opens.
2. Click **Start Scan**.

![screenshot:The top of the Dashboard: the Start Scan button (2), then the Valid GTINs and Needs GTIN counters.](QuickStartDashboardCounters.png)

When the scan finishes, the counters show how many variants have a valid GTIN (**Valid GTINs**), have no barcode (**Needs GTIN**), share a GTIN with another variant (**Duplicate GTINs**), or hold a value that is not a GTIN (**Not a GTIN**). Click **Start Scan** again whenever the counts look out of date.

### 2. Add your company prefix

1. In the GS1 Assistant menu, click **Settings**.
2. In **Prefixes**, click the arrow next to **Add**.
3. Click **Add Existing Prefix**.

![screenshot:Settings, Prefixes. The arrow next to Add (2) is open, and Add Existing Prefix (3) is outlined in the menu.](QuickStartAddMenu.png)

4. In **Company prefix or name**, type your prefix (numbers only, 6 to 11 digits) or search for your company name as GS1 registered it.
5. Click **Add Prefix**.

![screenshot:The Add your company prefix window. The Company prefix or name field (4) and the Add Prefix button (5) are outlined.](QuickStartAddPrefix.png)

> **GS1 US and GS1 Canada prefixes:** add a leading 0. For example, enter 12345 as 012345. Enter the GS1 Company Prefix from your certificate, not the U.P.C. Company Prefix.

The prefix appears in the **Prefixes** table with its **Size** and **Remaining** GTINs.

**Used GTINs from this prefix before?** Before you assign anything, set where the app should start, so it does not hand out a number that is already in use. See [How to Avoid Duplicate GTIN Assignments](https://gs1assistant.crisp.help/en/article/how-to-avoid-duplicate-gtin-assignments-6wuc5a/).

**No prefix yet, in the US?** Click the arrow next to **Add**, then **Get a New Prefix**, to license a prefix from GS1 US through the app.

### 3. Assign your first GTIN

1. In the GS1 Assistant menu, click **GTIN Manager**.
2. Click the **Needs GTIN** tab. It lists every variant without a barcode.
3. Tick the checkbox next to the variant.

![screenshot:GTIN Manager. The Needs GTIN tab (2) and the checkbox next to the first variant (3) are outlined.](QuickStartNeedsGTIN.png)

4. Click **Assign GTIN** in the bar above the list.

![screenshot:The bar above the list after selecting variants, with the Assign GTIN button (4) outlined.](QuickStartAssignBar.png)

5. In the **Select Company Prefix** window, check that your prefix is selected, then click **Assign**.

![screenshot:The Select Company Prefix window with prefix 5065023978, its Prefix Details, and the Assign button (5) outlined.](QuickStartSelectPrefix.png)

GS1 Assistant takes the next free GTIN from your prefix and writes it to the variant's barcode in Shopify. Click **Start Scan** to update the counts. The variant then appears under **Valid GTINs**.

The **Status** filter shows active products by default. To see draft products, set **Status** to **Draft** after you click a tab, because clicking a tab resets the filter.

### Connect your GS1 account (GS1 Germany, Netherlands, Sweden and Brazil)

If your prefix comes from one of these GS1 organizations, you can connect the app to your GS1 account so your products can sync to GS1. The plan page in the app lists "API Synchronization (where supported)" from **Growth** up, and "Auto Sync where your GS1 has an API" on **Automation**.

1. In the GS1 Assistant menu, click **Settings**.
2. In the **Prefixes** table, click **Connect** in the **GS1 Connection** column of your prefix. The button shows only where the app can connect to that prefix's GS1 organization.
3. In the **GS1 Connection** window, click the link to generate an access token in your GS1 account (for GS1 Germany: **Generate Access Token on GS1 Germany**).
4. Paste the token into **Access Token**.
5. Click **Validate**.

![screenshot:The GS1 Connection window for GS1 Germany. The Generate Access Token on GS1 Germany link (3) and the Access Token field (4) are outlined.](QuickStartConnect.png)

You do not need to connect to assign GTINs. For GS1 UK, US, Canada, France, Norway and Romania, download an import file for your GS1 portal instead; see [Downloading Your GTIN Export File for Retailers and Marketplaces](https://gs1assistant.crisp.help/en/article/downloading-your-gtin-export-file-for-retailers-and-marketplaces-1y4cusk/).

### What to do next

- **Assign GTINs to the rest of your catalog:** [Assign GTINs to Many Variants at Once](https://gs1assistant.crisp.help/en/article/bulk-gtin-assignment-assign-barcodes-to-your-entire-catalogue-at-once-1vrtodi/)
- **Give new products a GTIN automatically** (Automation plan): [Using Shopify Flow to Assign GTINs to New Products](https://gs1assistant.crisp.help/en/article/using-shopify-flow-to-assign-gtins-to-new-products-1qol6ru/)
- **Fill in your GS1 Defaults** (brand, category, language and more) under **Settings** > **GS1 Defaults** before you download an import file.

### Troubleshooting

- **"Prefix is not valid" when you add your prefix.** Check the digits, and add the leading 0 for a GS1 US or GS1 Canada prefix. Use the GS1 Company Prefix, not the U.P.C. Company Prefix. A prefix bought or renewed recently can take from a few hours to about a week to reach GS1's registry. If it still fails, click **Help** > **Chat with us**.
- **The counts look wrong or out of date.** Click **Start Scan**.
- **A product is missing from the list.** Check the **Status** filter. Draft and archived products appear only when you choose that status.
- **No Connect button next to your prefix.** The app has no API connection to your GS1 organization. If your organization is GS1 UK, US, Canada, France, Norway or Romania, use an import file instead.

### Related articles

- [Adding and Managing Your Company Prefix](https://gs1assistant.crisp.help/en/article/adding-and-managing-your-company-prefix-6cxy7p/)
- [Assign Your First GTIN to a Product](https://gs1assistant.crisp.help/en/article/assign-your-first-gtin-to-a-product-1kpwezj/)
- [Understanding GTIN Status](https://gs1assistant.crisp.help/en/article/understanding-gtin-status-what-ok-invalid-unassigned-and-verified-mean-cieak9/)
