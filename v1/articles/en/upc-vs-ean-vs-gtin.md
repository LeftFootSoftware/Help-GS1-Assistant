## UPC vs EAN vs GTIN: What Do I Actually Need?

UPC, EAN and GTIN are names for the same family of product numbers. Use the GTINs from your own GS1 company prefix, in the format your GS1 organization issues.

### GTIN is the family name

GTIN stands for Global Trade Item Number. UPC and EAN are GTINs of different lengths:

| Name | Where it comes from |
|---|---|
| UPC (GTIN-12), 12 digits | GS1 US and GS1 Canada |
| EAN (GTIN-13), 13 digits | Most other GS1 organizations |
| GTIN-14, 14 digits | Any GTIN with digits added in front, often for cases and packs |
| EAN-8 (GTIN-8), 8 digits | Very small packages |

A 12-digit UPC with a 0 in front is the same number as a 13-digit EAN. With 00 in front, it is the same number as a GTIN-14. For example, 614141123452, 0614141123452 and 00614141123452 identify the same product.

> **Note:** ISBNs for books are 13-digit GTINs from ranges reserved for publishers. They come from ISBN agencies, not GS1. GS1 Assistant does not assign ISBNs.

### What GS1 Assistant writes

GS1 Assistant writes each GTIN in the format set by your prefix's **GTIN Type** under **Settings** > **Prefixes**:

- **EAN** writes 13 digits.
- **GTIN** writes 14 digits, starting with 0.

There is no 12-digit UPC type. A GS1 US or GS1 Canada prefix is added with a leading 0, so its codes are written as 13 or 14 digits. They are still the same numbers as your UPCs. To change the type, see [Add and Manage Your Company Prefix](https://gs1assistant.crisp.help/en/article/adding-and-managing-your-company-prefix-6cxy7p/).

GS1 Assistant reads UPC, EAN and GTIN-14 values that start with 0. It does not support EAN-8, or GTIN-14 values that start with 1 to 9. An 8-digit barcode shows under **Not a GTIN**.

### Which format do I need?

Use the format your GS1 organization issues. Most marketplaces and retailers accept both UPC and EAN. If a retailer or trading partner asks for a specific format, follow their requirement.

### Where GTINs go in Shopify

Shopify stores GTINs in the **Barcodes** field of each variant, under **More details** on the variant page. When GS1 Assistant assigns a GTIN, the field shows the number with the type **GTIN**.

![screenshot:The Barcodes field of a Shopify variant showing 05065023978526 with the type GTIN.](UPCShopifyBarcodes.png)

Each variant needs its own GTIN. A small and a large shirt are two products with two GTINs. Two different products must never share a GTIN.

### Do you need GTINs if you only sell in your own store?

Not always. If you sell only through your own Shopify store, you can use your own internal codes. GS1 also reserves prefixes that start with 02 or 2 for internal use only. GS1 Assistant can assign numbers from such a prefix; to set one up, click **Help** > **Chat with us**. Internal-use numbers are not accepted by retailers or marketplaces. If you start selling through those channels, move the products to GTINs from your GS1 company prefix.

### Common mistakes

- **Buying resold barcodes.** Cheap reseller barcodes are registered to another company, or to none, in GS1's records. Buy your prefix from a GS1 organization. See [Where Should I Buy GTINs From?](https://gs1assistant.crisp.help/en/article/where-should-i-buy-gtins-from-17okkfp/)
- **One GTIN on several variants.** Each size, colour or configuration needs its own GTIN. GS1 Assistant lists shared GTINs under **Duplicate GTINs**.
- **Reusing a GTIN for a different product.** A GTIN identifies one product for good. See [How to Avoid Duplicate GTIN Assignments](https://gs1assistant.crisp.help/en/article/how-to-avoid-duplicate-gtin-assignments-6wuc5a/).

### Next step

[Add and Manage Your Company Prefix](https://gs1assistant.crisp.help/en/article/adding-and-managing-your-company-prefix-6cxy7p/)
