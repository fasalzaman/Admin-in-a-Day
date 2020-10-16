# Admin in a day

# Module 2: Reporting and Telemetry

# Hands on lab

# Lab Scenario

In this Hands-on Lab, you are an administrator for Contoso helping adopt the Power Platform.

An important part of keeping the Power Platform running successfully is monitoring the ongoing usage. In this hands-on lab you will be using the platform tools and the CoE Starter Kit to perform usage monitoring.

# Lab Requirements

## Lab Test Environment

This hands-on lab is designed to be completed in an environment setup for multiple students to complete the Admin in a day series of hands on labs.

You need to use the assigned user and environment information to complete this lab. You must have completed the prior labs to successfully complete this lab.

# Exercise 1: Explore the CoE Starter Kit

## Scenario

In this exercise, you will explore some of the apps and analytics that are part of the Power Platform CoE Starter Kit.  We have already installed and configured the starter kit into the tenant you are using for this lab.  As part of configuring we imported the solution, shared the apps, configured the flows that synchronize data and published the Power BI report.  If you were doing this in your own tenant, you would follow the instructions to complete these steps.

Now in this exercise, you will explore the following key components

-	Power Platform Admin View app
-	Power BI Dashboard
-	The business process that is used by the Developer Compliance process

### Task 1: Explore the Power Platform Admin View app

1.	Navigate to https://make.powerapps.com 

2.	Select **Power Platform CoE** environment in the environment selector.

 ![](Images%20MOD_2/img01.png)

4.	Click on Environments in the left navigation.  This will show you a list of all the environments in your tenant and key metrics like number of apps. Select any of the environment and review the details

![](Images%20MOD_2/image%206.png)

5.	Click on the Makers link in the left navigation, this shows you all the people that have built apps in your company

6.	Click on one of the Makers and explore the detail form. 

### Task 2: Power BI Dashboard

1.	Navigate in your browser to Power BI https://www.powerbi.com and click Sign in with your lab credentials.

2.	When you see the You have an account with us, click Sign In again and then click Start. 

![](Images%20MOD_2/image%209.png)

3.	When prompted to Invite more people, click Skip.

4.	On the left side navigation click Workspaces and then Create a workspace.  We are going to use this workspace to publish our report to from Power BI Desktop.  This would allow you to view it from PowerBI.com, the mobile app, or even embed it in other places like Microsoft Teams.  The workspace can also be shared with others so they can see the analytics.

![](Images%20MOD_2/image%2010.png)

5.	When prompted click Try Pro for free.  

![](Images%20MOD_2/image%2011.png)

6.	After the trial is started, you will have to re-navigate to Workspaces and then Create a workspace

7.	On the Create panel, provide a unique name like CoE and your lab admin user number.

![](Images%20MOD_2/image%2012.png)

8.	Launch Power BI Desktop on your local computer, if you don’t have it installed you can install it from here https://powerbi.microsoft.com/en-us/desktop/ 

9.	Click Sign-in and provide your lab admin account credentials

![](Images%20MOD_2/image%2013.png)

10.	Once signed in, click File, open report, and select Browse Reports

![](Images%20MOD_2/image%2014.png)

