## What GS1 Assistant Does (and What It Doesn't)

GS1 Assistant assigns GTINs from your own GS1 company prefix to your Shopify variants, shows which barcodes need attention, and helps you send your products to GS1.

### What you need

- **A GS1 company prefix** from your GS1 organization. GS1 Assistant assigns numbers from it; it does not create its own barcodes. Not sure you have one? See [Before You Install: Do You Have a GS1 Company Prefix?](https://gs1assistant.crisp.help/en/article/before-you-install-do-you-have-a-gs1-company-prefix-1rhru8v/)
- **A plan that fits your prefix.** Essential supports prefixes up to 100 GTINs, Growth up to 1,000, and Automation any size.

### What GS1 Assistant does

| Task | How |
|---|---|
| Assign GTINs | Pick variants in **GTIN Manager**, click **Assign GTIN**. The app takes the next free number from your prefix and writes it to the Shopify barcode field. |
| Find barcodes that need attention | After **Start Scan**, the tabs show variants that need a GTIN, share a GTIN, or hold a value that is not a GTIN, with the reason. |
| Give new products a GTIN automatically | Auto Assign through Shopify Flow. |
| Send products to GS1 | Auto Sync for GS1 Germany, Netherlands, Sweden and Brazil. An import file for GS1 UK, US, Canada, France, Norway and Romania. List as of November 2026. |
| Download barcode images | Click **Download Barcode** and choose **SVG Format** or **PNG Format**. |
| Get a prefix in the US | **Settings** > arrow next to **Add** > **Get a New Prefix** licenses a prefix from GS1 US through the app. |

Auto Assign needs the **Automation** plan. For sending products to GS1, the plan page lists "API Synchronization (where supported)" from **Growth** up, and "Auto Sync where your GS1 has an API" on **Automation**.

### What GS1 Assistant does not do

- **It does not sell barcodes of its own.** Every GTIN comes from a prefix registered to your business. In the US you can license that prefix through the app, but it still comes from GS1 US.
- **It does not replace your GS1 membership.** You keep your membership and pay its renewals with your GS1 organization.
- **It does not check that a code is accepted.** A GTIN under **Valid GTINs** has the right format. Whether GS1 has the product on record, and whether a marketplace accepts it, is decided outside the app.
- **It does not add products to GS1 by itself, except through Auto Sync.** Where Auto Sync is not available, you upload the import file to your GS1 portal.

### Is GS1 Assistant right for you?

It is a good fit if you:

- have a GS1 company prefix, or will license one;
- sell many variants and want to stop typing barcodes by hand;
- need to clean up barcode values from CSV imports or other apps.

It is not the right tool if you want low-cost barcodes from a reseller: those codes are not registered to your business, and GS1 Assistant cannot assign them from a prefix.

GS1 Assistant can also assign numbers for internal use only, from a prefix that starts with 02 or 2. These are not for retail or marketplaces. To set one up, click **Help** > **Chat with us**.

### Next step

- **You have a prefix:** [Set Up GS1 Assistant: Quick Start](https://gs1assistant.crisp.help/en/article/how-to-install-connect-and-add-your-prefix-17v6vte/)
- **You don't have one yet:** [Before You Install: Do You Have a GS1 Company Prefix?](https://gs1assistant.crisp.help/en/article/before-you-install-do-you-have-a-gs1-company-prefix-1rhru8v/)
