# Chat Started

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Chat Started",
    "chat": {
        "portalID": "<portalID>",
        "serviceLine": "<serviceLine>",
        "sessionID": "<sessionID>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|chat.portalID|string|Identifies the specific chat portal used||||||||
|chat.serviceLine|string|Identifies the specific chat portal used||||||||
|chat.sessionID|string|Identifies the specific chat session||||||||




