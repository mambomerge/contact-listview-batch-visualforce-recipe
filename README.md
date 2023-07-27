# contact-listview-batch-visualforce-recipe

This recipe will step you through creating a button for Contact List Views to generate a single docx file per selected record.

Mambo Merge Version 1.25.0 introduce Bulk and Batch functionality as built-in Pro Edition Features(Using Flows). Check out our <a href="https://www.mambomerge.com/support/">Support Page</a>  and <a href="https://www.youtube.com/@mambomerge">Youtube channel</a> for the latest features. 

## Instructions
1. Install Mambo Merge from the AppExchange by following these instructions: https://www.mambomerge.com/support/installation-from-appexchange/

2. Use the below button to deploy this repo to your Salesforce to create a new Visualforce Page, new Aura App, and new Contact List View Button
<a href="https://githubsfdeploy.herokuapp.com?owner=mambomerge&repo=contact-listview-batch-visualforce-recipe&ref=main">
  <img alt="Deploy to Salesforce"
       src="https://raw.githubusercontent.com/afawcett/githubsfdeploy/master/deploy.png">
</a>

3. Edit your lightning page to include Mambo Merge by following these instructions: https://www.mambomerge.com/support/editing-lightning-pages/

4. Upload your docx Template onto the Files tab by following these instructions: https://www.mambomerge.com/support/how-to-use-mambo-merge-to-generate-a-new-word-docx-file-drag-and-drop-copy/

5. Create a new Mambo Merge Configuration with Id **ContactListViewBatch** as follows:

  * 5a. Click on the down arrow in the top right corner of Mambo Merge and choose Setup

  * 5b. Create a new Single Record Configuration. 

  * 5c. Add a new Template to the configuration.

  * 5d. Save the Configuration. Don't forget to save Configuration Id as **ContactListViewBatch**

6. Create a new Custom Button for List Views on the Contact Object that uses the **ContactListViewBatchMamboMerge** page

  * 6a. Go to Buttons, Links, and Actions. 

  * 6b. Click **New Button or Link**.

  * 6c. Select Display Type **List Button** with Display Checkboxes (for Multi-Record Selection). 

  * 6d. Select **Visualforce Page** for Content Source. Content should be set to **ContactListViewBatchMamboMerge** page. 

7. Go to List View Button layout to add the new button.
