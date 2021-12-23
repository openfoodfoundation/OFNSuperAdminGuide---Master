# Create a segment to analyze behaviour in Admin

Since Matomo tracking is now also enabled for the Admin, we can separate back office visits from shopfront visits by **creating a segment that includes all visits of **_**/admin**_** pages.**

**Note:** this is not a segment grouping all Admin users but all visits of pages in /admin.

**Why is this different?**

We **cannot** (yet) separate

* Admin users, that visited the shopfront vs.
* shoppers that visited the shopfront

(For this the Tag Manager Data Layer needs to be implemented, to differentiate between users)

We **can track Admin user behavior though when they visit the /admin pages**, for example **analyzing**&#x20;

* which devices are used
* which pages are visited
* create funnels
* what actions are performed etc.

### **How to create the Admin Visits segment?**

1. Go to your Dashboard
2. Choose “Add new Segment” in the Top Menu Visits Filter

![](<../.gitbook/assets/image (10).png>)

3\. Name your Segment (preferably ADMIN to have it consistent across all instances ;))

![](<../.gitbook/assets/image (11).png>)

4\. Select Category (per default it is Acquisition Date) **Action > Page URL** from Dropdown

5\. Select **“Contains”**

6\. Enter **/admin** for value

7\. Click **“Save and apply”**

It may take a few hours until data is available for the segment, so if you check immediately there won’t be any results - but it will work backwards, i.e. track data from prior than segment was created.

### Use Case 1: Track Device Usage

1\.  Go to your Dashboard&#x20;

2\. Select **Visitors > Devices** from Sidebar Menu&#x20;

3\. Select **ADMIN** segment in top menu visits filter

![](<../.gitbook/assets/image (12).png>)

