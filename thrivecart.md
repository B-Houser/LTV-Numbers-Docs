# ThriveCart Data Sync Procedure

### Table Of Contents

1. [Set Up Webhooks](https://docs.ltvnumbers.com/thrivecart#1-set-up-webhooks)
    - [Create A Rule For Product Purchased](https://docs.ltvnumbers.com/thrivecart#create-a-rule-for-product-purchased)
    - [Create A Rule For Subscription Charged](https://docs.ltvnumbers.com/thrivecart#create-a-rule-for-subscription-charged)
2. [Historical Sales Data](https://docs.ltvnumbers.com/thrivecart#2-historical-sales-data)
    - [Export ThriveCart Order Data](https://docs.ltvnumbers.com/thrivecart#export-thrivecart-order-data)
    - [Export ThriveCart Recurring Subscriptions Data](https://docs.ltvnumbers.com/thrivecart#export-thrivecart-recurring-subscriptions-data)
    - [Export ThriveCart Limited Subscriptions Data](https://docs.ltvnumbers.com/thrivecart#export-thrivecart-limited-subscriptions-data)
    - [Import ThriveCart Historical Data Into LTV Numbers](https://docs.ltvnumbers.com/thrivecart#import-thrivecart-historical-data-into-ltv-numbers)

---

# 1. Set Up Webhooks

Webhooks pull your sales data in real time and should be set up first before importing historical sales data to avoid gaps in your data

1. <a href="https://app.ltvnumbers.com" target="_blank">Log into LTV Numbers</a>
2. In LTV Numbers’ side navigation bar, go to the "Settings" tab 
3. Click the "Copy" button for your Webhook URL in the “Clickfunnels Integrations” section. You will paste this into ThriveCart at a later step
4. In a separate browser window or tab, <a href="https://thrivecart.com/login/" target="_blank">log into ThriveCart</a>
5. Confirm you are in the appropriate ThriveCart dashboard
6. In ThriveCart's top right navigation bar, click on the Settings gear
7. In the left menu, click Integrations
8. Click the link at the top that says "Click here to go to the new integration rules engine"
9. In the Integrations Setup tab, click New Integration
10. Select Notify URL in the dropdown of the popup window and click Next Step
11. In the Name this Integration field, type “LTV Numbers”
12. Paste the Webhook URL you copied earlier into ThriveCart's Notify URL field and edit the Webhook URL by replacing "clickfunnels" with "thrivecart"
14. Click Save Integration to create the webhook connection
    - Note: this only creates the connection. The next steps define what that integration is used for

### Create A Rule For Product Purchased

1. Go to the Global Rules tab of the ThriveCart integration rules engine and click New Rule
2. In the Webhook Rule popup box, select Product Purchased as the trigger and click Next Step
3. Select the LTV Numbers webhook in the Integration dropdown and select Send Notify URL POST in the Action dropdown
4. Click Next Step then click Submit to finish setting up the product purchased rule

### Create A Rule For Subscription Charged

1. Go to the Global Rules tab of the ThriveCart integration rules engine and click New Rule
2. In the Webhook Rule popup box, select Subscription Charged as the trigger and click Next Step
3. Select the LTV Numbers webhook in the Integration dropdown and select Send Notify URL POST in the Action dropdown
4. Click Next Step then click Submit to finish setting up the subscription charged rule


# 2. Historical Sales Data

After setting up webhooks to pull in real time sales data, import your one time orders, indefinite recurring subscriptions, and limited subscriptions for a complete picture of your data

### Export ThriveCart Order Data

1. In ThriveCart's top navigation bar go to Activity > Orders
2. In the lower right, click Export CSV File
3. In the Export Report popup, set the Export Time Range to All Time
4. In the Email field, enter your email address you would like the export sent to and click Confirm
    - Note: this process may take some time to complete but you can continue to the next steps
5. Check your email for the export file and save it to your computer

### Export ThriveCart Recurring Subscriptions Data

1. In ThriveCart's top navigation bar go to Activity > Subscriptions
2. In the Recurring Subscriptions section, click Export CSV File
3. In the Export Report popup, set the Export Time Range to All Time
4. In the Email field, enter your email address you would like the export sent to and click Confirm
    - Note: this process may take some time to complete but you can continue to the next steps
5. Check your email for the export file and save it to your computer

### Export ThriveCart Limited Subscriptions Data

1. In ThriveCart's top navigation bar go to Activity > Subscriptions
2. In the Limited Subscriptions section, click Export CSV File
3. In the Export Report popup, set the Export Time Range to All Time
4. In the Email field, enter your email address you would like the export sent to and click Confirm
    - Note: this process may take some time to complete but you can continue to the next steps
5. Check your email for the export file and save it to your computer

### Import ThriveCart Historical Data Into LTV Numbers

1. In LTV Numbers' side menu, click "Upload" to get to the Data Uploader
2. Click the "Choose File" button
3. Select your ThriveCart Orders CSV file and click the "Next" button
4. In the "Choose Format" dropdown, select the corresponding format of the data file you wish to upload (e.g. select "ThriveCart Orders CSV" for your exported orders CSV file) and click Upload
5. Repeat this process for each of your exported CSV files, selecting "ThriveCart Recurring Subscriptions CSV" for your ThriveCart Recurring Subscriptions CSV and "ThriveCart Limited Subscriptions CSV" for your ThriveCart Limited Subscriptions CSV
    - Note: this process may take some time to complete
