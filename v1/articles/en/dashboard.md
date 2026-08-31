## Dashboard



The Dashboard provides an overview of your product variants and their associated GTINs, along with tools to manage them efficiently. From this central hub, you can assign, track, and manage GTINs, view their statuses, and perform bulk actions.

**GTIN Status and Management**

The **GTIN Status** page gives you a detailed overview of the GTINs assigned to your product variants. You can filter variants by GTIN status to easily manage your inventory and ensure compliance with GS1 standards.

 **Status Filters:** Use the filter options to navigate between different statuses:

&nbsp;&nbsp; **Assigned:** View products that have valid GTINs assigned.

&nbsp;&nbsp;**Unassigned:** View products that do not yet have a GTIN assigned.

 &nbsp;&nbsp;**Valid:** Indicates GTINs that meet the required format and comply with GS1 standards, making them ready for use across supported platforms.

&nbsp;&nbsp;**Invalid:** Highlights any GTINs that do not conform to the required format or GS1 standards.

&nbsp;&nbsp;**Duplicates:** Displays any GTINs that are duplicated across variants.

**GTIN Block Status:** In addition to the product status

&nbsp;&nbsp; **Available:** Shows the total number of GTINs remaining in the configured company prefix block, helping you keep track of how many GTINs can still be assigned.

&nbsp;&nbsp;**Pending Shopify:** GTINs that have been assigned but are still in the process of being synced or accepted by Shopify.

 &nbsp;&nbsp; **Pending GS1:** GTINs submitted for validation that are awaiting confirmation or verification from GS1.

 &nbsp;&nbsp; **Downloads:** GTINs that have been exported or downloaded for use in external systems or records.

**Manual and Automatic Refresh**

The Dashboard displays the last time the GTIN data was updated, allowing you to keep track of recent changes. A manual refresh can be triggered using the Refresh button at the top of the dashboard.

 &nbsp;&nbsp;**Automatic Refresh:** After any action, such as assigning or unassigning GTINs, the dashboard will automatically refresh to reflect the updated product status.

&nbsp;&nbsp;**Manual Refresh:** If needed, you can manually refresh the page using the Refresh button to update the status and product list at any time.

**Note:** For stores with a large number of products, the refresh process may take some time, depending on the size of your catalog.

**Catalog Status:**

&nbsp;&nbsp;The Status column shows whether the product’s GTIN exists in the GS1 Catalog.

&nbsp;&nbsp;**GTIN Status:** Indicates the validation status of the GTIN (Global Trade Item Number) against the GS1 Global Data Synchronization Network (GDSN)

&nbsp;&nbsp;**Verified:** Indicates whether the product’s GTIN and associated attributes (brand, description, etc.) have been validated through the Verified by GS1 service

![screenshot:Dashboard](Dashboard.png)

**Assigning and Unassigning GTINs**

The Dashboard allows you to assign and unassign GTINs directly from the variant list. You can do this either individually or in bulk, making it easier to handle large product catalogs

**1. Individual GTIN Assignment:**

&nbsp;&nbsp;Next to each product variant, you’ll see an Assign GTIN button. Click this button to manually assign a GTIN to that specific variant.

![screenshot:Assign GTINS](AssignGTINs.png)

**2. Bulk GTIN Assignment and Unassignment:**

&nbsp;&nbsp;You can assign or unassign GTINs for multiple products at once:

&nbsp;&nbsp;Select multiple product variants by checking the boxes next to them

&nbsp;&nbsp;Click the **Assign** button at the top of the list to automatically assign available GTINs to all selected variants.

&nbsp;&nbsp;To remove GTINs, use the **Unassign** button to unassign GTINs from the selected variants.

![screenshot:Bulk GTINS](BulkAction.png)

**Filtering and Searching for Variants**

The dashboard includes advanced filtering and search options to help you quickly locate specific product variants:

&nbsp;&nbsp;**Search Bar (Filter Variants):** You can use the search box to enter keywords, product titles, or GTINs to refine the list of variants. This feature allows you to quickly filter products based on their name, description, or other relevant data. For example, entering new in the search bar will filter the list to only show products that contain new in their title ordetails.

&nbsp;&nbsp;**Status Filters:** Use the status filters (Assigned, Unassigned, Duplicates, Valid, Invalid) to refine the list of products shown on the dashboard.

![screenshot:Filters GTINS](SearchingFilters.png)

**Synchronizing with Your GS1 Catalog**

You can synchronize your products with your GS1 Catalog in one of two ways:

&nbsp;&nbsp;**1. Direct Connection:** 

&nbsp;&nbsp;  If you have configured a direct connection with your GS1 entity (such as GS1 Germany), your products will sync automatically with the GS1 Catalog.

&nbsp;&nbsp;**2. Exporting and Importing:** 

&nbsp;&nbsp;  You can also export product data from GS1 Assistant and import it into your GS1 Catalog manually. The app currently supports export formats for **GS1 USA** and **GS1 Germany**.

&nbsp;&nbsp;If your region is not yet supported, and you’re able to assist with expanding functionality to additional GS1 entities, please reach out to us.

![screenshot:Download GTINS](DownloadModel.png)
