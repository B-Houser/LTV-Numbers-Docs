# **DEPRECATED** Shopify Data Sync Procedure

**DEPRECATED** - This method is no longer supported and should only be used in special cases. For most cases, use the Shopify app method outlined [here](https://docs.ltvnumbers.com/shopify).

### Table Of Contents

1. [Set Up Webhooks](https://docs.ltvnumbers.com/shopify-deprecated#1-set-up-webhooks)
3. [Historical Sales Data](https://docs.ltvnumbers.com/shopify-deprecated#2-historical-sales-data)
    - [Export Historical Sales Data From Shopify](https://docs.ltvnumbers.com/shopify-deprecated#export-historical-sales-data-from-shopify)
    - [Import Shopify Historical Data Into LTV Numbers](https://docs.ltvnumbers.com/shopify-deprecated#import-shopify-historical-data-into-ltv-numbers)

---

# 1. Set Up Webhooks

Webhooks pull your sales data in real time and should be set up first before importing historical sales data to avoid gaps in your data

1. <a href="https://app.ltvnumbers.com" target="_blank">Log into LTV Numbers</a>
2. In LTV Numbers’ side navigation bar, go to the "Settings" tab 
3. Click the "Copy" button for your Webhook URL in the “Shopify Integrations” section. You will paste this into Shopify at a later step
4. In a separate browser window or tab, <a href="https://accounts.shopify.com/store-login" target="_blank">log into Shopify</a>
    - To log in as a Shopify Partner, <a href="https://partners.shopify.com/organizations" target="_blank">log in to your Shopify Partner account</a>, then click "Log In" next to the appropriate Shopify store 
        - Note: Your partner account will need all permissions except for Online Store permissions, Manage locations, View Shopify Payments payouts, and View billing details
6. In Shopify's side navigation bar, go to Settings
7. Click on Notifications and scroll to the Webhooks section
8. Click the "Create Webhook" button and configure each field as follows:
    - Event: "Order payment"
    - Format: "JSON"
    - URL: Paste the LTV Numbers Webhook URL and edit the Webhook URL by replacing "clickfunnels" with "shopify"
    - Webhook API version: select the (Latest) version (i.e. "yyyy-mm (Latest)")
10. Click the "Save" button
11. Repeat steps 7 - 10 for Event: "Refund create"


# 2. Historical Sales Data

After setting up webhooks to pull in real time sales data, import your past sales for a complete picture of your data

### Export Historical Sales Data From Shopify

1. From your Shopify home dashboard, go to Analytics then Reports in the left menu
2. Click the "Sales by product" report in the Sales section
3. Select a date range that contains the historial sales data you with to export
    - Note: we recommend at least a year of historical data to establish a good analysis baseline. Older data doesn't necessarily reflect the current state of the business.
4. Click the Edit Columns dropdown and select all columns
5. At the top right, click Export > Export to generate your historical sales data CSV
6. When your file is ready, click the “Download” button
7. Save the file to your computer

### Import Shopify Historical Data Into LTV Numbers

1. In LTV Numbers' side menu, click "Upload" to get to the Data Uploader
2. Click the "Choose File" button
3. Select the historical sales data CSV from the previous section and click the "Next" button
4. In the "Choose Format" dropdown, select "Shopify Orders CSV" and click the "Next" button to begin the ingest process
    - Note: this process may take some time to complete
