## Download Barcode Images for Your GTINs

Download a barcode image for each variant that has a GTIN, in SVG or PNG format, to use on packaging, labels or tags.

### Before you start

- **Your variants have GTINs.** They are listed under the **Valid GTINs** tab in **GTIN Manager**. To give them GTINs, see [Assign GTINs to Many Variants at Once](https://gs1assistant.crisp.help/en/article/bulk-gtin-assignment-assign-barcodes-to-your-entire-catalogue-at-once-1vrtodi/).
- **GS1 Assistant makes the image only.** It does not print labels, and it does not check the size or print quality of your barcode.

### Download barcode images

1. In **GTIN Manager**, click the **Valid GTINs** tab.
2. Tick the variants you need. To select the whole list, tick the top checkbox, then click **Select all [number]+ variants**.
3. Click **Download Barcode** in the bar above the list.
4. In the **Select Barcode Format** window, click **SVG Format** or **PNG Format**.

![screenshot:The Select Barcode Format window with the text Choose the format for downloading barcodes. The SVG Format and PNG Format buttons (4) are outlined, with Cancel below.](BarcodeFormatWindow.png)

The window closes and your browser downloads a ZIP file. GS1 Assistant shows no message. Look for the file in your browser's downloads.

To download the barcode of one variant, click the eye icon on its row. The variant page shows the barcode with a **Download Barcode** button at the top.

### What the file contains

- **The ZIP file** is named with the format, your store and the date, for example barcodes_png_yourstore_2026-11-05.zip.
- **Each image** is named with the product, the variant and the GTIN, for example Linen_Shirt_-_Blue_S_05065023978519.png.
- **The PNG image** shows the bars with the GTIN digits below them, on a white background, at 448 × 244 pixels.

![screenshot:A downloaded PNG barcode image: black bars with the number 05065023978519 below them, on a white background.](BarcodePNGExample.png)

Choose **SVG Format** when you print large or resize the barcode: an SVG image stays sharp at any size. A PNG image has a fixed number of pixels and blurs when you enlarge it.

### Before you print

- **Check the barcode type.** In our test, the PNG image was a Code 128 barcode of the 14-digit GTIN. Shop checkouts usually scan EAN-13 or UPC-A barcodes. Ask your retailer or your printer which barcode type they need.
- **Leave white space at the sides.** The image has no white margin at its left and right edges. Keep a clear space on both sides when you place it on your design.
- **Test a print.** Print one barcode and scan it before you print many.

### Troubleshooting

- **Download Barcode is not in the bar.** Tick at least one variant first.
- **Nothing downloaded.** Open your browser's downloads list. If your browser blocked the download, allow downloads from admin.shopify.com, then try again.

### Related articles

- [Assign a GTIN to One Variant](https://gs1assistant.crisp.help/en/article/assign-your-first-gtin-to-a-product-1kpwezj/)
- [Assign GTINs to Many Variants at Once](https://gs1assistant.crisp.help/en/article/bulk-gtin-assignment-assign-barcodes-to-your-entire-catalogue-at-once-1vrtodi/)
- [UPC vs EAN vs GTIN: What Do I Actually Need?](https://gs1assistant.crisp.help/en/article/upc-vs-ean-vs-gtin-3b4ykj/)
