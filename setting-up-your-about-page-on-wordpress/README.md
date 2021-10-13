---
description: >-
  Most Open Food Network instances use a wordpress site for additional content
  and an 'About' page as this is quicker and easier for communications team
  members to add or change info
---

# Setting up your 'About' page on wordpress

### **HOW TO SET UP THE THEME ON YOUR SITE**

Please keep in mind that all these instructions are written by people who don’t do Wordpress work as their core business - if you know better ways to do something, please share them! Please add handy hints and instructions to this document as you find them (The #local-wordpress-sites channel in slack is the best place to alert people)\


We found that applying the theme to existing content didn’t work for us, which then meant pages needed to be recreated, which led to lots of confusing duplication! My advice would be to instead follow the steps outlined below. (But if you know a better way to apply the theme, please share it with the rest of us :) )\


1. Set up a subdomain where you want to build your new site, e.g. wp.openfoodnetwork.org.au 
2. Make sure your Wordpress is up to date
3. Download the zipped file for the theme: Divi: [Divi.zip](https://drive.google.com/open?id=1dPB4WWjiyZaHk3IE0ajCwrFZebvxQGlC)
4. Upload the Divi new Theme in Appearance -> Themes -> Add new. 
5. Activate the Divi theme in Wordpress
6. Access the Wordpress theme/content files in the Global GDrive:\
   [06 Communication -> Global Website -> DIVI_OFN\
   ](https://drive.google.com/drive/folders/1OQrrWU86c1j9xUA-dSMzNOiOl0vab7pi?usp=sharing)The files you need are:
   1. [Divi Customizer Settings.json](https://drive.google.com/open?id=1ldn_bc3gpzIKG_B\_4VDeD6HsNXbyB8Ww)
   2. [OFN Divi Theme.json](https://drive.google.com/open?id=1miEXYE8-5G7EJM7gms4PcPJS-ww0uatU)
   3. [openfoodnetwork…xml](https://drive.google.com/open?id=17WzNMGBX\_0tuulv9-ANStHejgJD2Cgfz)
7. Use the instructions at the bottom of [this article](https://amazingsystem.zendesk.com/hc/en-us/articles/115002832512-Export-Divi-site-to-another-host) to upload the theme customisation files.
8. Upload the file [Step 1 OFN Divi Customizer Settings.json](https://drive.google.com/open?id=1ldn_bc3gpzIKG_B\_4VDeD6HsNXbyB8Ww)
9. Upload the file [Step 2 OFN Divi Theme.json](https://drive.google.com/open?id=1miEXYE8-5G7EJM7gms4PcPJS-ww0uatU)
10. Upload the file [Step 3 openfoodnetwork…xml](https://drive.google.com/open?id=17WzNMGBX\_0tuulv9-ANStHejgJD2Cgfz)
11. Update all of your content
12. Use relative links in your content. For example, if you are linking within your Wordpress page, don’t enter [https://wp.openfoodnetwork.org.au/about](https://wp.openfoodnetwork.org.au/about) as link target but /about instead. Otherwise these links break when you move the site to another domain.
13. Put in place any redirects you need
14. Once your new site is ready, go to the Wordpress settings and change the domain name to the one you want to use, for example from wp.openfoodnetwork.org.au to about.openfoodnetwork.org.au.\
    Then point the domain about.openfoodnetwork.org.au to the IP address of the new server with your new Wordpress site.

There are instructions/recommendations of what to set up/check in terms of content + tips/tricks further down\
