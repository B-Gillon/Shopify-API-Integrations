A location is a fulfillment node - warehouse, store, kiosk, etc. - anywhere that will house inventory that should be exposed to the webstore.  In order to post a locaton's inventory for a product to Shopify, that product must first be associated to the location.

***This assumes Shopify is handling any required order sourcing logic.  If that is being handled by the 3PL, Shopify will only have a single LocationID value that represents the entire 3Pl.  This is expected, as Shopify will maintain a single On Hand Qty inventory value for the 3PL.

<b>Retrieve</b> - Ability to GET a list of locations in the Shopify webstore
<b>Connect</b> - Allows you to connect a product to a location, one location at a time.
<b>Disconnect</b> - Allows you to disconnect a product from a location, one location at a time.  This would make sense if an product will no longer be shipping from a location.
