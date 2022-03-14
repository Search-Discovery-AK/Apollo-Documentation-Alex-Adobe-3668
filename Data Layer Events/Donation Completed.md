# Donation Completed

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Donation Completed",
    "donation": {
        "item": [
            {
                "donationID": "<donationID>"
            }
        ],
        "profile": {
            "address": {
                "stateProvince": "<stateProvince>"
            }
        },
        "total": {
            "currency": "<currency>"
        }
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|donation.item[n].donationID|string|Unique identifier of the donation. Max Length 20. Used to prevent duplication.||^[a-zA-Z0-9]{6,20}$|6|20||||
|donation.profile.address.stateProvince|string|The mailing state or province associated with the donation payment. |MO, GA, NB, ON|||||||
|donation.total.currency|string|Currency of the donation payment. ISO 4217 \(3 character alpha\), uppercase |USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||




