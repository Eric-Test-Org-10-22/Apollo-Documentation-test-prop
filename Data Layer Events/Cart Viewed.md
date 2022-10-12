# Cart Viewed

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Cart Viewed",
    "cart": {
        "cartID": "<cartID>",
        "item": [
            {
                "price": {
                    "isHidden": <isHidden>,
                    "priceTier": "<priceTier>",
                    "priceType": "<priceType>"
                },
                "productInfo": {
                    "brand": "<brand>",
                    "color": "<color>",
                    "isBackOrdered": <isBackOrdered>,
                    "isOutOfStock": <isOutOfStock>,
                    "name": "<name>",
                    "productID": "<productID>",
                    "productLine": "<productLine>",
                    "sku": "<sku>",
                    "trademarkedTechnology": "<trademarkedTechnology>"
                }
            }
        ]
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|cart.cartID|string|Back-end identifier for a shopping cart|12345, 435678, 34567, XCV456, XCV876|||||||
|cart.item[n].price.isHidden|integer|Count of times the price of a product was hidden in the cart due to MAP \(Minimum Advertised Pricing\) requirements.   Set in the product string for only those products where it is applicable, with a value of 1||||||||
|cart.item[n].price.priceTier|string|Describes the general pricing tier of a product. \(Good, Better, Best\)|Good, Better, Best, Bronze, Silver, Gold|||||||
|cart.item[n].price.priceType|string|Describes the type of price offered using commonly used terms. |1st mark, 2nd mark, 3rd mark, clearance, sale, doorbuster|||||||
|cart.item[n].productInfo.brand|string|Describes the brand of a product or offering.|Ford, Chevrolet, Dodge, Levis, Columbia, Patagonia|||||||
|cart.item[n].productInfo.color|string|Describes the colorway of a product or product variant|Antique Oak, Granite, Black Marble, Knotty Pine|||||||
|cart.item[n].productInfo.isBackOrdered|boolean|Boolean flag indicating that an inventoried product is on backorder|TRUE, FALSE|||||||
|cart.item[n].productInfo.isOutOfStock|integer|Count of times a product was out of stock at the time of cart view.||||||||
|cart.item[n].productInfo.name|string|Name of the product or offering.  Should be unique and 1:1 with productID|Oceana, Corsica, Flame Tech, Air Jordan 88|||||||
|cart.item[n].productInfo.productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|cart.item[n].productInfo.productLine|string|Describes the product Line of a product. |Laminate Wood, Vinyl, Hardwood, Stone, Ceramic|||||||
|cart.item[n].productInfo.sku|string|Stock Keeping Unit \(SKU\) Unique Identifier of specific item \(typically\) held in inventory.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level below productID for products with SKU variants. |34567890, 4567890, 00155-large-cornflower|||||||
|cart.item[n].productInfo.trademarkedTechnology|string|Describes trademarks and\/or technical branding used to describe the product|Stainmaster, GoreTex, WeatherShield|||||||