Now, Click [here](https://fasalspektrastorage.blob.core.windows.net/admin-in-a-day/Dashboard-PowerPlatformAdminDashboard-2020-10-13.pbit) to download Dashboard-PowerPlatformAdminDashboard file 

11.	Locate the folder containing lab files you downloaded and select the Dashboard-PowerPlatformAdminDashboard file

![](Images%20MOD_2/image%2015.png)

12.	The file should load and you should see the Overview page loaded with some data from a test environment, this data is more interesting than the lab tenant, so we are going to explore a few things and then change the data source to point to your lab environment and then publish it to PowerBI.com

![](Images%20MOD_2/image%2016.png)

13.	Review this overview page, notice it gives a good high-level look at our tenant activity. If you have multiple locations, it will quickly highlight which users are more engaged with building apps.  You can also quickly see which environments are most active.

14.	Click through each page using the navigation at the bottom of the app and review the insights available.

![](Images%20MOD_2/image%2017.png)

15.	On the Environments page, use the date slider and see how it effects the other data on the page.  When you are done leave it set at the max date range

![](Images%20MOD_2/imagen18.png)

16.	On the Apps page notice the Creation Trend, this is a good way to watch adoption progress.

![](Images%20MOD_2/image%2019.png)

17.	Click through the other pages and review the data available.

18.	Next, we are going to change the data source to point to your lab environment, in another browser tab, navigate to Power Platform Admin Center https://aka.ms/ppac and select Environments.

19.	Locate the Power Platform COE environment and click on the name to show the details page .

20.	Right click on the Environment URL and select Copy link.

![](Images%20MOD_2/image%2020.png)

21.	Back in Power BI Desktop click Transform data and select Edit parameters

![](Images%20MOD_2/img76.png)

22.	In the OrgUrl parameter paste in the value you copied from the environment details page and click OK.

![](Images%20MOD_2/image%2021.png)

23.	Just below the command bar, you should now see that there are pending changes, Click Apply Changes.

![](Images%20MOD_2/image%2022.png)

24.	You will be prompted to sign in, use your lab admin account and then click Connect.

![](Images%20MOD_2/img77.png)

25.	Wait for the query changes to be applied. Briefly look at the pages again, notice the data is different.

26.	From the File menu click Save.

27.	Click Publish and publish the report to Power BI.

28.	Navigate to https://PowerBI.com 

29.	Click on Workspaces and CoE Workspace

30.	Select the Reports tab and click on Dashboard-PowerPlatform.. to open the report.

![](Images%20MOD_2/image%2023.png)

31.	Select the Environments page. Use the Date slider to ensure the date range includes the last month.

![](Images%20MOD_2/image%2024.png)

32.	You have now successfully deployed the Power BI reports that come with the CoE starter kit.  

# Exercise 2: Get notification of new apps, flows and connectors

## Scenario

In this exercise, you will be using one of the pre-built Power Automate templates that run on a schedule and looks for newly created canvas apps, flows and connectors and sends you an email.

### Task 1: Create the flow from the template

1.	Navigate to https://flow.microsoft.com and sign in.

2.	Make sure **Power Platform COE** environment is selected.  Note: This environment is where the CoE starter kit is installed and is intended to be our dedicated admin environment.  Even if you don’t use the starter kit, having a dedicated admin environment can be helpful.

![](Images%20MOD_2/image%2025.png)

3.	Paste the URL and press enter. https://us.flow.microsoft.com/en-us/galleries/public/templates/0b2ffb0174724ad6b4681728c0f53062/get-list-of-new-powerapps-flows-and-connectors/ 

4.	**Click Sign in.**

![](Images%20MOD_2/image%2026.png)

5.	Select the user you are signed in as.

6.	Click **Accept.**

![](Images%20MOD_2/image%2027.png)

7.	Click sign in for each of the rest of the connectors.

8.	Click **Continue.**

![](Images%20MOD_2/image%2028.png)

8.	Examine the flow steps and then click **Flow Checker.**

![](Images%20MOD_2/image%2029.png)

9.	There should be no errors.

10.	Click **Save.**

11.	Click on the back arrow.

![](Images%20MOD_2/image%2030.png)

12.	The flow should have one run in progress.

![](Images%20MOD_2/image%2031.png)

13.	Wait for the flow to complete and then click to open the run. You can refresh to see the updated status of the flow.

![](Images%20MOD_2/image%2032.png)

14.	Examine the flow run.

![](Images%20MOD_2/image%2033.png)

15.	Click **App** launcher and select **Outlook.**

![](Images%20MOD_2/image%2034.png)

16.	Navigate to https://outlook.office.com/ 

17.	You should get an email from the flow. Open the email.

![](Images%20MOD_2/image%2035.png)

17.	The report should list flows, power apps, connectors in tables.

![](Images%20MOD_2/image%2036.png)

# Exercise 3: Review tenant audit logs (Optional if you have time)

## Scenario

All other auditing of Power Apps and Power Automate flows (other than CDS data modification) are viewed through the Office 365 Security and Compliance site.

Prior to use, this must be enabled by a global tenant administrator using these instructions. In the tenant you are using we have already completed that for you as well as granting you permission to view the audit log data for the tenant. That was done using the PowerShell command Add-RoleGroupMember “Compliance Management” -Member your user.

In this exercise, you will be using the log search and alert tools to work with the audit data.

### Task 1: Review audit logging in the environment

1.	Navigate to https://Protection.office.com 

2.	Expand **Search.**

3.	Select **Audit log search.**

![](Images%20MOD_2/image%2037.png)

4.	Click **Search** using the default search criteria.

![](Images%20MOD_2/image%2038.png)

5.	Review the items displayed; drill into a few of them to see the type of data available.

6.	Click **Export Results**. You can download the data if you like. Using export, you can open the data in other tools for analysis

![](Images%20MOD_2/image%2039.png)

7.	Click on the **Activities** dropdown.

![](Images%20MOD_2/image%2040.png)

8.	Select all Power Apps, Power Automate and Dynamics 365 activities. Click on the section names to select all.

9.	Click Search again.

10.	Review the results.

11.	Look for an activity of Edited Flow, click on the item to open up the detail. Click on the More info, and review what data is provided.

12.	A common task is to look at all activity for a particular user. Copy the user from this Edited flow activity and go back to the search criteria.

13.	Paste the user you copied into the Users filter and click search again. Now you are looking at all the activity for a single user.

14.	You can also click on the filter results in the upper right corner. This will expose filters just below the headers in the table.

15.	Try clicking on an item to view detail. Copy the Item field and then go back to the list and click the filter results. Paste the item info you just copied into the filed. The results list will now only show activities related to that item. For example, you could use this to show all activities for a specific flow.

# Terms of Use

© 2020 Microsoft Corporation. All rights reserved.

By using this demo/lab, you agree to the following terms: The technology/functionality described in this demo/lab is provided by Microsoft Corporation for purposes of obtaining your feedback and to provide you with a learning experience. You may only use the demo/lab to evaluate such technology features and functionality and provide feedback to Microsoft. You may not use it for any other purpose. You may not modify, copy, distribute, transmit, display, perform, reproduce, publish, license, create derivative works from, transfer, or sell this demo/lab or any portion thereof. COPYING OR REPRODUCTION OF THE DEMO/LAB (OR ANY PORTION OF IT) TO ANY OTHER SERVER OR LOCATION FOR FURTHER REPRODUCTION OR REDISTRIBUTION IS EXPRESSLY PROHIBITED. THIS DEMO/LAB PROVIDES CERTAIN SOFTWARE TECHNOLOGY/PRODUCT FEATURES AND FUNCTIONALITY, INCLUDING POTENTIAL NEW FEATURES AND CONCEPTS, IN A SIMULATED ENVIRONMENT WITHOUT COMPLEX SET-UP OR INSTALLATION FOR THE PURPOSE DESCRIBED ABOVE. THE TECHNOLOGY/CONCEPTS REPRESENTED IN THIS DEMO/LAB MAY NOT REPRESENT FULL FEATURE FUNCTIONALITY AND MAY NOT WORK THE WAY A FINAL VERSION MAY WORK. WE ALSO MAY NOT RELEASE A FINAL VERSION OF SUCH FEATURES OR CONCEPTS. YOUR EXPERIENCE WITH USING SUCH FEATURES AND FUNCTIONALITY IN A PHYSICAL ENVIRONMENT MAY ALSO BE DIFFERENT.

## FEEDBACK

If you give feedback about the technology features, functionality and/or concepts described in this demo/lab to Microsoft, you give to Microsoft, without charge, the right to use, share and commercialize your feedback in any way and for any purpose. You also give to third parties, without charge, any patent rights needed for their products, technologies and services to use or interface with any specific parts of a Microsoft software or service that includes the feedback. You will not give feedback that is subject to a license that requires Microsoft to license its software or documentation to third parties because we include your feedback in them. These rights survive this agreement. MICROSOFT CORPORATION HEREBY DISCLAIMS ALL WARRANTIES AND CONDITIONS WITH REGARD TO THE DEMO/LAB, INCLUDING ALL WARRANTIES AND CONDITIONS OF MERCHANTABILITY, WHETHER EXPRESS, IMPLIED OR STATUTORY, FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. MICROSOFT DOES NOT MAKE ANY ASSURANCES OR REPRESENTATIONS WITH REGARD TO THE ACCURACY OF THE RESULTS, OUTPUT THAT DERIVES FROM USE OF DEMO/ LAB, OR SUITABILITY OF THE INFORMATION CONTAINED IN THE DEMO/LAB FOR ANY PURPOSE.

## DISCLAIMER

This demo/lab contains only a portion of new features and enhancements in Microsoft PowerApps. Some of the features might change in future releases of the product. In this demo/lab, you will learn about some, but not all, new features.






























 

 
 


