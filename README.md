1) Lookout for 'store.register' in index.js and replace the value of 'id' with your product ID
Make sure you the value of 'type' according to the type of InApp Product

2) Modify the 'alias' for each product as per the requirement. Make sure to search & replace the existing alias in the index.js file - as it is referenced inside the code. For eg, if you're going to replace the alias value '20 Coins' then ensure that you replace it at line 117 which reads as 'store.when("20 Coins").approved(function (order) {'

3) Inside index.html, there is a "div" wrapper with id - "in-app-purchase-list" where all the products are displayed.
Make sure that the ids of the inner div match that of the last part of the product id.

For instance - for product with id 'mahendra.demo.coins20' we have a div with id 'coins20-purchase'
The idea is to use the last part of the id (here - coins20) so that the id of the div inside html becomes "<last-part>-purchase"

4) In config.xml - can the id inside the 'widget' tag to match your bundleid / packagename. 

5) Replace the value of "BILLING_KEY" with the one for your app.

Here we pass the license key for the android application as parameter. The license key can be found from your PlayStore console. Go to your app on PlayStore, select it, then select "Services & APIs" and then go to "YOUR LICENSE KEY FOR THIS APPLICATION".


