# ThriveCart Data Sync Procedure

### Table Of Contents

1. [Set Up Webhooks](https://docs.ltvnumbers.com/thrivecart#1-set-up-webhooks)
2. [Historical Sales Data](https://docs.ltvnumbers.com/thrivecart#2-historical-sales-data)
    - [Export ThriveCart Transactions](https://docs.ltvnumbers.com/thrivecart#export-thrivecart-transactions)
    - [Import ThriveCart Transactions Into LTV Numbers](https://docs.ltvnumbers.com/thrivecart#import-thrivecart-transactions-into-ltv-numbers)
3. [UTM Passthrough Script](https://docs.ltvnumbers.com/thrivecart#3-utm-passthrough-script)

---

# 1. Set Up Webhooks

Webhooks pull your sales data in real time and should be set up first before importing historical sales data to avoid gaps in your data

1. <a href="https://app.ltvnumbers.com" target="_blank">Log into LTV Numbers</a>
2. In LTV Numbers’ side navigation bar, go to the "Settings" tab 
3. Click the "Copy" button for your Webhook URL in the “Clickfunnels Integrations” section. You will paste this into ThriveCart at a later step
4. In a separate browser window or tab, <a href="https://thrivecart.com/login/" target="_blank">log into ThriveCart</a> and go to your vendor account 
5. In ThriveCart, in the top right drop down, go to Settings
6. Go to API & Webhooks in the lower right 
7. Go to Webhooks & notifications at the bottom
8. Type "LTV Numners" into the Name field
9. Paste the Webhook URL you copied earlier into ThriveCart's Webhook URL field and edit the Webhook URL by replacing "clickfunnels" with "thrivecart"
10. Click the Save This Webhook button. ThriveCart should notify you that your webhook has been saved


# 2. Historical Sales Data

After setting up webhooks to pull in real time sales data, import your past sales for a complete picture of your data

### Export ThriveCart Transactions

1. In the middle of ThriveCart’s top navigation bar go to Transactions 
2. In the date selector dropdown menu, select "All Time"
3. Ensure "All transactions" is selected in the transaction type dropdown menu 
4. Click "Download CSV" at the bottom of the page and save the file to your computer

### Import ThriveCart Transactions Into LTV Numbers

1. In LTV Numbers' side menu, click "Upload" to get to the Data Uploader
2. Click the "Choose File" button
3. Select your ThriveCart Transactions CSV file and click the "Next" button
4. In the "Choose Format" dropdown, select "ThriveCart Transactions CSV"
5. Click the "Next" button then the “Upload” button to begin the ingest process
6. Repeat this process for each of your exported CSV files, selecting "ThriveCart Recurring Subscriptions CSV" for your ThriveCart Recurring Subscriptions CSV and "ThriveCart Limited Subscriptions CSV" for your ThriveCart Limited Subscriptions CSV
    - Note: this process may take some time to complete


# 3. UTM Passthrough Script

Due to limitations with ThriveCart, all past UTM information is lost from the historical sales data and cannot be recovered. Follow the steps below for each of your landing pages to set up the UTM Passthrough Script to bring in UTMs through your webhook sales and thus enable traffic analysis going forward. 

1. Navigate to the editor of your landing page that sends traffic to one of your ThriveCart checkout pages
    - Note: you can check the CTA link to verify this landing page sends traffic to your ThriveCart checkout page, which should contain yourbusinessname.thrivecart.com/*
2. Paste the following script into the <body> or <footer> code of the landing page:
    >`<script src="https://storage.googleapis.com/ltv-numbers-prod/url_parameter_passthrough.js?v=x.x.x" defer></script>`
    - Note: if necessary, this script can also be placed in the <head> of the page but may cause unintended behavior
3. Save your landing page
4. Repeat the steps above for each landing page that sends traffic to your ThriveCart checkout page(s)
