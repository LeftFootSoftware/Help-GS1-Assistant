## Assign GTINs to New Products Automatically with Shopify Flow

Set up Auto Assign so that every new variant gets a GTIN from your prefix when it is added in Shopify. Auto Assign runs through Shopify Flow.

### Before you start

- **The Automation plan.** Auto Assign and every GS1 Assistant action in Shopify Flow need the Automation plan. On other plans, assign GTINs yourself; see [Assign GTINs to Many Variants at Once](https://gs1assistant.crisp.help/en/article/bulk-gtin-assignment-assign-barcodes-to-your-entire-catalogue-at-once-1vrtodi/).
- **Shopify Flow**, a free Shopify app, installed from the [Shopify App Store](https://apps.shopify.com/flow).
- **A company prefix with free GTINs.** Check **Remaining** under **Settings** > **Prefixes**.

### Option 1: Import the ready-made workflow (recommended)

The ready-made workflow waits 10 seconds after a variant is added, checks that its barcode is empty, then runs **Assign GTIN to Variant**. The wait gives Shopify time to save the new variant before the check runs.

1. Download the workflow file: [Auto Assign GTIN to New Variants.flow](https://raw.githubusercontent.com/LeftFootSoftware/Help-GS1-Assistant/main/v1/assets/en/Auto%20Assign%20GTIN%20to%20New%20Variants.flow).
2. In your Shopify admin, open **Apps** > **Flow**.
3. Click **Import** and choose the file.
4. Click **Turn on workflow**.

### Option 2: Build the workflow yourself

1. In your Shopify admin, open **Apps** > **Flow** and click **Create workflow**.
2. Choose the trigger **Product variant added**.
3. Add an action: search for **GS1**, then choose **Assign GTIN to Variant** from **GS1 Assistant (UPC EAN GTIN)**.
4. Fill in both fields with **Add variable**: **Variant id** = `{{productVariant.id}}` and **Product id** = `{{product.id}}`.

![screenshot:The Assign GTIN to Variant action in Shopify Flow, with the Variant id and Product id fields. The Add variable links (4) are outlined.](FlowActionFields.png)

5. Click **Turn on workflow**.

![screenshot:A Shopify Flow workflow that is on: Product variant added, then Assign GTIN to Variant. The button now reads Turn off workflow.](FlowWorkflowOn.png)

To match the ready-made workflow, add a **Wait** step of 10 seconds after the trigger, and a **Condition** that the variant's barcode is empty before the action. Without the condition, check what the action does to a variant that already has a barcode before you rely on it.

### Check that it works

1. Add a test variant in Shopify with the barcode left empty, and save.
2. After about a minute, open the variant in Shopify. The barcode field shows a GTIN from your prefix, with the type **GTIN**.
3. In GS1 Assistant, click **Start Scan**. The variant appears under **Valid GTINs**.

In Shopify Flow, **Run history** lists each run of the workflow.

> **Warning:** a run can show as completed even when the variant did not get a GTIN. After you add products, click **Start Scan** in GS1 Assistant and check the **Needs GTIN** tab. Assign any variant left there yourself.

### Good to know

- **The action has no prefix setting.** Flow takes the GTIN from a prefix in your **Prefixes** table; you cannot choose which one in the workflow.
- **Auto Assign only covers variants added after you turn the workflow on.** For the products you already have, use [Assign GTINs to Many Variants at Once](https://gs1assistant.crisp.help/en/article/bulk-gtin-assignment-assign-barcodes-to-your-entire-catalogue-at-once-1vrtodi/).
- **The GS1 Assistant counts do not update by themselves after Flow assigns a GTIN.** Click **Start Scan**.
- **Auto Assign is not Auto Sync.** Auto Assign gives new variants a GTIN. Auto Sync sends products to GS1 where your GS1 organization has an API.

### Troubleshooting

- **A new variant has no GTIN.** Check that the workflow is on. Then check the **Needs GTIN** tab after **Start Scan**, and assign the variant yourself. If it keeps happening, add or lengthen the **Wait** step; bulk imports can need up to a minute.
- **The workflow runs but nothing is assigned on any variant.** Check that your plan is Automation. Flow actions work only on that plan.
- **The workflow stopped assigning.** Your prefix may have no free GTINs left. Check **Remaining** under **Settings** > **Prefixes**.

### Related articles

- [Assign GTINs to Many Variants at Once](https://gs1assistant.crisp.help/en/article/bulk-gtin-assignment-assign-barcodes-to-your-entire-catalogue-at-once-1vrtodi/)
- [Add and Manage Your Company Prefix](https://gs1assistant.crisp.help/en/article/adding-and-managing-your-company-prefix-6cxy7p/)
- [What the GTIN Status Counts and Tabs Mean](https://gs1assistant.crisp.help/en/article/understanding-gtin-status-what-ok-invalid-unassigned-and-verified-mean-cieak9/)
