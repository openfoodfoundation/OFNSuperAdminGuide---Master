# How to set up events for tracking user behaviour - Mapping Matomo and code

As product managers / instance managers we would like to get a detailed understanding of how users are interacting with the product and more specifically with certain features.

Aside from tracking visits on specific pages, Matomo allows us also to track clickable elements (buttons, links) as well as errors occurring to understand how users are using the features and detect possible flaws in UX.

Setting up events can be tricky though, as defining an event on an element (like a button or an input field) can be **dependent on how it has been coded,** which differs across the product due to the lack of a styleguide (which is in progress :)).

Using the example of the implementing analytics for the new checkout process, this article explains how we are working to build a resuable methodology for Matomo.

#### **1. Matomo Setup**&#x20;

First, let´s have a look on how events are reported in Matomo. There are 3 hierarchies:

* Events Category
* Event Action&#x20;
* Event Name

For example under the category _alert_ we can differentiate between the event actions _success_ and _error._&#x20;

![](<../.gitbook/assets/image (14).png>)

The next sub-level are event _names_, where we can for example see the specific buttons that have been clicked during the checkout process.

![](<../.gitbook/assets/image (17).png>)

#### **2. How to create an event**

In order to track these interactions, both a trigger and a tag need to be defined within the tag manager.

A **tag** is a snippet of code which can be executed on your site, as soon as the condition of a connected **trigger** is met.

To create an functioning trigger on an element it is important to know how the element has been defined in the code**.** Along the work of the new checkout process we started creating a wiki on which element to be tracked how. See more details in [this issue](https://app.zenhub.com/workspaces/dev-pipe-54b840c6a249c8781446d4b2/issues/openfoodfoundation/openfoodnetwork/8214).



| Element                                                                                                                                                         | Code                                                                                                                                 | Matomo                             |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------- |
| ![Capture d’écran 2021-10-07 à 16 53 21](https://user-images.githubusercontent.com/296452/136409674-225eb0e8-aa76-4acf-bb0d-c4a899c11e26.png)Primary Button   | `<input type="submit" name="commit" value="Next - Payment method" class="button primary" data-disable-with="Next - Payment method">` | ClickClass contains `button`       |
| ![Capture d’écran 2021-10-07 à 16 55 56](https://user-images.githubusercontent.com/296452/136410125-d446f574-11bc-4759-bfd3-590c10e54531.png)Secondary Button | `<a class="button cancel" href="/cart"> Back to Edit basket </a>`                                                                    | ClickClass contains `button`       |
|                                                                                                                                                                 |                                                                                                                                      |                                    |
| ![Capture d’écran 2021-10-07 à 16 58 06](https://user-images.githubusercontent.com/296452/136410565-a9855683-57b9-4dc5-91d3-56c5455a61dd.png)ClickableTab     | `<div class="columns three text-center checkout-tab success">...</div>`                                                              | ClickClass contains `checkout-tab` |
| ![Capture d’écran 2021-10-07 à 16 59 24](https://user-images.githubusercontent.com/296452/136410798-07933f6b-e458-4279-87d6-4ad8b54f862e.png) Global Error    |                                                                                                                                      | ClickClass contains `alert-box`    |
| ![Capture d’écran 2021-10-07 à 17 00 33](https://user-images.githubusercontent.com/296452/136411029-1e9f3f1c-d763-4fe9-a34d-f68c1c2bec92.png)Form Error       | `<span class="formError standalone">Select a payment method</span>`                                                                  | ClickClass contains `formError`    |
| ![Capture d’écran 2021-10-07 à 17 01 49](https://user-images.githubusercontent.com/296452/136411250-aa50faa3-e320-46d2-97bd-b462ce7ccbd2.png) Link            | `<a class="summary-edit" href="/checkout/details">Edit your details</a>`                                                             | Click element equals `a`           |

**NOTE: This will only work, if elemnts have been coded in the same way!**

So for example, to track all button clicks along the checkout process, we define the trigger in the following way (under Matomo>Tag Manager>Trigger):

* _Page Path contains checkout_
* _Click Class contains button_&#x20;

&#x20;

![](<../.gitbook/assets/image (16).png>)

Then, a tag (or event) can be set up (under Matomo>Tag Manager>Tags)

![](<../.gitbook/assets/image (15).png>)

where in the bottom we select the previously created trigger that will execute the tag: ![](<../.gitbook/assets/image (13).png>)

_**Note: Once Triggers and Tags are defined, do not forget to publish the new version of Matomo tracking, otherwise the edits won´t go live.**_
