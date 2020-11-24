# Creating a Matomo funnel to track a specific user journey on the platform

Use funnels if you want to track how users progress through the platform. This can be useful if you want to see something like how people use a particular entry page.

The Matomo Help pages can help you with any queries on how to set up funnels.

**Case study - Group page to checkout**

Here is an example of a funnel set-up from Australia to measure how many people are progressing to actually purchasing food through a particular entry point \(a group page\).  
\(I've used 'inverted commas' to denote a button/option in Matomo\)

1. **Set a goal.**  Go to your Matomo Dashboard Choose 'Manage goals' from the left menu options Click 'Add a New goal' at the bottom

![](../.gitbook/assets/image%20%288%29.png)

**2. Define the end point of your funnel.**  
In this case our end goal is for someone who has entered via a certain page to get to a successfully completed order.   
We set our goal name as 'Groups \(Pickup/Delivery\) to Checkout'  
We set our description as 'Landing on specific groups and then getting to a successful checkout' \(this is so you understand what you're measuring\)   
The goal is triggered 'when visitors' 'send an event'  
Where the 'Event name' 'contains' Your order has been processed successfully \(we chose that text as reliable within our set-up, you'll need to confirm your text for that example\)  
We allowed goal to be converted more than once per visit

**3. Configure your funnel**  
This sets the specific path you want to measure, and you need to set each step. For our funnel we used a mix of path commands \(what's in the URL\) and page title commands \(where the title is always the same but the URL is user-specific\)  
Our path was:   


![](../.gitbook/assets/image%20%287%29.png)

Step 1 Group pickup delivery - 'Path contains' groups/pickup-delivery \(this means we're measuring people who come via the specific groups page we set up and are trying to measure\)  
Step 2 Shop - 'path contains' /shop \(they have made it to a URL with /shop i.e. to a shop on the platform\)  
Step 3 Checkout - 'path contains' /checkout \(they have made it to a URL with /checkout i.e. a shop checkout on the platform\)  
Step 4 Order confirmation - 'Page title contains' Order Confirmation \(they have made it to a confirmed order with a unique to the transaction URL, which is why we have chosen a page title rather than path\)  
Step 5 Completed - 'Converts goal' for the funnel we've already set up \(why it's important to get your end goal for the funnel right\)

You can then validate your funnel to make sure it's working properly. 

