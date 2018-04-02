# Why we need different formats for invoices?

Each country has its own rules regarding what information should be displayed on an invoice.

There are two possible format for invoices today:
- **the Australian format which is the default format when you deploy the OFN**. This comprises a detail for each line of the price (including OR excluding tax depending on instance set up "prices include tax or not") + the collected tax amount for this line. But the rate applied is not displayed.

![](/assets/Screenshot from 2018-04-02 11-49-41.png)

- **a format that fit more French / European requirements regarding how invoices should look like**. This comprises a detail for each line of the price excluding and including tax and tax rate applied + a total for the order excluding and including tax and the total tax amount per tax rate that the enterprise need to report to fiscal administration (so if in the order there are items with different tax rates there will be two "total tax" lines in the totals).
This option also enable the hub to add some custom text on his hub's invoices (this is done in enterprise setting menu).

![](/assets/Screenshot from 2018-04-02 11-50-30.png)


# Give your users the possibility to print a receipt

Some hubs are using and OFN instance to manage onsite sales and needed to be able to print a receipt. So it is possible as an instance manager to enable that usage on your instance.
The receipt format shows each line item and display clearly the amount excluding and including VAT.


# How to set up the alternative invoice format and receipt?

Go to **Configuration > Invoice setting**
![](/assets/Screenshot from 2018-04-02 11-44-29.png)