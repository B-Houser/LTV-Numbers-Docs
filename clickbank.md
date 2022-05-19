# ClickBank Data Sync Procedure

### Table Of Contents

1. [Webhook Secret Key](https://docs.ltvnumbers.com/clickbank#1-webhook-secret-key)
3. [Set Up Webhooks](https://docs.ltvnumbers.com/clickbank#2-set-up-webhooks)
4. [Historical Sales Data](https://docs.ltvnumbers.com/clickbank#3-historical-sales-data)
    - [Export Historical Sales Data From ClickBank](https://docs.ltvnumbers.com/clickbank#export-historical-sales-data-from-clickbank)
    - [Import ClickBank Historical Data Into LTV Numbers](https://docs.ltvnumbers.com/clickbank#import-clickbank-historical-data-into-ltv-numbers)

---

# 1. Webhook Secret Key

The Secret Key allows LTV Numbers to decrypt your webhook payloads

1. <a href="https://accounts.clickbank.com/login.htm" target="_blank">Log into ClickBank</a> 
2. In ClickBank's top navigation bar, click on Vendor Settings
3. On the My Site page, scroll down to the Advanced Tools section
4. Copy the Secret Key
5. Send your Secret Key to us at LTV Numbers via email or Slack
    - Note: a ClickBank integration is in the works that will improve this process

# 2. Set Up Webhooks

Webhooks pull your sales data in real time and should be set up first before importing historical sales data to avoid gaps in your data

1. <a href="https://app.ltvnumbers.com" target="_blank">Log into LTV Numbers</a>
2. In LTV Numbers' side navigation bar, go to the "Settings" tab 
3. Click the "Copy" button for your Webhook URL in the “ClickBank Integrations” section. You will paste this into ClickBank at a later step
4. In a separate browser window or tab, <a href="https://accounts.clickbank.com/login.htm" target="_blank">log into ClickBank</a>
6. In ClickBank's top navigation bar, click on Vendor Settings
7. On the My Site page, scroll down to the Advanced Tools section and click Edit
8. Paste the LTV Numbers Webhook URL into an empty "Instant Notification URL" field and edit the Webhook URL by replacing "clickfunnels" with "clickbank"
    - Note: if your account doesn't have any empty "Instant Notification URL" fields, request another slot from ClickBank support
10. Select the latest version (currently version 7.0)
11. Click the "Test IPN" button to verify the webhook
12. Once verified, click the Save Changes button

# 3. Historical Sales Data

After setting up webhooks to pull in real time sales data, import your past sales for a complete picture of your data. Note: due to Clickbank's exporting limitations, you may have to subdivide your data and export it in multiple batches. The goal here is to establish a good analysis baseline with at least a year of data. (Older data doesn't necessarily reflect the current state of the business.)

### Export Historical Sales Data From ClickBank

1. In the ClickBank’s top navigation, bar go to Reporting, then the Transactions page
2. At the top of the Transactions page, there is usually a link to download all of the previous year’s transactions. Click this link to download the CSV file of last year's data and save it to your computer. 
3. Export the current year to date sales data by setting the date range to the beginning of the year to today's date
4. Scroll to the bottom of the page, click the "Export Options: CSV" link, and save the file to your computer
    - Note: if there is too much data for ClickBank to export, the Export Options: CSV option will not be present. Choose a smaller date range and try again, repeating as necessary to include all of your relevant data.

### Import ClickBank Historical Data Into LTV Numbers

1. In LTV Numbers' side menu, click "Upload" to get to the Data Uploader
2. Click the "Choose File" button
3. Select the historical sales data CSV from the previous section and click the "Next" button
    - Note: if you have multiple sales record CSV files, you can multiselect them to upload them all at the same time. Otherwise, repeat this process for each file.
5. In the "Choose Format" dropdown, select "ClickBank Sales CSV" and click the "Next" then the "Upload" button button to begin the ingest process
    - Note: this process may take some time to complete
