# Internal Campaign Clicked

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Internal Campaign Clicked",
    "internalCampaign": {
        "campaignList": [
            {
                "internalCampaignID": "<internalCampaignID>",
                "internalCampaignName": "<internalCampaignName>",
                "internalCampaignObjective": "<internalCampaignObjective>",
                "internalCampaignPosition": <internalCampaignPosition>
            }
        ],
        "internalCampaignID": "<internalCampaignID>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|internalCampaign.campaignList[n].internalCampaignID|string|Unique Identifier of an internal campaign|2345, 56789, 9876|||||||
|internalCampaign.campaignList[n].internalCampaignName|string|The name of the promotion.|Trek bikes for kids, REI Spring Sale 2019, Viking Cruise Fall Specials|||||||
|internalCampaign.campaignList[n].internalCampaignObjective|string|Objective of the Internal Campaign|Order Starter, Order Value, Newsletter Subscriptions, 12, 33, 44|||||||
|internalCampaign.campaignList[n].internalCampaignPosition|integer|The position of a internal campaign offering within a list of internal campaigns|1, 5, 78, 3||||1|||
|internalCampaign.internalCampaignID|string|Unique Identifier of an internal campaign|2345, 56789, 9876|||||||




