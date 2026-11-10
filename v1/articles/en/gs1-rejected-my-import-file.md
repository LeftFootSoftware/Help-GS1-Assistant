## GS1 Rejected My Import File

Fix the most common reasons a GS1 portal rejects the import file you downloaded from GS1 Assistant. GS1 Assistant fills the file from your Shopify data and the fields you chose; your GS1 organization checks it against its own rules.

### Before you upload again

- **Read the error your GS1 portal shows.** It usually names the row and the column.
- **Download a new file** after each fix. Files stay on the **Downloads** page for 24 hours.
- **Keep the file as it is.** Do not rename, delete or reorder columns, and save it in the same format (Excel). Opening and saving it in another program can change it.

### Common reasons and fixes

- **The category is not a brick.** GS1 portals need the most detailed GPC level, the brick. A higher level, such as a segment, is rejected; GS1 Romania and GS1 Canada are known to reject it. In the **Download** window, click **GPC Browser** and choose a brick. Brick codes start with 1, for example 10001352.
- **The file has a different category from the one you chose (GS1 USA).** If the product has a Shopify product category, the file can carry a code taken from that category instead of the brick you chose, and that code is not always a brick. Before you upload, check the **GPCBrick** column: every code must start with 1. Replace any other code with your brick, for example 10001352.
- **The language columns are empty (GS1 USA).** The **Language** field in the **Download** window starts at **aa**. Left that way, the file has no language in its description columns, and GS1 US requires one. Download the file again with **Language** set to your language, for example **en**.
- **A French description is missing (GS1 Canada).** GS1 Canada asks for a French product description next to the English one. GS1 Assistant does not translate. Add the French text in the file's French description column before you upload.
- **The NumberBank file does not match (GS1 UK).** For GS1 UK, GS1 Assistant updates the Excel file you export from My Numberbank. Export a fresh file from My Numberbank for the same prefix, choose it under **Choose File**, and upload the result without changing its headers.
- **Blank rows (GS1 UK).** Delete empty rows from the file, then upload again.
- **The brand is your store name.** If you leave **Brand** empty, the file can use your Shopify store name. Fill in **Brand** in the **Download** window.
- **A GTIN is already used for another product in your GS1 portal.** GS1 Assistant cannot see products that exist only in your GS1 portal. Replace the GTIN and stop it happening again; see [How to Avoid Duplicate GTIN Assignments](https://gs1assistant.crisp.help/en/article/how-to-avoid-duplicate-gtin-assignments-6wuc5a/).
- **A barcode is not a valid GTIN.** Check the **Not a GTIN** tab in **GTIN Manager** and fix those variants before you download. See [What the GTIN Status Counts and Tabs Mean](https://gs1assistant.crisp.help/en/article/understanding-gtin-status-what-ok-invalid-unassigned-and-verified-mean-cieak9/).

### Still rejected?

Click **Help** > **Chat with us**. Include your GS1 organization, the file name, and the exact error your GS1 portal shows.

### Related articles

- [Download an Import File for Your GS1 Portal](https://gs1assistant.crisp.help/en/article/downloading-your-gtin-export-file-for-retailers-and-marketplaces-1y4cusk/)
- [What the GTIN Status Counts and Tabs Mean](https://gs1assistant.crisp.help/en/article/understanding-gtin-status-what-ok-invalid-unassigned-and-verified-mean-cieak9/)
