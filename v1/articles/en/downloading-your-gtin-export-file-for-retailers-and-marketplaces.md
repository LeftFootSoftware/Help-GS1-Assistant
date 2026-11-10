## Download an Import File for Your GS1 Portal

Download a file of your assigned GTINs and product details in your GS1 organization's format, then upload it to your GS1 portal.

### Do you need an import file?

GTINs you assign are already in the barcode field of your Shopify products. An import file is for adding those products to your GS1 organization's records.

| Your GS1 organization | How products reach GS1 |
|---|---|
| GS1 Germany, Netherlands, Sweden, Brazil | Auto Sync sends them for you after you connect your GS1 account. See [Set Up GS1 Assistant: Quick Start](https://gs1assistant.crisp.help/en/article/how-to-install-connect-and-add-your-prefix-17v6vte/). You can also download an import file. |
| GS1 UK, US, Canada, France, Norway, Romania | Download an import file and upload it to your GS1 portal. |
| Any other organization | GS1 Assistant has no file or sync for it yet. Add your products in your GS1 portal. |

This list is correct as of November 2026.

### Before you start

- **Your variants have GTINs.** They are listed under the **Valid GTINs** tab in **GTIN Manager**.
- **You know your product's GPC brick.** The **Category** field needs a GS1 brick, the most detailed level of the Global Product Classification. Click **GPC Browser** in the window to find it.

### Download the file

1. In **GTIN Manager**, click the **Valid GTINs** tab.
2. Tick the variants to include. To select the whole list, tick the top checkbox, then click **Select all [number]+ variants**.
3. Click **Download Import File** in the bar above the list.

![screenshot:The bar above the list with the Download Import File button (3) outlined.](ExportBarButton.png)

4. In **GS1 Member Organization**, choose your GS1 organization. The fields below change to match it.
5. In **Category**, choose your product's brick.
6. Fill in the other fields. For GS1 USA, change **Language** from **aa** to your language, for example **en**. If you leave it at **aa**, the language columns in the file stay empty, and GS1 US requires them.

![screenshot:The Download window for GS1 USA. GS1 Member Organization (4), Category (5) and Language set to aa (6) are outlined. Target Market, Brand, Net Content Count and Net Content Unit Of Measure are also shown.](ExportUSAWindow.png)

7. Click **Ok**.

For GS1 USA, the window also has **Target Market**, **Brand**, **Net Content Count**, **Net Content Unit Of Measure**, **Action**, **Packaging Level**, **Product Status**, **Industry**, **Purchasable** and **Variable**. Fill in **Brand**: in our test, an empty **Brand** put the store name in the file.

### Get the file from Downloads

GS1 Assistant builds the file in the background. A message confirms the request.

1. In the GS1 Assistant menu, click **Downloads**.
2. When the file shows "Your file is ready to download.", click **Download**.

The file stays on the **Downloads** page for 24 hours. For GS1 USA, it is an Excel file named GS1_US_Product_Import_ followed by a number.

### Upload the file to GS1

Upload the file to your GS1 portal, such as Data Hub for GS1 US. Check every row before you upload: GS1 Assistant fills in the file from your Shopify data and the fields you chose, and does not check it against your GS1 organization's rules.

### GS1 UK: update your NumberBank file

For GS1 UK, GS1 Assistant adds your GTINs and product details to a file you export from My Numberbank. It does not create a new file.

1. In the **Download** window, choose **GS1 UK**, then click **Choose File** and select the Excel file you exported from My Numberbank.
2. In **Category**, choose your product's brick.

![screenshot:The Download window for GS1 UK. Choose File (1) with the message Please Select GS1 UK NumberBank file to Update, and Category (2) with the message Please Select Brick, are outlined.](ExportUKWindow.png)

3. Check **Target Market**, **Status**, **Brand**, **Submit to Verified by GS1**, **Net Content** and **Unit Of Measure**, then click **Ok**.

**Ok** stays greyed out until you choose a file and a brick. Upload the updated file back to My Numberbank. Keep its columns and headers unchanged.

### Troubleshooting

- **Download Import File is not in the bar.** Tick at least one variant first.
- **Ok is greyed out (GS1 UK).** Choose your NumberBank file and a brick in **Category**.
- **The file is not on the Downloads page yet.** Wait a few minutes, then open **Downloads** again.
- **The GS1 US file has empty language columns.** Download it again with **Language** set to your language instead of **aa**.
- **Your GS1 organization is not in the list.** GS1 Assistant has no file for it yet. Add your products in your GS1 portal.

### Related articles

- [Assign GTINs to Many Variants at Once](https://gs1assistant.crisp.help/en/article/bulk-gtin-assignment-assign-barcodes-to-your-entire-catalogue-at-once-1vrtodi/)
- [Set Up GS1 Assistant: Quick Start](https://gs1assistant.crisp.help/en/article/how-to-install-connect-and-add-your-prefix-17v6vte/)
- [Understanding GTIN Status](https://gs1assistant.crisp.help/en/article/understanding-gtin-status-what-ok-invalid-unassigned-and-verified-mean-cieak9/)
