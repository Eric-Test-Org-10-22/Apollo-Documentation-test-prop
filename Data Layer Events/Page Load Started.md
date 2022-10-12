# Page Load Started

### Page Load Started is part of the page load sequence, including virtual page loads in the case of single page apps, and must be the first event pushed in the page load event sequence.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Page Load Started",
    "page": {
        "pageName": "<pageName>",
        "siteCountry": "<siteCountry>",
        "siteLanguage": "<siteLanguage>",
        "siteName": "<siteName>",
        "siteType": "<siteType>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|page.pageName|string|Describes the page and its content specifically. |product - XYZ123, Mens - Tops - Sweaters, Order Confirmation|||||||
|page.siteCountry|string|Indicates the primary country served by the site. ISO 3166 \(alpha-2\) Uppercase.|US, CA, FR, UK|^[A-Z]{2}$||||||
|page.siteLanguage|string|Language in which the site is presented ISO 639-1 code. |en-us, en-gb, ch-cn, fr-ca, fr-fr, da|^[a-z]{2}([-]{1}[a-z]{2}){0,1}$||||||
|page.siteName|string|Common language used within the business to refer to the website. May be specific County Sites.|Prospecting-EU, Prospecting-US, Member Portal, Shop-CA, Shop-US, Shop-EU|||||||
|page.siteType|string|Common language description of the site type of purpose. May be used to group siteName.|Prospecting, Shop, Members, Brand|||||||




