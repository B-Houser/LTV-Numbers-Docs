# SamCart Data Sync Procedure

### Table Of Contents

1. [Set Up Webhooks](https://docs.ltvnumbers.com/samcart#1-set-up-webhooks)
    - [Create A Rule For Product Purchased](https://docs.ltvnumbers.com/samcart#create-a-rule-for-product-purchased)
    - [Create A Rule For Subscription Charged](https://docs.ltvnumbers.com/samcart#create-a-rule-for-subscription-charged)
2. [Historical Sales Data](https://docs.ltvnumbers.com/samcart#2-historical-sales-data)
    - [Export SamCart Order Data](https://docs.ltvnumbers.com/samcart#export-samcart-order-data)
    - [Export SamCart Recurring Subscriptions Data](https://docs.ltvnumbers.com/samcart#export-samcart-recurring-subscriptions-data)
    - [Export SamCart Limited Subscriptions Data](https://docs.ltvnumbers.com/samcart#export-samcart-limited-subscriptions-data)
    - [Import SamCart Historical Data Into LTV Numbers](https://docs.ltvnumbers.com/samcart#import-samcart-historical-data-into-ltv-numbers)

---

# 1. Set Up Webhooks

Webhooks pull your sales data in real time and should be set up first before importing historical sales data to avoid gaps in your data

1. <a href="https://app.ltvnumbers.com" target="_blank">Log into LTV Numbers</a>
2. In LTV Numbers’ side navigation bar, go to the "Settings" tab 
3. Click the "Copy" button for your Webhook URL in the “Clickfunnels Integrations” section. You will paste this into SamCart at a later step
4. In a separate browser window or tab, <a href="https://samcart.com/auth/login" target="_blank">log into SamCart</a>
5. Confirm you are in the appropriate SamCart dashboard
6. In SamCart’s top right navigation bar, click on the Settings gear
7. In the left menu, click Integrations
8. Click the link at the top that says "Click here to go to the new integration rules engine"
9. In the Integrations Setup tab, click New Integration
10. Select Notify URL in the dropdown of the popup window and click Next Step
11. In the Name this Integration field, type “LTV Numbers”
12. Paste the Webhook URL you copied earlier into SamCart's Notify URL field and edit the Webhook URL by replacing "clickfunnels" with "samcart"
14. Click Save Integration to create the webhook connection
    - Note: this only creates the connection. The next steps define what that integration is used for

### Create A Rule For Product Purchased

1. Go to the Global Rules tab of the SamCart integration rules engine and click New Rule
2. In the Webhook Rule popup box, select Product Purchased as the trigger and click Next Step
3. Select the LTV Numbers webhook in the Integration dropdown and select Send Notify URL POST in the Action dropdown
4. Click Next Step then click Submit to finish setting up the product purchased rule

### Create A Rule For Subscription Charged

1. Go to the Global Rules tab of the SamCart integration rules engine and click New Rule
2. In the Webhook Rule popup box, select Subscription Charged as the trigger and click Next Step
3. Select the LTV Numbers webhook in the Integration dropdown and select Send Notify URL POST in the Action dropdown
4. Click Next Step then click Submit to finish setting up the subscription charged rule


# 2. Historical Sales Data

After setting up webhooks to pull in real time sales data, import your one time orders, indefinite recurring subscriptions, and limited subscriptions for a complete picture of your data

### Export SamCart Order Data

1. In SamCart’s top navigation bar go to Activity > Orders
2. In the lower right, click Export CSV File
3. In the Export Report popup, set the Export Time Range to All Time
4. In the Email field, enter your email address you would like the export sent to and click Confirm
    - Note: this process may take some time to complete but you can continue to the next steps
5. Check your email for the export file and save it to your computer

### Export SamCart Recurring Subscriptions Data

1. In SamCart’s top navigation bar go to Activity > Subscriptions
2. In the Recurring Subscriptions section, click Export CSV File
3. In the Export Report popup, set the Export Time Range to All Time
4. In the Email field, enter your email address you would like the export sent to and click Confirm
    - Note: this process may take some time to complete but you can continue to the next steps
5. Check your email for the export file and save it to your computer

### Export SamCart Limited Subscriptions Data

1. In SamCart’s top navigation bar go to Activity > Subscriptions
2. In the Limited Subscriptions section, click Export CSV File
3. In the Export Report popup, set the Export Time Range to All Time
4. In the Email field, enter your email address you would like the export sent to and click Confirm
    - Note: this process may take some time to complete but you can continue to the next steps
5. Check your email for the export file and save it to your computer

### Import SamCart Historical Data Into LTV Numbers

1. In LTV Numbers' side menu, click "Upload" to get to the Data Uploader
2. Click the "Choose File" button
3. Select your SamCart Orders CSV file and click the "Next" button
4. In the "Choose Format" dropdown, select the corresponding format of the data file you wish to upload (e.g. select "SamCart Orders CSV" for your exported orders CSV file)
5. Click the “Next” button then the “Upload” button to begin the ingest process
6. Repeat this process for each of your exported CSV files, selecting "SamCart Recurring Subscriptions CSV" for your SamCart Recurring Subscriptions CSV and "SamCart Limited Subscriptions CSV" for your SamCart Limited Subscriptions CSV
    - Note: this process may take some time to complete
