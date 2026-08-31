## Configuration



The first step in using the GS1 Assistant app is configuring the settings that determine how your GTINs are assigned and managed.

This section will guide you through manage Company prefix, and configuring the app language.

![screenshot:Get Started](GetStarted.png)

 **Manage Company Prefix**

 Use your own GS1-assigned global company prefix (GPC) to generate GTINs.

A company prefix is assigned when you purchase barcodes through GS1

This requires entering your GCP, specifying the GTIN format (UPC/EAN/GTIN-14), and configuring the range of GTINs to be used.

![screenshot:Manage Company Prefix](ManageCompanyPrefix.png)

![screenshot:New Company Prefix](NewCompanyPrefix.png)

 **Updating a GS1 Company Prefix**

You can update an existing company prefix to set specific ranges for GTINs that should be assigned to your products

 **1. Open the GS1 Configuration Screen:**

 Click the Edit button next to the company prefix you want to update in the list.

 **2. Company Prefix and Block Size:**
The Company Prefix and Block Size fields are pre-filled and read-only. These fields show the prefix and the size of the block assigned, which cannot be changed after initial configuration.

 **3. Sequence Ranges:** You can optionally define sequence ranges for GTIN assignments. These ranges specify the order or sequence in which GTINs will be assigned to product variants from your company prefix block. It’s important to note that the sequence ranges are not the actual GTIN numbers, but the internal sequence positions within the block.

&nbsp;&nbsp; **Start:** Enter the starting sequence number. This is the first position in the company prefix block from which GTINs will begin to be assigned.

&nbsp;&nbsp; **End:** Enter the ending sequence number. This is the last sequence position that will be used for GTIN assignments.

![screenshot:Updating Prefix](UpdatingPrefix.png)

 **Connecting to GS1**

You can connect the app to your GS1 account to sync company prefixes and GTIN assignments. Once connected, prefixes stored in your GS1 account will be automatically pulled into the app.

 **1.  Connect to GS1:**

Click the Connect to GS1 button to start the process. You will need to generate an API token from your GS1 entity to establish the connection.

**2. Sync Company Prefixes:**

After connecting, your company prefixes will be synced with your GS1 account, and the Status column will indicate whether each prefix exists in the GS1 Catalog.

 **Note:** The syncing process will not overwrite your local configurations, but will only sync new data from GS1.

![screenshot:PrefixGrid](PrefixGrid.png)

![screenshot:Connect GS1](ConnectGS1.png)

**GS1 Defaults**

 This section allows you to set default product information used when assigning GTINs (Global Trade Item Numbers). These values help standardize your product listings across GS1-compliant systems and marketplaces.

![screenshot:GS1 Defaults](GS1Defaults.png)
