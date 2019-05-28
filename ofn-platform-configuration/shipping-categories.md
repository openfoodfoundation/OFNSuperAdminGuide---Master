# Shipping Categories

Shipping categories are used to help provide information that might be relevant during shipping. The primary motivation for the addition of shipping categories is to enable products to be labelled as ‘Temperature Controlled’, meaning they require refrigeration or heat. This can then be used to filter into reports.

Currently Shipping Categories is only used to denote ‘Temperature Controlled’ Items in specific reports. See Current Usage below for details.

**Use Case for Shipping Categories**    
A shipping category ‘Requires Refrigeration’ is added in the configuration. A product such as milk can then have this shipping category. Using the Delivery Report the delivery driver knows that an order has a refrigerated component helping them to remember to get this item from the fridge/cool box when dropping off the rest of the order.

**How to Use Shipping Categories**    
Configure “shipping categories” giving a relevant name and selecting ‘Temperature Controlled’ if relevant.

When you add a product, add the relevant “Shipping Category”. This will enable the property to filter through to reports where appropriate. This is a compulsory field. It was not compulsory before so lots of products have a Shipping Category names "default" that we used for data migration when we did the Spree upgrade to v.2.

![](../.gitbook/assets/shippingcategorynewproduct.png)

Shipping categories are also linked in shipping methods. When you create a shipping method you have to make sure you select all the shipping categories this method can cover. It you use cool boxes for instance in a regular truck, you can select all shipping categories when creating your shipping method. 

{% hint style="info" %}
If a product is associated to a shipping category, but the shipping method used by the customer for checkout doesn't include that shipping category, the customer won't be able to checkout !
{% endhint %}

**Current Usage**    
Use of the ‘Temperature Controlled’ field on a Shipping Category features in Order Cycle Management - Delivery Report and in the upcoming Packing Reports implemented for the UK team. It can be added to other reports if required.

