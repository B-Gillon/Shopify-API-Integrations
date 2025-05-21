Orders.json gives you the ability to pull orders from Shopify.  There are two primary considerations here.

#1 - When you pull an order, the response will not include all the information necessary to fulfill the order.  You will need to use the order# to pull the associated fulfillment orders using fulfillment_orders.json.  This will give you everything you will need.
#2 - If Shopify is handling the order sourcing logice between fulfillment nodes, orders.json will not tell you which location should be fulfilling which part of the order.  This is not the only info you'll need to get from fulfillment_orders.json, but it's a significant part.
#3 - Shopify's RESTful APIs do not allow you to filter and only recive orders that are associated to a specific LocationID.  However, the GraphQL option can do this, which is one of many reasons why that is the preferred method.
