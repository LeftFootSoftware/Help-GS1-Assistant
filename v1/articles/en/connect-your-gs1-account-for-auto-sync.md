## Connect Your GS1 Account for Auto Sync

Connect GS1 Assistant to your GS1 account, so the products you assign GTINs to are sent to your GS1 organization without an import file.

### Which GS1 organizations have Auto Sync

| Your GS1 organization | How products reach GS1 |
|---|---|
| GS1 Germany, Netherlands, Sweden, Brazil | Auto Sync, after you connect your GS1 account |
| GS1 UK, US, Canada, France, Norway, Romania | An import file; see [Download an Import File for Your GS1 Portal](https://gs1assistant.crisp.help/en/article/downloading-your-gtin-export-file-for-retailers-and-marketplaces-1y4cusk/) |
| Any other organization | You add products in your GS1 portal yourself |

This list is correct as of November 2026.

### Before you start

- **The right plan.** The plan page in the app lists "API Synchronization (where supported)" from **Growth** up, and "Auto Sync where your GS1 has an API" on **Automation**.
- **Your prefix is added** under **Settings** > **Prefixes**. See [Add and Manage Your Company Prefix](https://gs1assistant.crisp.help/en/article/adding-and-managing-your-company-prefix-6cxy7p/).
- **Admin access to your GS1 account.** The access token must come from a GS1 user with admin rights for the prefix you connect. For GS1 Germany, a token from a user without those rights does not work.

### Connect your GS1 account

1. In the GS1 Assistant menu, click **Settings**.
2. In the **Prefixes** table, click **Connect** in the **GS1 Connection** column of your prefix. The button shows only for prefixes from a GS1 organization the app can connect to.
3. In the **GS1 Connection** window, click the link to create an access token in your GS1 account (for GS1 Germany: **Generate Access Token on GS1 Germany**). Create the token there and copy it.
4. Paste the token into **Access Token**.

![screenshot:The GS1 Connection window for GS1 Germany: Generate API Token, Enter API Token and Synchronize Prefixes, then Select GS1 Member Organization GS1-Germany.de. The Generate Access Token on GS1 Germany link (3) and the Access Token field (4) are outlined.](QuickStartConnect.png)

5. Click **Validate**.

GS1 Assistant checks the token and connects to your GS1 account. If the token is refused, an error shows in the window and the prefix keeps its **Connect** button.

### What Auto Sync does after you connect

- **Assigning usually sends the product too.** When you assign a GTIN from a connected prefix, GS1 Assistant usually sends the product to GS1 at the same time.
- **Sync with GS1 sends products again.** To send products yourself, for example after you change their details, open **GTIN Manager**, select the products, and choose **Sync with GS1**. Sync with GS1 only sends product details to GS1. It does not assign GTINs.
- **The Verified by GS1 column shows the result.** **Synced** means the product was submitted to GS1. **Not submitted** means it was not sent yet.

Your GS1 organization checks what it receives and decides what it accepts.

> **Note:** Auto Sync is not Auto Assign. Auto Sync sends products to GS1. Auto Assign gives new products a GTIN through Shopify Flow. See [Assign GTINs to New Products Automatically with Shopify Flow](https://gs1assistant.crisp.help/en/article/using-shopify-flow-to-assign-gtins-to-new-products-1qol6ru/).

### Troubleshooting

- **No Connect button next to your prefix.** GS1 Assistant has no connection to that GS1 organization yet. Use an import file instead.
- **The token is refused.** Create a new token from a GS1 user with admin rights for this prefix, then paste it again.
- **Products stay Not submitted after you assign.** Select them in **GTIN Manager** and choose **Sync with GS1**. If they still do not change, click **Help** > **Chat with us**.

### Related articles

- [Set Up GS1 Assistant: Quick Start](https://gs1assistant.crisp.help/en/article/how-to-install-connect-and-add-your-prefix-17v6vte/)
- [Download an Import File for Your GS1 Portal](https://gs1assistant.crisp.help/en/article/downloading-your-gtin-export-file-for-retailers-and-marketplaces-1y4cusk/)
- [What the GTIN Status Counts and Tabs Mean](https://gs1assistant.crisp.help/en/article/understanding-gtin-status-what-ok-invalid-unassigned-and-verified-mean-cieak9/)
