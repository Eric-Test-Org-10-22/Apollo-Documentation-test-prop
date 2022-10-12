# Accommodation Booking Started

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Accommodation Booking Started",
    "booking": {
        "roomList": [
            {
                "location": {
                    "locationId": "<locationId>"
                },
                "room": {
                    "numAdults": <numAdults>,
                    "numKids": <numKids>,
                    "numberInMultiRoomReservation": <numberInMultiRoomReservation>,
                    "rateCode": "<rateCode>",
                    "ratePerNight": "<ratePerNight>",
                    "stayDate": "<stayDate>",
                    "typeCode": "<typeCode>"
                }
            }
        ],
        "total": {
            "currency": "<currency>"
        }
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|booking.roomList[n].location.locationId|string|Unique Identifier of a Location. |155, 65588, 987764448|||||||
|booking.roomList[n].room.numAdults|integer|Integer number of adults for the booking.|1, 2, 3, 4, 5||||1|||
|booking.roomList[n].room.numKids|integer|Integer number of kids for the booking.|1, 2, 3, 4, 5||||0|||
|booking.roomList[n].room.numberInMultiRoomReservation|integer|Integer position of a room in a multi-room booking action.|1, 2, 3||||1|||
|booking.roomList[n].room.rateCode|string|Description of the rate being offered. Should match rate codes from back-end systems to allow data import. |AAA, MILITARY, CORP-567, CORP-345|||||||
|booking.roomList[n].room.ratePerNight|string|String representation of the price per use-period. Typically nightly rate for a hotel room or monthly rate for an apartment. Positive. Up to two decimal places for cents. No currency symbol.|200, 75.29, 150, 89.2|^[0-9]*(\.[0-9]{1,2})?$||||||
|booking.roomList[n].room.stayDate|string|Date of each room night. ISO 8601 form \(YYYY-MM-DD\). Jan 1, 2019 is 2019-01-01|2001-12-22, 2011-01-01|^([0-9]{4})-(1[0-2]|0[1-9])-(3[01]|0[1-9]|[12][0-9])$||||||
|booking.roomList[n].room.typeCode|string|A code describing the room features. Often indicates number of beds, smoking or non-smoking, ADA accessibility and so on.|1-K-NS, 2-Q-S, S-K-NS-City|||||||
|booking.total.currency|string|Currency of the payment for the booking. ISO 4217 \(3 character alpha\), uppercase |USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||




