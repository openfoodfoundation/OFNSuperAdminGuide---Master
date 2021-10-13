# Integrate OFN with Mailchimp

You might want integrate OFN with Mailchimp for two main reasons:

* You want to propose any new user on your local OFN instance to register to your local newsletter
* Or you want to enable a food hub to integrate their customer list with their own Mailchimp account, so they can manage their newsletter, order cycle mailings, etc. easily.

Today you can use Zapier to establish this kind of integrations. We want to improve it later on with cleaner solution, but for now it does the job !

## Requirements

* Premium Zapier account (ask on the Zappiness slack channel for more details)
* PostgresDB connection in Zapier

## Feed any new customer of hub into the Mailchimp audience of that hub

**What you want is :** When there is a new order, you want the name and email of the customer to be added to the Mailchimp audience list of the hub.

#### The trigger

* Select as a trigger : PostgreSQL

![](<../.gitbook/assets/Capture du 2019-05-28 18-01-37.png>)

You want the trigger to be : when an order is made by a new customer in the hub's shop. So for that Zapier will need to read in the OFN database, which is a PostgreSQL type database.

* Then you will choose "new row" as you want to check when there is a new order (a new row/line in the database in the orders table) if the customer id is new or not.

![](<../.gitbook/assets/Capture du 2019-05-28 18-02-26.png>)

* Select the PostgreSQL database you have previously connected

![](<../.gitbook/assets/Capture du 2019-05-28 18-04-01.png>)

* Then enter the query that will look for the info you want in the database. You can ask on Zappiness Slack channel if you don't know how to do that !

![](<../.gitbook/assets/Capture du 2019-05-28 18-05-38.png>)

In this case the query is :

```
select spree_addresses.firstname, spree_orders.email from spree_addresses, spree_orders where spree_orders.bill_address_id = spree_addresses.id  and state = 'complete' and distributor_id = xxx
```

#### The action

What you want now is to describe what you want to happen when the trigger happens. Here, you want that new customer email to be added to the Mailchimp audience of the hub.

* Choose Mailchimp as the app to use in the action section

![](<../.gitbook/assets/Capture du 2019-05-28 18-25-07.png>)

* Then choose "add/update subscriber

![](<../.gitbook/assets/Capture du 2019-05-28 18-23-47.png>)

* You are then asked to connect an account, fill in the username and password for the Mailchimp account you want to connect. The user needs to have requested you to make that integration and provide the credentials by any secure media (phone recommended).

![](<../.gitbook/assets/Capture du 2019-05-28 18-26-53.png>)

* You then have some options to setup on what you want to happen on Mailchimp side. You will select the Mailchimp audience that you want the new customer to be added to. 

![](<../.gitbook/assets/Capture du 2019-05-28 18-34-42 (1).png>)

\[to be completed]
