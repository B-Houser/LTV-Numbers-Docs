# Clickfunnels Data Sync Procedure

### Table Of Contents

1. [Set Up Webhooks](https://docs.ltvnumbers.com/clickfunnels#1-set-up-webhooks)
3. [Historical Sales Data](https://docs.ltvnumbers.com/clickfunnels#2-historical-sales-data)
    - [Export Historical Sales Data From Clickfunnels](https://docs.ltvnumbers.com/clickfunnels#export-historical-sales-data-from-clickfunnels)
    - [Import Clickfunnels Historical Data Into LTV Numbers](https://docs.ltvnumbers.com/clickfunnels#import-clickfunnels-historical-data-into-ltv-numbers)
5. [Add Funnels](https://docs.ltvnumbers.com/clickfunnels#3-add-funnels)
    - [Add Funnels Individually](https://docs.ltvnumbers.com/clickfunnels#add-funnels-individually)
    - [Add Funnels As A Batch](https://docs.ltvnumbers.com/clickfunnels#add-funnels-as-a-batch)
        - [Page Source Funnels List](https://docs.ltvnumbers.com/clickfunnels#page-source-funnels-list)
        - [Upload Funnels List](https://docs.ltvnumbers.com/clickfunnels#upload-funnels-list)

---

# 1. Set Up Webhooks

Webhooks pull your sales data in real time and should be set up first before importing historical sales data to avoid gaps in your data

1. <a href="https://app.ltvnumbers.com" target="_blank">Log into LTV Numbers</a>
2. In LTV Numbers’ side navigation bar, go to the "Settings" tab 
3. Click the "Copy" button for your Webhook URL in the “Clickfunnels Integrations” section. This will be your webhook URL for all of your funnels
4. In a separate browser window or tab, <a href="https://app.clickfunnels.com/users/sign_in" target="_blank">log into Clickfunnels</a>
6. In Clickfunnels’ top navigation bar, go to Clickfunnels > Funnels
7. Click on a funnel you want to track to open it
8. Click on the "Settings" tab in the upper right
9. Scroll down to the "Webhooks" section and click "Manage Your Funnel Webhooks"
10. Click the "+ New Webhook" button
11. Enter the following information:
    - URL: paste your webhook URL that you copied earlier
    - Adapter: "json"
12. Click "Create Funnel Webhook" to create a webhook for this funnel
13. Repeat steps 5-11 for each funnel you want to track


# 2. Historical Sales Data

After setting up webhooks to pull in real time sales data, import your past sales for a complete picture of your data

### Export Historical Sales Data From Clickfunnels

1. In Clickfunnels’ top navigation bar, go to Clickfunnels > Sales
2. In the "Showing Sales For" date selector, choose "All Time"
3. Click the "Download Purchases" button. A popup with a progress bar will appear, indicating that Clickfunnels is preparing your historical sales data as a CSV file.
    - Note: this process may take some time to complete
4. To download your historical sales data, either:
    - Wait until the progress bar finishes, then click the "Download" button and save the CSV file to your computer
    - Check your email for the download link and save the CSV file to your computer

### Import Clickfunnels Historical Data Into LTV Numbers

1. In LTV Numbers' side menu, click "Upload" to get to the Data Uploader
2. Click the "Choose File" button
3. Select the historical sales data CSV from the previous section and click the "Next" button
4. In the "Choose Format" dropdown, select "Clickfunnels Sales CSV" and click the "Next" button then the "Upload" button to begin the ingest process
    - Note: this process may take some time to complete


# 3. Add Funnels

To finalize the connection between LTV Numbers and your funnels, you'll need to add them in LTV Numbers, individually or in a batch

### Add Funnels Individually

Use this simple method do add a few funnels, one at a time

1. In LTV Numbers’ side navigation bar, go to the "Settings" tab
2. Click the "Add Funnel" button in the "Clickfunnels Integrations" section
3. Enter the "Funnel Name" and "Funnel URL" for each funnel, both of which can be found in the funnel's Settings tab
    - The "Funnel Name" can be found in the "NAME" field and the "Funnel URL" can be found in the "Share This Funnel URL" field
 4. Repeat this process for each funnel 


### Add Funnels As A Batch

Use this advanced method to add several funnels all at once

##### Page Source Funnels List

1. In Clickfunnels’ top navigation bar, go to Clickfunnels > Funnels
2. Scroll to the bottom of the page and set the funnels per page to the maximum number
3. View the page source (right click > view page source or ctrl+u in Chrome-based browsers)
4. Copy the entire page source (ctrl+a, ctrl+c)
    - Note: The page source contains a list of your funnels displayed on this page
5. Paste the page source into a plain text editor such as Notepad or Visual Studio Code
6. Save the page source funnel list to your computer as an .html file
7. Repeat the above steps for each page of funnels in the "Funnels" page of your Clickfunnels account

##### Upload Funnels List 
1. In LTV Numbers' side menu, click "Upload" to get to the Data Uploader
2. Click the "Choose File" button
3. Select your page source funnel list html file and click the "Next" button
    - Note: You can multiselect all page source funnel list html files by ctrl+click-ing or clicking and dragging to highlight multiple files
4. In the "Choose Format" dropdown, select "Clickfunnels Funnels HTML" and click the "Next" button then the "Upload" button to begin the ingest process
