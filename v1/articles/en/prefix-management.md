## Managing Company Prefixes



**Entering Your Global Company Prefix (GCP)**

When adding or managing a company prefix in GS1 Assistant, you'll need to enter your Global Company Prefix (GCP). This is the unique identifier assigned to your company by a GS1 Member Organization.

**Selecting a Prefix**

You can type your company name in the Company Prefix field to filter the list of available prefixes. This makes it easier to find and select the correct prefix from your account.

**UPC Prefix Conversion**

If your prefix is a **UPC Prefix** (used for 12-digit barcodes in North America), you must add a leading `0` to convert it into a 13-digit format. This aligns it with GS1's Global Company Prefix (GCP) standard.

**Example:** If your UPC Prefix is `12345`, enter `012345` in the Company Prefix field.

**API Validation Requirements**

If your prefix is from a region with **Direct API Sync** capabilities (as shown in the "Capabilities by Region" table above), validation with API credentials is required.

**For regions with API access:**

1. **Enter your Company Prefix:** Type your company name to filter the list, or type or select your company prefix from the dropdown list.

2. **Verify Prefix Details:** The system will display the prefix details, including:
   - The prefix number
   - The GS1 region (e.g., GS1 Germany, GS1 US, GS1 UK)
   - The company name associated with the prefix

3. **Enter API Credentials:** The specific API credentials required vary by Member Organization. Common requirements include:
   - API Key
   - API Secret
   - Access Token
   - Other authentication credentials

   Refer to your specific Member Organization's documentation or portal for the exact credentials needed. Some Member Organizations provide links to generate these credentials directly from the prefix management interface.

4. **Save:** Once the API credentials are entered and validated, click the **Save** button to complete the setup.

**Important Notes:**

- API credentials are required to enable direct synchronization between GS1 Assistant and your GS1 Member Organization's repository.
- Without valid API credentials, you may see a warning that the prefix does not appear to be registered to your business.
- UPCs and GTINs must come from a prefix licensed to your company in order to be valid for retail and online marketplaces.
- If you see a warning message, verify that you've entered the correct prefix and that you have the proper API credentials for API-enabled regions.
