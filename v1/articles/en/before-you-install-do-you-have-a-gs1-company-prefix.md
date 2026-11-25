## Before You Install: Do You Have a GS1 Company Prefix?

Check whether you already have a GS1 company prefix, and get one if you don't. GS1 Assistant assigns GTINs only from a prefix registered to your business.

### What a company prefix is

A GS1 company prefix is a number that a GS1 organization issues to your business. Every GTIN you create starts with it, followed by a product number and a check digit.

For example, with the prefix 5065023978, the product number 00 and the check digit 7, the GTIN is 5065023978007. GS1 Assistant picks the product numbers and calculates the check digit for you.

![screenshot:Diagram of the GTIN 5065023978007: company prefix 5065023978, product number 00, check digit 7.](prefixexample.png)

### How many GTINs a prefix gives you

The longer the prefix, the fewer GTINs it holds. For a 13-digit GTIN:

| Prefix length | Number of GTINs |
|---|---|
| 11 digits | 10 |
| 10 digits | 100 |
| 9 digits | 1,000 |
| 8 digits | 10,000 |
| 7 digits | 100,000 |

Each variant needs its own GTIN. Count your variants, including sizes and colours, before you choose a size. Your GS1 Assistant plan also has a limit: Essential supports prefixes up to 100 GTINs, Growth up to 1,000, and Automation any size.

### Check whether you already have a prefix

- **Your GS1 account.** Log in to your GS1 organization's portal, for example GS1 US, GS1 UK or GS1 Germany. Your prefix is on your account or your certificate.
- **Your existing barcodes.** If you already used GS1 barcodes, they start with your prefix. For example, the GTIN 00614141123452 comes from the prefix 0614141.

> **Note:** GS1 US and GS1 Canada certificates show two numbers. GS1 Assistant needs the **GS1 Company Prefix**, not the U.P.C. Company Prefix.

### Get a prefix if you don't have one

- **In the US:** you can license a prefix from GS1 US inside GS1 Assistant. Go to **Settings**, click the arrow next to **Add**, then **Get a New Prefix**.

![screenshot:The License Company Prefix window from GS1 US Channel Partner, with packages 1-10, 1-100, 1-1,000, 1-10,000 and 1-100,000 and their prices.](PrefixLicenseNew.png)

- **Anywhere else:** buy a prefix from the GS1 organization in your country. Find yours on [GS1's list of member organizations](https://www.gs1.org/contact/overview).

Barcodes sold cheaply by resellers are not registered to your business. GS1's records show them under another company, or under none. See [Where Should I Buy GTINs From?](https://gs1assistant.crisp.help/en/article/where-should-i-buy-gtins-from-17okkfp/) and [UPC vs EAN vs GTIN: What Do I Actually Need?](https://gs1assistant.crisp.help/en/article/upc-vs-ean-vs-gtin-3b4ykj/).

### A new prefix shows "Prefix is not valid"

A prefix you bought or renewed recently can take from a few hours to about a week to reach GS1's registry. Until then, GS1 Assistant may show **Prefix is not valid** when you add it.

1. Check the digits. For GS1 US and GS1 Canada, add a leading 0, for example 012345.
2. Wait, then try to add the prefix again.
3. If it still fails after a week, or you need it sooner, click **Help** > **Chat with us**. The support team can check it for you.

### Once you have your prefix

Install GS1 Assistant and follow [Set Up GS1 Assistant: Quick Start](https://gs1assistant.crisp.help/en/article/how-to-install-connect-and-add-your-prefix-17v6vte/). If you already gave some products GTINs from this prefix, read [How to Avoid Duplicate GTIN Assignments](https://gs1assistant.crisp.help/en/article/how-to-avoid-duplicate-gtin-assignments-6wuc5a/) before you assign new ones.
