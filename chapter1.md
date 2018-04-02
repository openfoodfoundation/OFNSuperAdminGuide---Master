# Configuration - General Settings

When you're logged in as super-admin, click on 'configuration' in the top blue menu.![](/assets/import.png)

Check:

* Site name e.g. Open Food Network MyCountry
* Default meta keywords e.g. OFN open food
* Default meta description e.g. OFN Australia 
* Site URL e.g. openfoodnetwork.org.au

Then scroll down to see a range of other settings. Emulate tick boxes as in image below or vary if obvious for your instance e.g. currency.

![](/assets/config-generalsettings2.png)

## Terms of Service



## Embedded shopfront settings

* [the User Guide for enterprises using embedded shopfronts is here](https://www.gitbook.com/book/ofn-user-guide/ofn-super-admin-guide/edit#). Tick this box and add domains in the box to allow particular enterprises to use it. \[checking if there is anything particular about the separator\]

## Number localisation settings



Mail

* Will be set up already

\*\*Image Setting\*\*

* Will be set up already

\*\*Tax categories, tax rates, tax settings\*\*

* Create your tax categories in 'tax categories'. This is just the name of the categories.

* In 'tax rate' you can apply the calculator to the 'tax categories' you have created.

* In tax settings, you can select if the tax selection is compulsory, if it is applied to shipping and billing

For your reference, the image below shows Australia's flat rate 10% tax in 'tax rate'

&lt;img src="/uploads/default/original/1X/21a143fd7f2a466b07dcdaea8be00d78c562dcf5.png" width="639" height="500"&gt;

\*\*Zones, Countries States\*\*

* \*\*Payment Methods\*\*

* Allow users to create their own payment methods. Don't need to do anything as super-admin.

\#\#Taxonomies

You need to have product categories set-up before you can start creating products, as every Product must have a product category.

&gt;=&gt; \*Configuration / Taxonomies\*

Any taxonomies, and entries within them, that you create will become available as Product Categories to attach to products. We HIGHLY recommend that you keep them high-level . . these product categories will become the filters at the top of your list views and shop-front and you do not want too many in use across your site

&lt;img src="/uploads/default/136/caae7c73e8e7edce.png" width="331" height="120"&gt;

You can attach icons to product categories

\*\*Shipping methods\*

\*\*shipping categories\*\*

* This is where you can create optional shipping categories to be applied to products. Such as 'refrigerated'. Any categories created here can be applied to products when you start creating products.

\*\*Inventory settings\*\*

* In Australia neither of these options are selected.

\*\*Analytics tracker.\*\*

* You can install an analytics tracker here. Non-essential.

\*\*CMS Admin\*\*

* This tab is no longer active. Ignore.

\*\*Enterprise Fees\*\*

* Super-admin can ignore this tab. Enterprises should create their own enterprise fees.

\*\*Content\*\*

This is where you can customise some pages. See further instrcutions here... \[\[\[[http://community.openfoodnetwork.org/t/configuration-content/307\]\[1\]\(http://community.openfoodnetwork.org/t/configuration-content/307\]\[1\)\]\(http://community.openfoodnetwork.org/t/configuration-content/307\]\[1\]\(http://community.openfoodnetwork.org/t/configuration-content/307\]\[1\)\)\](http://community.openfoodnetwork.org/t/configuration-content/307][1]%28http://community.openfoodnetwork.org/t/configuration-content/307][1%29]%28http://community.openfoodnetwork.org/t/configuration-content/307][1]%28http://community.openfoodnetwork.org/t/configuration-content/307][1%29%29\)\]

\*\*Accounts and Billing\*\*

* This is where you can set-up billing. This is billing from the OFN to enterprises for the use of the software. \[\[\[[http://community.openfoodnetwork.org/t/enterprise-user-accounts-configuration-accounts-billing/348\]\[2\]\(http://community.openfoodnetwork.org/t/enterprise-user-accounts-configuration-accounts-billing/348\]\[2\)\]\(http://community.openfoodnetwork.org/t/enterprise-user-accounts-configuration-accounts-billing/348\]\[2\]\(http://community.openfoodnetwork.org/t/enterprise-user-accounts-configuration-accounts-billing/348\]\[2\)\)\](http://community.openfoodnetwork.org/t/enterprise-user-accounts-configuration-accounts-billing/348][2]%28http://community.openfoodnetwork.org/t/enterprise-user-accounts-configuration-accounts-billing/348][2%29]%28http://community.openfoodnetwork.org/t/enterprise-user-accounts-configuration-accounts-billing/348][2]%28http://community.openfoodnetwork.org/t/enterprise-user-accounts-configuration-accounts-billing/348][2%29%29\)\]

\#\#Producer and Product Properties

Read more details on \[how these work\]\[3\] and the \[kind of things\]\[4\] to set them to. The Australian set are shown below - these are the options enterprise users can choose from

&lt;img src="/uploads/default/137/b34469bab89b3f93.png" width="613" height="500"&gt;

To set up, go to

&gt;=&gt; \*Products / Properties\*

BE CAREFUL: on the product page, when you add properties to a product through your super-admin account, you are not proposed the existing list of properties, you have to start typing for a suggestion to appear, and you are not blocked if you write a new property, which will be added to the whole properties list... so there is a high risk of creating duplicates, that then will be proposed in the general list and generate confusion! So the easiest way to avoid mistakes is to always use a regular "user account" when working on tasks related to hubs and products administration. Don't add products when using your super-admin account ;-\)

&lt;img src="/uploads/default/original/1X/c44edc352206207663cbd586d1ef1f4175c550db.jpg" width="690" height="350"&gt;

\#\#Users

You will have a super-admin user. We recommend that you create some Enterprise Users to start setting up, especially if you're setting up Hubs \(read more about Users \[here\]\[5\]. Getting your Users and Enterprises right will save a lot of manual fiddling around later.

e.g.

* Create a User \(click users in the blue menu, then new user\)

  * set their \# of allowed Enterprises to &gt;1 \(e.g. 10\)

  * if you click the 'admin' box, it will give this user super-admin permission. Create some non super admin users.

* Create an Enterprise \(click enterprises, + new enterprise\)

  * Once you have created a users, you can make them the owner of this new enterprise.

  * set type Any to make it a Hub \(read more about \[Enterprise Types\]\[6\]\) and \[how to manage them\]\([http://community.openfoodnetwork.org/t/managing-enterprises/166\](http://community.openfoodnetwork.org/t/managing-enterprises/166%29\)

* Login as that new User

  * now creating additional Producers and Hubs will automatically link these new Enterprises to your first Hub. \[more about auto-E2E-links\]\([http://community.openfoodnetwork.org/t/what-e2e-links-do-new-enterprises-have/33\](http://community.openfoodnetwork.org/t/what-e2e-links-do-new-enterprises-have/33%29\)

\#Input Data

\#\#Enterprises

\*\*\*NB. You MUST complete the email validation from enterprise confirmation emails. These are sent to the nominated contact email for an enterprise, and the enterprise will not be visible or useable in an Order Cycle until that email has been verified.\*\*\*

NOW you are ready to start building up your working enterprises!

1. Create Producers

   * profiles

   * products and variants

2. Create Hubs

   * make sure you create shipping and payment methods to make these valid

3. Order Cycles

\#Keep smiling :-\)

This initial configuration can be a bit painful: you are not yet used to the interface, and there can be some bugs also in this "super admin zone". It's better to prepare the informations you want to put in before entering them \(categories and properties\) to avoid multiple modifications. If you experience a bug, try in another browser, that may work better!

\[1\]: [http://community.openfoodnetwork.org/t/configuration-content/307](http://community.openfoodnetwork.org/t/configuration-content/307)

\[2\]: [http://community.openfoodnetwork.org/t/enterprise-user-accounts-configuration-accounts-billing/348](http://community.openfoodnetwork.org/t/enterprise-user-accounts-configuration-accounts-billing/348)

\[3\]: [http://community.openfoodnetwork.org/t/properties-of-enterprises-and-product-variants-e-g-organic-certified/50](http://community.openfoodnetwork.org/t/properties-of-enterprises-and-product-variants-e-g-organic-certified/50)

\[4\]: [http://community.openfoodnetwork.org/t/what-product-properties-should-ofn-aus-support/57](http://community.openfoodnetwork.org/t/what-product-properties-should-ofn-aus-support/57)

\[5\]: [http://community.openfoodnetwork.org/t/users-and-enterprise-types/152](http://community.openfoodnetwork.org/t/users-and-enterprise-types/152)

\[6\]: [http://community.openfoodnetwork.org/t/users-and-enterprise-types/152/1](http://community.openfoodnetwork.org/t/users-and-enterprise-types/152/1)

