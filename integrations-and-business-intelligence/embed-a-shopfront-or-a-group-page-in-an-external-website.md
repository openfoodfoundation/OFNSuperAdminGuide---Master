# Embed a shopfront or a group page in an external website

This feature lets users who have OFN shopfronts embed their shop and/or group into their own website. This gives customers a more fluid experience and avoids the need to redirect them between multiple websites. It also allows users to retain some of their visual branding in the shop. When you embed your OFN shop in your own site, your OFN base shop will remain, so customers can choose where they want to shop. [The User Guide for enterprises using embedded shopfronts is here](https://ofn-user-guide.gitbooks.io/ofn-user-guide-master/content/embedded-shopfronts.html).

If a user ask you for this feature, you need to add their domain in the whitelist of domains, in [General Settings](../ofn-platform-configuration/general-settings.md). Then they have one line of code to integrate in their website.

This feature is very limited and we know has the following limitations :

* It is not properly functional on mobile. Especially on mac tablets and phone, it's impossible to scroll the list of products in a shop, so it's basically impossible to shop.
* Also the UX can be a bit confusing, especially if a login is requested. There is no "single sign on" the user will need to create an account and login on the OFN website within the host website, which can be a bit confusing in term of UX.
* And there is no possibility to customize the visual aspect of the integrated shop in the external website, so it's not always easy to make it looks good.

We hope when we move forward on documenting and cleaning the OFN API that we can move toward some other mùore efficient solutions like widgets or plugins. Stay tuned !

