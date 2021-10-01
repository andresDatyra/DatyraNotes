
# Conversation API Test Report

**Report Generated On**: Thu Sep 30 2021 16:05:08 GMT-0700 (Pacific Daylight Time)
**API Methods Tested**: 8

## Table of Contents

A. [Test Results](#test-results):

- 1. [Get Conversation event](#get-conversation-event) :x:


- 2. [Get Conversation](#get-conversation) :x:


- 3. [List Conversation events](#list-conversation-events) :x:


- 4. [List Conversation media](#list-conversation-media) :x:


- 5. [List Conversations](#list-conversations) :x:


- 6. [Send Conversation Message](#send-conversation-message) :x:


- 7. [Update Conversation Membership](#update-conversation-membership) :white_check_mark:


- 8. [Update Conversation Info](#update-conversation-info) :x:
  9. [Leave Conversation](#leave-conversation) :white_check_mark:
  10. [Delete Conversation Message](#delete-conversation-message) :white_check_mark:
  11. [Create Conversation](#create-conversation) :x:
  12. [Add Conversation recipients](#add-conversation-recipients) :x:
  13. [Find Conversation](#find-conversation) :x:


## Test Results

### Get Conversation event

> Route: **conversation.get_event**
> Time elapsed: **0.800s**
> Variations successful: 0/1


#### Variation 1 (0.799s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "conversationId": "13",
    "eventId": "72"
}
```

##### :package: Response Data

```json
null
```

##### :warning: Response Error

```json
Error: Request failed with status code 500
    at createError (/Users/matteuc/Desktop/Family Proud/FamilyProudCloud/function-tests/node_modules/axios/lib/core/createError.js:16:15)
    at settle (/Users/matteuc/Desktop/Family Proud/FamilyProudCloud/function-tests/node_modules/axios/lib/core/settle.js:17:12)
    at IncomingMessage.handleStreamEnd (/Users/matteuc/Desktop/Family Proud/FamilyProudCloud/function-tests/node_modules/axios/lib/adapters/http.js:269:11)
    at IncomingMessage.emit (events.js:327:22)
    at endReadableNT (internal/streams/readable.js:1327:12)
    at processTicksAndRejections (internal/process/task_queues.js:80:21)
```

##### :ab: Response Type Error

```json
null
```

##### :mag_right: Verification Cases


***

### Get Conversation

> Route: **conversation.get**
> Time elapsed: **0.651s**
> Variations successful: 0/1


#### Variation 1 (0.646s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "conversationId": "13"
}
```

##### :package: Response Data

```json
{
    "createdAt": 1619530964000,
    "id": 13,
    "isGroup": false,
    "isPrivate": true,
    "keywords": [
        "t",
        "tr",
        "tre",
        "trev",
        "trevo",
        "trevor",
        "trevor ",
        "trevor  ",
        "trevor  p",
        "trevor  pr",
        "trevor  pro",
        "trevor  prop",
        "trevor  proph",
        "trevor  prophe",
        "trevor  prophet",
        "trevor  prophet ",
        "trevor  prophet  ",
        "trevor  prophet  m",
        "trevor  prophet  ma",
        "trevor  prophet  mat",
        "trevor  prophet  matt",
        "trevor  prophet  matth",
        "trevor  prophet  matthe",
        "trevor  prophet  matthew",
        "trevor  prophet  matthew ",
        "trevor  prophet  matthew c",
        "trevor  prophet  matthew ch",
        "trevor  prophet  matthew che",
        "trevor  prophet  matthew chen",
        "p",
        "pr",
        "pro",
        "prop",
        "proph",
        "prophe",
        "prophet",
        "m",
        "ma",
        "mat",
        "matt",
        "matth",
        "matthe",
        "matthew",
        "c",
        "ch",
        "che",
        "chen"
    ],
    "lastEventId": null,
    "lastUpdated": 1619629509000,
    "nickname": null,
    "recipientsIndex": [
        10,
        11
    ],
    "type": "c",
    "avatarKey": null,
    "muted": false,
    "read": true,
    "allRecipients": [
        {
            "attributes": [],
            "challenges": "!!!!!!!jkkghjghjhg",
            "createdAt": 1617839288000,
            "disabled": null,
            "email": "yuishean@gmail.com",
            "firstName": "Matt",
            "fullName": "Matt Chen",
            "geohash": "9mueksxy3r",
            "helpingOut": "",
            "id": 22,
            "initialPersona": 0,
            "keywords": [
                "m",
                "ma",
                "mat",
                "matt",
                "matt",
                "matt c",
                "matt ch",
                "matt che",
                "matt chen",
                "c",
                "ch",
                "che",
                "chen"
            ],
            "lastLoginTime": 1632929787391,
            "lastLogoutTime": 1632929787391,
            "lastName": "Chen",
            "lat": 32.94086965214003,
            "lng": -117.2134142493164,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "",
            "sms": "324324",
            "type": "u",
            "updatedAt": 1632929787391,
            "zipCode": "92130",
            "userRef": 11,
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633647903&Signature=lUakoCZ12oTT76Sk7j1sNZQ9xHl4nWbU8SXHshDQ3Aq%2BLSjyDPWR8G7KN63gUuGXbCbs1c0hKY14GsXwD2VNiX1yJ1T2PbKxxAsousdt%2BDzTbPUivfz0VwAkE5XhKER0m1B5Mh%2Fe3z9p36ed7iNDeC2icXLA7mwGX3zc1AxS69ctN4MN8QJge6hGPGwiR%2F2a9gk7hCrEUatBYtL%2FX5%2FAJ8W%2BMf0KA5Feh787wu7Zo7HwSmiDd5DMVDBVHoGAvProkaqr7%2B7%2BlMVFUh9nY5mG3bAQdL%2FdxyeiNGJoir3hR5Uy7E%2B37g7J4CXF4aNQKkdtD6DQLH6Zb3joEmaAdtmwUw%3D%3D"
            },
            "userId": 11
        },
        {
            "attributes": [
                "Veteran"
            ],
            "challenges": "New challenge to test save. ",
            "createdAt": 1619526930000,
            "disabled": null,
            "email": "trevor@familyproud.com",
            "firstName": "Trevor ",
            "fullName": "Trevor  Prop",
            "geohash": "9muds49fh4",
            "helpingOut": "Pick up foo",
            "id": 23,
            "initialPersona": 1,
            "keywords": [
                "t",
                "tr",
                "tre",
                "trev",
                "trevo",
                "trevor",
                "trevor ",
                "trevor  ",
                "trevor  p",
                "trevor  pr",
                "trevor  pro",
                "trevor  prop",
                "trevor  prop ",
                "trevor  prop v",
                "trevor  prop ve",
                "trevor  prop vet",
                "trevor  prop vete",
                "trevor  prop veter",
                "trevor  prop vetera",
                "trevor  prop veteran",
                "p",
                "pr",
                "pro",
                "prop",
                "v",
                "ve",
                "vet",
                "vete",
                "veter",
                "vetera",
                "veteran"
            ],
            "lastLoginTime": 1619526930000,
            "lastLogoutTime": 0,
            "lastName": "Prop",
            "lat": 32.797291898342145,
            "lng": -117.24351527372028,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "None xyz",
            "sms": "",
            "type": "u",
            "updatedAt": 1625667495000,
            "zipCode": "92109",
            "userRef": 10,
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VK6iwMLAOwR8KNagKU1cHu2NXTL2/0srQ8yFHbVpDqEhtVBAd?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633647903&Signature=XwaMDk%2FuycYwkOdYCbWpIomk31kEALLDpZGtANa0KY610IWp2CO4FZkCX%2BsGuNdr3IvBvyU9sew0RRxz0Ar5XZvpCZ2uPi%2BkNzjHnnam0%2FqkzBRXPUpf7ZmnCWPg0yTpilG%2B%2BpMT2yYg8rNlR9QXLSTCHOy41SjFpJ286%2BhdLc7Cg2yFet7czUfwkfVtZp5MPXrlOyB%2BKUcRljZtX28sTlPOohfe8eSXwHHiqe%2FgUWgIzQ3Fra4grnLbqtdcoA%2FBQgznisYOxS42oXoT7A39qURIkMBqIvvJLmVrP78tZMakXHt6jSlsYKl%2BP4%2F2H%2BeMYn02r5guaBVeE9kgHvmUww%3D%3D"
            },
            "userId": 10
        }
    ],
    "activeRecipients": [
        {
            "attributes": [],
            "challenges": "!!!!!!!jkkghjghjhg",
            "createdAt": 1617839288000,
            "disabled": null,
            "email": "yuishean@gmail.com",
            "firstName": "Matt",
            "fullName": "Matt Chen",
            "geohash": "9mueksxy3r",
            "helpingOut": "",
            "id": 22,
            "initialPersona": 0,
            "keywords": [
                "m",
                "ma",
                "mat",
                "matt",
                "matt",
                "matt c",
                "matt ch",
                "matt che",
                "matt chen",
                "c",
                "ch",
                "che",
                "chen"
            ],
            "lastLoginTime": 1632929787391,
            "lastLogoutTime": 1632929787391,
            "lastName": "Chen",
            "lat": 32.94086965214003,
            "lng": -117.2134142493164,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "",
            "sms": "324324",
            "type": "u",
            "updatedAt": 1632929787391,
            "zipCode": "92130",
            "userRef": 11,
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633647903&Signature=lUakoCZ12oTT76Sk7j1sNZQ9xHl4nWbU8SXHshDQ3Aq%2BLSjyDPWR8G7KN63gUuGXbCbs1c0hKY14GsXwD2VNiX1yJ1T2PbKxxAsousdt%2BDzTbPUivfz0VwAkE5XhKER0m1B5Mh%2Fe3z9p36ed7iNDeC2icXLA7mwGX3zc1AxS69ctN4MN8QJge6hGPGwiR%2F2a9gk7hCrEUatBYtL%2FX5%2FAJ8W%2BMf0KA5Feh787wu7Zo7HwSmiDd5DMVDBVHoGAvProkaqr7%2B7%2BlMVFUh9nY5mG3bAQdL%2FdxyeiNGJoir3hR5Uy7E%2B37g7J4CXF4aNQKkdtD6DQLH6Zb3joEmaAdtmwUw%3D%3D"
            },
            "userId": 11
        },
        {
            "attributes": [
                "Veteran"
            ],
            "challenges": "New challenge to test save. ",
            "createdAt": 1619526930000,
            "disabled": null,
            "email": "trevor@familyproud.com",
            "firstName": "Trevor ",
            "fullName": "Trevor  Prop",
            "geohash": "9muds49fh4",
            "helpingOut": "Pick up foo",
            "id": 23,
            "initialPersona": 1,
            "keywords": [
                "t",
                "tr",
                "tre",
                "trev",
                "trevo",
                "trevor",
                "trevor ",
                "trevor  ",
                "trevor  p",
                "trevor  pr",
                "trevor  pro",
                "trevor  prop",
                "trevor  prop ",
                "trevor  prop v",
                "trevor  prop ve",
                "trevor  prop vet",
                "trevor  prop vete",
                "trevor  prop veter",
                "trevor  prop vetera",
                "trevor  prop veteran",
                "p",
                "pr",
                "pro",
                "prop",
                "v",
                "ve",
                "vet",
                "vete",
                "veter",
                "vetera",
                "veteran"
            ],
            "lastLoginTime": 1619526930000,
            "lastLogoutTime": 0,
            "lastName": "Prop",
            "lat": 32.797291898342145,
            "lng": -117.24351527372028,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "None xyz",
            "sms": "",
            "type": "u",
            "updatedAt": 1625667495000,
            "zipCode": "92109",
            "userRef": 10,
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VK6iwMLAOwR8KNagKU1cHu2NXTL2/0srQ8yFHbVpDqEhtVBAd?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633647903&Signature=XwaMDk%2FuycYwkOdYCbWpIomk31kEALLDpZGtANa0KY610IWp2CO4FZkCX%2BsGuNdr3IvBvyU9sew0RRxz0Ar5XZvpCZ2uPi%2BkNzjHnnam0%2FqkzBRXPUpf7ZmnCWPg0yTpilG%2B%2BpMT2yYg8rNlR9QXLSTCHOy41SjFpJ286%2BhdLc7Cg2yFet7czUfwkfVtZp5MPXrlOyB%2BKUcRljZtX28sTlPOohfe8eSXwHHiqe%2FgUWgIzQ3Fra4grnLbqtdcoA%2FBQgznisYOxS42oXoT7A39qURIkMBqIvvJLmVrP78tZMakXHt6jSlsYKl%2BP4%2F2H%2BeMYn02r5guaBVeE9kgHvmUww%3D%3D"
            },
            "userId": 10
        }
    ],
    "events": [
        {
            "conversationId": 13,
            "conversationMemberId": 23,
            "createdAt": 1619530968000,
            "eventType": "message",
            "id": 82,
            "text": "Testing",
            "updatedAt": 1619530968000,
            "user": {
                "attributes": [
                    "Veteran"
                ],
                "challenges": "New challenge to test save. ",
                "createdAt": 1619526930000,
                "disabled": null,
                "email": "trevor@familyproud.com",
                "firstName": "Trevor ",
                "fullName": "Trevor  Prop",
                "geohash": "9muds49fh4",
                "helpingOut": "Pick up foo",
                "id": 23,
                "initialPersona": 1,
                "keywords": [
                    "t",
                    "tr",
                    "tre",
                    "trev",
                    "trevo",
                    "trevor",
                    "trevor ",
                    "trevor  ",
                    "trevor  p",
                    "trevor  pr",
                    "trevor  pro",
                    "trevor  prop",
                    "trevor  prop ",
                    "trevor  prop v",
                    "trevor  prop ve",
                    "trevor  prop vet",
                    "trevor  prop vete",
                    "trevor  prop veter",
                    "trevor  prop vetera",
                    "trevor  prop veteran",
                    "p",
                    "pr",
                    "pro",
                    "prop",
                    "v",
                    "ve",
                    "vet",
                    "vete",
                    "veter",
                    "vetera",
                    "veteran"
                ],
                "lastLoginTime": 1619526930000,
                "lastLogoutTime": 0,
                "lastName": "Prop",
                "lat": 32.797291898342145,
                "lng": -117.24351527372028,
                "locationName": "San Diego, CA",
                "mapVisibility": true,
                "onBoardingComplete": true,
                "onboardingProgress": null,
                "organizationId": null,
                "ownNeeds": "None xyz",
                "sms": "",
                "type": "u",
                "updatedAt": 1625667495000,
                "zipCode": "92109",
                "userRef": 10,
                "avatarKey": {
                    "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VK6iwMLAOwR8KNagKU1cHu2NXTL2/0srQ8yFHbVpDqEhtVBAd?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633647903&Signature=XwaMDk%2FuycYwkOdYCbWpIomk31kEALLDpZGtANa0KY610IWp2CO4FZkCX%2BsGuNdr3IvBvyU9sew0RRxz0Ar5XZvpCZ2uPi%2BkNzjHnnam0%2FqkzBRXPUpf7ZmnCWPg0yTpilG%2B%2BpMT2yYg8rNlR9QXLSTCHOy41SjFpJ286%2BhdLc7Cg2yFet7czUfwkfVtZp5MPXrlOyB%2BKUcRljZtX28sTlPOohfe8eSXwHHiqe%2FgUWgIzQ3Fra4grnLbqtdcoA%2FBQgznisYOxS42oXoT7A39qURIkMBqIvvJLmVrP78tZMakXHt6jSlsYKl%2BP4%2F2H%2BeMYn02r5guaBVeE9kgHvmUww%3D%3D"
                },
                "userId": 10
            },
            "attachmentsMap": {}
        },
        {
            "conversationId": 13,
            "conversationMemberId": 23,
            "createdAt": 1619530977000,
            "eventType": "message",
            "id": 79,
            "text": "",
            "updatedAt": 1619530977000,
            "user": {
                "attributes": [
                    "Veteran"
                ],
                "challenges": "New challenge to test save. ",
                "createdAt": 1619526930000,
                "disabled": null,
                "email": "trevor@familyproud.com",
                "firstName": "Trevor ",
                "fullName": "Trevor  Prop",
                "geohash": "9muds49fh4",
                "helpingOut": "Pick up foo",
                "id": 23,
                "initialPersona": 1,
                "keywords": [
                    "t",
                    "tr",
                    "tre",
                    "trev",
                    "trevo",
                    "trevor",
                    "trevor ",
                    "trevor  ",
                    "trevor  p",
                    "trevor  pr",
                    "trevor  pro",
                    "trevor  prop",
                    "trevor  prop ",
                    "trevor  prop v",
                    "trevor  prop ve",
                    "trevor  prop vet",
                    "trevor  prop vete",
                    "trevor  prop veter",
                    "trevor  prop vetera",
                    "trevor  prop veteran",
                    "p",
                    "pr",
                    "pro",
                    "prop",
                    "v",
                    "ve",
                    "vet",
                    "vete",
                    "veter",
                    "vetera",
                    "veteran"
                ],
                "lastLoginTime": 1619526930000,
                "lastLogoutTime": 0,
                "lastName": "Prop",
                "lat": 32.797291898342145,
                "lng": -117.24351527372028,
                "locationName": "San Diego, CA",
                "mapVisibility": true,
                "onBoardingComplete": true,
                "onboardingProgress": null,
                "organizationId": null,
                "ownNeeds": "None xyz",
                "sms": "",
                "type": "u",
                "updatedAt": 1625667495000,
                "zipCode": "92109",
                "userRef": 10,
                "avatarKey": {
                    "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VK6iwMLAOwR8KNagKU1cHu2NXTL2/0srQ8yFHbVpDqEhtVBAd?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633647903&Signature=XwaMDk%2FuycYwkOdYCbWpIomk31kEALLDpZGtANa0KY610IWp2CO4FZkCX%2BsGuNdr3IvBvyU9sew0RRxz0Ar5XZvpCZ2uPi%2BkNzjHnnam0%2FqkzBRXPUpf7ZmnCWPg0yTpilG%2B%2BpMT2yYg8rNlR9QXLSTCHOy41SjFpJ286%2BhdLc7Cg2yFet7czUfwkfVtZp5MPXrlOyB%2BKUcRljZtX28sTlPOohfe8eSXwHHiqe%2FgUWgIzQ3Fra4grnLbqtdcoA%2FBQgznisYOxS42oXoT7A39qURIkMBqIvvJLmVrP78tZMakXHt6jSlsYKl%2BP4%2F2H%2BeMYn02r5guaBVeE9kgHvmUww%3D%3D"
                },
                "userId": 10
            },
            "attachmentsMap": {}
        },
        {
            "conversationId": 13,
            "conversationMemberId": 23,
            "createdAt": 1619531002000,
            "eventType": "message",
            "id": 76,
            "text": "",
            "updatedAt": 1619531002000,
            "user": {
                "attributes": [
                    "Veteran"
                ],
                "challenges": "New challenge to test save. ",
                "createdAt": 1619526930000,
                "disabled": null,
                "email": "trevor@familyproud.com",
                "firstName": "Trevor ",
                "fullName": "Trevor  Prop",
                "geohash": "9muds49fh4",
                "helpingOut": "Pick up foo",
                "id": 23,
                "initialPersona": 1,
                "keywords": [
                    "t",
                    "tr",
                    "tre",
                    "trev",
                    "trevo",
                    "trevor",
                    "trevor ",
                    "trevor  ",
                    "trevor  p",
                    "trevor  pr",
                    "trevor  pro",
                    "trevor  prop",
                    "trevor  prop ",
                    "trevor  prop v",
                    "trevor  prop ve",
                    "trevor  prop vet",
                    "trevor  prop vete",
                    "trevor  prop veter",
                    "trevor  prop vetera",
                    "trevor  prop veteran",
                    "p",
                    "pr",
                    "pro",
                    "prop",
                    "v",
                    "ve",
                    "vet",
                    "vete",
                    "veter",
                    "vetera",
                    "veteran"
                ],
                "lastLoginTime": 1619526930000,
                "lastLogoutTime": 0,
                "lastName": "Prop",
                "lat": 32.797291898342145,
                "lng": -117.24351527372028,
                "locationName": "San Diego, CA",
                "mapVisibility": true,
                "onBoardingComplete": true,
                "onboardingProgress": null,
                "organizationId": null,
                "ownNeeds": "None xyz",
                "sms": "",
                "type": "u",
                "updatedAt": 1625667495000,
                "zipCode": "92109",
                "userRef": 10,
                "avatarKey": {
                    "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VK6iwMLAOwR8KNagKU1cHu2NXTL2/0srQ8yFHbVpDqEhtVBAd?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633647903&Signature=XwaMDk%2FuycYwkOdYCbWpIomk31kEALLDpZGtANa0KY610IWp2CO4FZkCX%2BsGuNdr3IvBvyU9sew0RRxz0Ar5XZvpCZ2uPi%2BkNzjHnnam0%2FqkzBRXPUpf7ZmnCWPg0yTpilG%2B%2BpMT2yYg8rNlR9QXLSTCHOy41SjFpJ286%2BhdLc7Cg2yFet7czUfwkfVtZp5MPXrlOyB%2BKUcRljZtX28sTlPOohfe8eSXwHHiqe%2FgUWgIzQ3Fra4grnLbqtdcoA%2FBQgznisYOxS42oXoT7A39qURIkMBqIvvJLmVrP78tZMakXHt6jSlsYKl%2BP4%2F2H%2BeMYn02r5guaBVeE9kgHvmUww%3D%3D"
                },
                "userId": 10
            },
            "attachmentsMap": {}
        }
    ],
    "media": []
}
```

##### :warning: Response Error

```json
null
```

##### :ab: Response Type Error

```json
ValidationError: Expected { id: string; nickname: string | null; isGroup: boolean; isPrivate: boolean; lastEventId: string | null; recipientsIndex: string; keywords: string[]; lastUpdated: number; createdAt: number; muted: boolean; lastChecked: number; read: boolean; avatarKey: { uri: string; } | null; allRecipients: ({ id: string; userId: string; } & { avatarKey: { uri: string; } | null; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; })[]; activeRecipients: ({ id: string; userId: string; } & { avatarKey: { uri: string; } | null; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; })[]; events: { id: string; eventType: "message"; conversationId: string; conversationMemberId: string; text: string; createdAt: number; updatedAt: number; user: { id: string; userId: string; } & { avatarKey: { uri: string; } | null; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; attachmentsMap: { [_: string]: { id: string; conversationId: string; eventId: string; mediaType: "image"; ref: { uri: string; }; createdAt: number; } }; }[]; media: { id: string; conversationId: string; eventId: string; mediaType: "image"; ref: { uri: string; }; createdAt: number; }[]; } | null, but was object
```

##### :mag_right: Verification Cases


***

### List Conversation events

> Route: **conversation.list_events**
> Time elapsed: **0.577s**
> Variations successful: 0/1


#### Variation 1 (0.574s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "conversationId": "13"
}
```

##### :package: Response Data

```json

[
    {
        "conversationId": 13,
        "conversationMemberId": 23,
        "createdAt": 1619530968000,
        "eventType": "message",
        "id": 82,
        "text": "Testing",
        "updatedAt": 1619530968000,
        "user": {
            "attributes": [
                "Veteran"
            ],
            "challenges": "New challenge to test save. ",
            "createdAt": 1619526930000,
            "disabled": null,
            "email": "trevor@familyproud.com",
            "firstName": "Trevor ",
            "fullName": "Trevor  Prop",
            "geohash": "9muds49fh4",
            "helpingOut": "Pick up foo",
            "id": 23,
            "initialPersona": 1,
            "keywords": [
                "t",
                "tr",
                "tre",
                "trev",
                "trevo",
                "trevor",
                "trevor ",
                "trevor  ",
                "trevor  p",
                "trevor  pr",
                "trevor  pro",
                "trevor  prop",
                "trevor  prop ",
                "trevor  prop v",
                "trevor  prop ve",
                "trevor  prop vet",
                "trevor  prop vete",
                "trevor  prop veter",
                "trevor  prop vetera",
                "trevor  prop veteran",
                "p",
                "pr",
                "pro",
                "prop",
                "v",
                "ve",
                "vet",
                "vete",
                "veter",
                "vetera",
                "veteran"
            ],
            "lastLoginTime": 1619526930000,
            "lastLogoutTime": 0,
            "lastName": "Prop",
            "lat": 32.797291898342145,
            "lng": -117.24351527372028,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "None xyz",
            "sms": "",
            "type": "u",
            "updatedAt": 1625667495000,
            "zipCode": "92109",
            "userRef": 10,
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VK6iwMLAOwR8KNagKU1cHu2NXTL2/0srQ8yFHbVpDqEhtVBAd?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633647903&Signature=XwaMDk%2FuycYwkOdYCbWpIomk31kEALLDpZGtANa0KY610IWp2CO4FZkCX%2BsGuNdr3IvBvyU9sew0RRxz0Ar5XZvpCZ2uPi%2BkNzjHnnam0%2FqkzBRXPUpf7ZmnCWPg0yTpilG%2B%2BpMT2yYg8rNlR9QXLSTCHOy41SjFpJ286%2BhdLc7Cg2yFet7czUfwkfVtZp5MPXrlOyB%2BKUcRljZtX28sTlPOohfe8eSXwHHiqe%2FgUWgIzQ3Fra4grnLbqtdcoA%2FBQgznisYOxS42oXoT7A39qURIkMBqIvvJLmVrP78tZMakXHt6jSlsYKl%2BP4%2F2H%2BeMYn02r5guaBVeE9kgHvmUww%3D%3D"
            },
            "userId": 10
        },
        "attachmentsMap": {}
    },
    {
        "conversationId": 13,
        "conversationMemberId": 23,
        "createdAt": 1619530977000,
        "eventType": "message",
        "id": 79,
        "text": "",
        "updatedAt": 1619530977000,
        "user": {
            "attributes": [
                "Veteran"
            ],
            "challenges": "New challenge to test save. ",
            "createdAt": 1619526930000,
            "disabled": null,
            "email": "trevor@familyproud.com",
            "firstName": "Trevor ",
            "fullName": "Trevor  Prop",
            "geohash": "9muds49fh4",
            "helpingOut": "Pick up foo",
            "id": 23,
            "initialPersona": 1,
            "keywords": [
                "t",
                "tr",
                "tre",
                "trev",
                "trevo",
                "trevor",
                "trevor ",
                "trevor  ",
                "trevor  p",
                "trevor  pr",
                "trevor  pro",
                "trevor  prop",
                "trevor  prop ",
                "trevor  prop v",
                "trevor  prop ve",
                "trevor  prop vet",
                "trevor  prop vete",
                "trevor  prop veter",
                "trevor  prop vetera",
                "trevor  prop veteran",
                "p",
                "pr",
                "pro",
                "prop",
                "v",
                "ve",
                "vet",
                "vete",
                "veter",
                "vetera",
                "veteran"
            ],
            "lastLoginTime": 1619526930000,
            "lastLogoutTime": 0,
            "lastName": "Prop",
            "lat": 32.797291898342145,
            "lng": -117.24351527372028,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "None xyz",
            "sms": "",
            "type": "u",
            "updatedAt": 1625667495000,
            "zipCode": "92109",
            "userRef": 10,
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VK6iwMLAOwR8KNagKU1cHu2NXTL2/0srQ8yFHbVpDqEhtVBAd?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633647903&Signature=XwaMDk%2FuycYwkOdYCbWpIomk31kEALLDpZGtANa0KY610IWp2CO4FZkCX%2BsGuNdr3IvBvyU9sew0RRxz0Ar5XZvpCZ2uPi%2BkNzjHnnam0%2FqkzBRXPUpf7ZmnCWPg0yTpilG%2B%2BpMT2yYg8rNlR9QXLSTCHOy41SjFpJ286%2BhdLc7Cg2yFet7czUfwkfVtZp5MPXrlOyB%2BKUcRljZtX28sTlPOohfe8eSXwHHiqe%2FgUWgIzQ3Fra4grnLbqtdcoA%2FBQgznisYOxS42oXoT7A39qURIkMBqIvvJLmVrP78tZMakXHt6jSlsYKl%2BP4%2F2H%2BeMYn02r5guaBVeE9kgHvmUww%3D%3D"
            },
            "userId": 10
        },
        "attachmentsMap": {}
    },
    {
        "conversationId": 13,
        "conversationMemberId": 23,
        "createdAt": 1619531002000,
        "eventType": "message",
        "id": 76,
        "text": "",
        "updatedAt": 1619531002000,
        "user": {
            "attributes": [
                "Veteran"
            ],
            "challenges": "New challenge to test save. ",
            "createdAt": 1619526930000,
            "disabled": null,
            "email": "trevor@familyproud.com",
            "firstName": "Trevor ",
            "fullName": "Trevor  Prop",
            "geohash": "9muds49fh4",
            "helpingOut": "Pick up foo",
            "id": 23,
            "initialPersona": 1,
            "keywords": [
                "t",
                "tr",
                "tre",
                "trev",
                "trevo",
                "trevor",
                "trevor ",
                "trevor  ",
                "trevor  p",
                "trevor  pr",
                "trevor  pro",
                "trevor  prop",
                "trevor  prop ",
                "trevor  prop v",
                "trevor  prop ve",
                "trevor  prop vet",
                "trevor  prop vete",
                "trevor  prop veter",
                "trevor  prop vetera",
                "trevor  prop veteran",
                "p",
                "pr",
                "pro",
                "prop",
                "v",
                "ve",
                "vet",
                "vete",
                "veter",
                "vetera",
                "veteran"
            ],
            "lastLoginTime": 1619526930000,
            "lastLogoutTime": 0,
            "lastName": "Prop",
            "lat": 32.797291898342145,
            "lng": -117.24351527372028,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "None xyz",
            "sms": "",
            "type": "u",
            "updatedAt": 1625667495000,
            "zipCode": "92109",
            "userRef": 10,
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VK6iwMLAOwR8KNagKU1cHu2NXTL2/0srQ8yFHbVpDqEhtVBAd?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633647903&Signature=XwaMDk%2FuycYwkOdYCbWpIomk31kEALLDpZGtANa0KY610IWp2CO4FZkCX%2BsGuNdr3IvBvyU9sew0RRxz0Ar5XZvpCZ2uPi%2BkNzjHnnam0%2FqkzBRXPUpf7ZmnCWPg0yTpilG%2B%2BpMT2yYg8rNlR9QXLSTCHOy41SjFpJ286%2BhdLc7Cg2yFet7czUfwkfVtZp5MPXrlOyB%2BKUcRljZtX28sTlPOohfe8eSXwHHiqe%2FgUWgIzQ3Fra4grnLbqtdcoA%2FBQgznisYOxS42oXoT7A39qURIkMBqIvvJLmVrP78tZMakXHt6jSlsYKl%2BP4%2F2H%2BeMYn02r5guaBVeE9kgHvmUww%3D%3D"
            },
            "userId": 10
        },
        "attachmentsMap": {}
    },
    {
        "conversationId": 13,
        "conversationMemberId": 22,
        "createdAt": 1619613641000,
        "eventType": "message",
        "id": 78,
        "text": "very majestic dog photo",
        "updatedAt": 1619613641000,
        "user": {
            "attributes": [],
            "challenges": "!!!!!!!jkkghjghjhg",
            "createdAt": 1617839288000,
            "disabled": null,
            "email": "yuishean@gmail.com",
            "firstName": "Matt",
            "fullName": "Matt Chen",
            "geohash": "9mueksxy3r",
            "helpingOut": "",
            "id": 22,
            "initialPersona": 0,
            "keywords": [
                "m",
                "ma",
                "mat",
                "matt",
                "matt",
                "matt c",
                "matt ch",
                "matt che",
                "matt chen",
                "c",
                "ch",
                "che",
                "chen"
            ],
            "lastLoginTime": 1632929787391,
            "lastLogoutTime": 1632929787391,
            "lastName": "Chen",
            "lat": 32.94086965214003,
            "lng": -117.2134142493164,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "",
            "sms": "324324",
            "type": "u",
            "updatedAt": 1632929787391,
            "zipCode": "92130",
            "userRef": 11,
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633647903&Signature=lUakoCZ12oTT76Sk7j1sNZQ9xHl4nWbU8SXHshDQ3Aq%2BLSjyDPWR8G7KN63gUuGXbCbs1c0hKY14GsXwD2VNiX1yJ1T2PbKxxAsousdt%2BDzTbPUivfz0VwAkE5XhKER0m1B5Mh%2Fe3z9p36ed7iNDeC2icXLA7mwGX3zc1AxS69ctN4MN8QJge6hGPGwiR%2F2a9gk7hCrEUatBYtL%2FX5%2FAJ8W%2BMf0KA5Feh787wu7Zo7HwSmiDd5DMVDBVHoGAvProkaqr7%2B7%2BlMVFUh9nY5mG3bAQdL%2FdxyeiNGJoir3hR5Uy7E%2B37g7J4CXF4aNQKkdtD6DQLH6Zb3joEmaAdtmwUw%3D%3D"
            },
            "userId": 11
        },
        "attachmentsMap": {}
    },
    {
        "conversationId": 13,
        "conversationMemberId": 23,
        "createdAt": 1619613905000,
        "eventType": "message",
        "id": 80,
        "text": "🐶",
        "updatedAt": 1619613905000,
        "user": {
            "attributes": [
                "Veteran"
            ],
            "challenges": "New challenge to test save. ",
            "createdAt": 1619526930000,
            "disabled": null,
            "email": "trevor@familyproud.com",
            "firstName": "Trevor ",
            "fullName": "Trevor  Prop",
            "geohash": "9muds49fh4",
            "helpingOut": "Pick up foo",
            "id": 23,
            "initialPersona": 1,
            "keywords": [
                "t",
                "tr",
                "tre",
                "trev",
                "trevo",
                "trevor",
                "trevor ",
                "trevor  ",
                "trevor  p",
                "trevor  pr",
                "trevor  pro",
                "trevor  prop",
                "trevor  prop ",
                "trevor  prop v",
                "trevor  prop ve",
                "trevor  prop vet",
                "trevor  prop vete",
                "trevor  prop veter",
                "trevor  prop vetera",
                "trevor  prop veteran",
                "p",
                "pr",
                "pro",
                "prop",
                "v",
                "ve",
                "vet",
                "vete",
                "veter",
                "vetera",
                "veteran"
            ],
            "lastLoginTime": 1619526930000,
            "lastLogoutTime": 0,
            "lastName": "Prop",
            "lat": 32.797291898342145,
            "lng": -117.24351527372028,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "None xyz",
            "sms": "",
            "type": "u",
            "updatedAt": 1625667495000,
            "zipCode": "92109",
            "userRef": 10,
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VK6iwMLAOwR8KNagKU1cHu2NXTL2/0srQ8yFHbVpDqEhtVBAd?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633647903&Signature=XwaMDk%2FuycYwkOdYCbWpIomk31kEALLDpZGtANa0KY610IWp2CO4FZkCX%2BsGuNdr3IvBvyU9sew0RRxz0Ar5XZvpCZ2uPi%2BkNzjHnnam0%2FqkzBRXPUpf7ZmnCWPg0yTpilG%2B%2BpMT2yYg8rNlR9QXLSTCHOy41SjFpJ286%2BhdLc7Cg2yFet7czUfwkfVtZp5MPXrlOyB%2BKUcRljZtX28sTlPOohfe8eSXwHHiqe%2FgUWgIzQ3Fra4grnLbqtdcoA%2FBQgznisYOxS42oXoT7A39qURIkMBqIvvJLmVrP78tZMakXHt6jSlsYKl%2BP4%2F2H%2BeMYn02r5guaBVeE9kgHvmUww%3D%3D"
            },
            "userId": 10
        },
        "attachmentsMap": {}
    }
]

/* For this preview, a max of 5 items shown */

```

##### :warning: Response Error

```json
null
```

##### :ab: Response Type Error

```json
ValidationError: Expected { id: string; eventType: "message"; conversationId: string; conversationMemberId: string; text: string; createdAt: number; updatedAt: number; user: { id: string; userId: string; } & { avatarKey: { uri: string; } | null; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; attachmentsMap: { [_: string]: { id: string; conversationId: string; eventId: string; mediaType: "image"; ref: { uri: string; }; createdAt: number; } }; }[], but was incompatible
```

##### :mag_right: Verification Cases


***

### List Conversation media

> Route: **conversation.list_media**
> Time elapsed: **0.611s**
> Variations successful: 0/1


#### Variation 1 (0.610s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "conversationId": "13"
}
```

##### :package: Response Data

```json

[
    {
        "conversationId": 13,
        "createdAt": 1619531002000,
        "eventId": 76,
        "id": 3,
        "mediaType": "image",
        "ref": {
            "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/conversations/M4HQPJIWNqVjxfST99iP/W2RodyF7pSf4XQnTzndt?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633647904&Signature=Ps1nnIDTXfjuTRh40LeH6WS4TTNnkx2DqhaZWJmuVpqeoLRdq7CB9KRwZOe35RacooUMjY%2FjZHj84i4WM%2FcQTib9JnjhTS23QX%2BoJ7CPX%2BH8gWCgQMZgXmMN%2BJkuZNS4C72BXS3spToeTs8uQAR0knGlh74JM1qfxR8UfWbGQ%2FoTf4XCh6pCColNkk9fFDr%2B2qxnO7BYDhpmBlwn8Gc4aLq%2FxbukFf6BK5mb%2B5ZykDs%2BId58YxKdwB0IUe927my53dqNMeJiH5IzAGx%2F3BOm%2FCdEpCgC7NnifuE%2BcEvMqa9TD0jRtH6mOP3cTx2F%2BemJ%2F1GU43PrERSTSuR43h93VA%3D%3D"
        }
    },
    {
        "conversationId": 13,
        "createdAt": 1619530977000,
        "eventId": 79,
        "id": 4,
        "mediaType": "image",
        "ref": {
            "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/conversations/M4HQPJIWNqVjxfST99iP/pHkF0FNALxyEF8NHpayn?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633647904&Signature=foCgWMh2JBgJE5fbqOqx2BOFNxSJvs%2BUH8CcGt6NOAibXmsYcvbJoAdZeUR0mSaVgOgz4lxo%2FREZab%2BS9lU5rS6gCteeOQ5neC3T5qMrskzrcIIpFgtRr3PAiMm5a4ZLJD384a1osWaA9n0LaSOHooL9cC9HQYJ5NEaa4UUZHpHq8WHuAH8Qt5DOu2M%2B%2BxqY4jZBUbyEFn%2FvlRncCXOzoMd85X4F2JhEC7k3nWXNhH2JILrReWSfBWT%2FskdNQdOvj3TfCcf0TZj5jAI%2BFJBvlydXNgffScwY4XSe3O3uhzJHccTpDwG0iFXVhKspH5Voxgr%2FZz%2FzUNBCZ%2F05aNQMCA%3D%3D"
        }
    }
]

/* For this preview, a max of 5 items shown */

```

##### :warning: Response Error

```json
null
```

##### :ab: Response Type Error

```json
ValidationError: Expected { id: string; conversationId: string; eventId: string; mediaType: "image"; ref: { uri: string; }; createdAt: number; }[], but was incompatible
```

##### :mag_right: Verification Cases


***

### List Conversations

> Route: **conversation.list**
> Time elapsed: **1.025s**
> Variations successful: 0/1


#### Variation 1 (1.025s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{}
```

##### :package: Response Data

```json
null
```

##### :warning: Response Error

```json
Error: Request failed with status code 500
    at createError (/Users/matteuc/Desktop/Family Proud/FamilyProudCloud/function-tests/node_modules/axios/lib/core/createError.js:16:15)
    at settle (/Users/matteuc/Desktop/Family Proud/FamilyProudCloud/function-tests/node_modules/axios/lib/core/settle.js:17:12)
    at IncomingMessage.handleStreamEnd (/Users/matteuc/Desktop/Family Proud/FamilyProudCloud/function-tests/node_modules/axios/lib/adapters/http.js:269:11)
    at IncomingMessage.emit (events.js:327:22)
    at endReadableNT (internal/streams/readable.js:1327:12)
    at processTicksAndRejections (internal/process/task_queues.js:80:21)
```

##### :ab: Response Type Error

```json
null
```

##### :mag_right: Verification Cases


***

### Send Conversation Message

> Route: **conversation.send_message**
> Time elapsed: **0.510s**
> Variations successful: 0/1


#### Variation 1 (0.509s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "conversationId": "13",
    "text": "This is a test message from Family Proud QA!",
    "attachments": []
}
```

##### :package: Response Data

```json
{
    "conversationId": 13,
    "conversationMemberId": 22,
    "createdAt": 1633043105464,
    "eventType": "message",
    "text": "This is a test message from Family Proud QA!",
    "updatedAt": 1633043105464,
    "id": 620,
    "user": {
        "attributes": [],
        "challenges": "!!!!!!!jkkghjghjhg",
        "createdAt": 1617839288000,
        "disabled": null,
        "email": "yuishean@gmail.com",
        "firstName": "Matt",
        "fullName": "Matt Chen",
        "geohash": "9mueksxy3r",
        "helpingOut": "",
        "id": 22,
        "initialPersona": 0,
        "keywords": [
            "m",
            "ma",
            "mat",
            "matt",
            "matt",
            "matt c",
            "matt ch",
            "matt che",
            "matt chen",
            "c",
            "ch",
            "che",
            "chen"
        ],
        "lastLoginTime": 1632929787391,
        "lastLogoutTime": 1632929787391,
        "lastName": "Chen",
        "lat": 32.94086965214003,
        "lng": -117.2134142493164,
        "locationName": "San Diego, CA",
        "mapVisibility": true,
        "onBoardingComplete": true,
        "onboardingProgress": null,
        "organizationId": null,
        "ownNeeds": "",
        "sms": "324324",
        "type": "u",
        "updatedAt": 1632929787391,
        "zipCode": "92130",
        "userRef": 11,
        "avatarKey": {
            "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633647905&Signature=pvEE7rqxqopjh66okzKXF5Q4OnC2xxRD6yW6jI7tjQo%2FkKiggFUm7G9LVIDg2NPTkpCLww26eqVxbpjwSZuQVAvGgM%2FxAnS7QUUiKSvxNm6D0I4RBNT7QJPxjJN7j5Ckq5I0fl0oD4zclL1FTlHugUppPDfCAFfJUooFWztLvHzLUgSAGUlinKQgvXJ9f6V43io0UuEUfmz6GI0k8Kp9Ph8pHBVrHas9mrU6dDJDl5hRQjU97VwI7kAYGuE%2F%2BZM1%2F2FCKNIqcI2FU8tWlo2y72TpT3jZgPKQab34ji66XVUby2XQM6gnRvYxeSmX6k1kQD49kT5nuEXqY6o4jn9Thw%3D%3D"
        },
        "userId": 11
    },
    "attachmentsMap": {}
}
```

##### :warning: Response Error

```json
null
```

##### :ab: Response Type Error

```json
ValidationError: Expected { id: string; eventType: "message"; conversationId: string; conversationMemberId: string; text: string; createdAt: number; updatedAt: number; user: { id: string; userId: string; } & { avatarKey: { uri: string; } | null; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; attachmentsMap: { [_: string]: { id: string; conversationId: string; eventId: string; mediaType: "image"; ref: { uri: string; }; createdAt: number; } }; }, but was incompatible
```

##### :mag_right: Verification Cases


***

### Update Conversation Membership

> Route: **conversation.update_membership**
> Time elapsed: **2.558s**
> Variations successful: 3/3


#### Variation 1 (0.409s) :white_check_mark:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "conversationId": "13",
    "update": {
        "muted": true
    }
}
```

##### :package: Response Data

```json
null
```

##### :warning: Response Error

```json
null
```

##### :ab: Response Type Error

```json
null
```

##### :mag_right: Verification Cases



#### Variation 2 (2.556s) :white_check_mark:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "conversationId": "13",
    "update": {
        "muted": false
    }
}
```

##### :package: Response Data

```json
null
```

##### :warning: Response Error

```json
null
```

##### :ab: Response Type Error

```json
null
```

##### :mag_right: Verification Cases



#### Variation 3 (2.556s) :white_check_mark:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "conversationId": "13",
    "update": {
        "checked": true
    }
}
```

##### :package: Response Data

```json
null
```

##### :warning: Response Error

```json
null
```

##### :ab: Response Type Error

```json
null
```

##### :mag_right: Verification Cases


***

### Update Conversation Info

> Route: **conversation.update**
> Time elapsed: **0.514s**
> Variations successful: 0/1


#### Variation 1 (0.513s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "conversationId": "13",
    "update": {
        "nickname": "Family Proud QA"
    }
}
```

##### :package: Response Data

```json
null
```

##### :warning: Response Error

```json
Error: Request failed with status code 404
    at createError (/Users/matteuc/Desktop/Family Proud/FamilyProudCloud/function-tests/node_modules/axios/lib/core/createError.js:16:15)
    at settle (/Users/matteuc/Desktop/Family Proud/FamilyProudCloud/function-tests/node_modules/axios/lib/core/settle.js:17:12)
    at IncomingMessage.handleStreamEnd (/Users/matteuc/Desktop/Family Proud/FamilyProudCloud/function-tests/node_modules/axios/lib/adapters/http.js:269:11)
    at IncomingMessage.emit (events.js:327:22)
    at endReadableNT (internal/streams/readable.js:1327:12)
    at processTicksAndRejections (internal/process/task_queues.js:80:21)
```

##### :ab: Response Type Error

```json
null
```

##### :mag_right: Verification Cases

### Leave Conversation

> Route: **conversation.leave**
> Time elapsed: **0.611s**
> Variations successful: 1/1


#### Variation 1 (0.610s) :white_check_mark:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "conversationId": "11"
}
```

##### :package: Response Data

```json
null
```

##### :warning: Response Error

```json
null
```

##### :ab: Response Type Error

```json
null
```

##### :mag_right: Verification Cases

### Delete Conversation message

> Route: **conversation.delete_message**
> Time elapsed: **0.817s**
> Variations successful: 1/1


#### Variation 1 (0.816s) :white_check_mark:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "conversationId": "23",
    "eventId": "100"
}
```

##### :package: Response Data

```json
null
```

##### :warning: Response Error

```json
null
```

##### :ab: Response Type Error

```json
null
```

##### :mag_right: Verification Cases

### Create Conversation

> Route: **conversation.create**
> Time elapsed: **1.581s**
> Variations successful: 0/1


#### Variation 1 (1.575s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "recipients": [
        "1"
    ]
}
```

##### :package: Response Data

```json
{
    "createdAt": 1633046104093,
    "id": 492,
    "isGroup": true,
    "isPrivate": true,
    "keywords": [
        "s",
        "st",
        "ste",
        "step",
        "steph",
        "steph",
        "steph h",
        "steph h",
        "steph h m",
        "steph h ma",
        "steph h mat",
        "steph h matt",
        "steph h matt",
        "steph h matt c",
        "steph h matt ch",
        "steph h matt che",
        "steph h matt chen",
        "h",
        "m",
        "ma",
        "mat",
        "matt",
        "c",
        "ch",
        "che",
        "chen"
    ],
    "lastEventId": null,
    "lastUpdated": 1633046104093,
    "nickname": null,
    "recipientsIndex": [
        1,
        11
    ],
    "type": "c",
    "avatarKey": null,
    "muted": false,
    "read": false,
    "allRecipients": [
        {
            "attributes": [
                "Cancer"
            ],
            "challenges": "",
            "createdAt": 1622601286000,
            "disabled": null,
            "email": "steph@familyproud.com",
            "firstName": "Steph",
            "fullName": "Steph H",
            "geohash": "9mudp1c6t2",
            "helpingOut": "",
            "id": 1018,
            "initialPersona": 0,
            "keywords": [
                "s",
                "st",
                "ste",
                "step",
                "steph",
                "steph ",
                "steph h",
                "steph h ",
                "steph h c",
                "steph h ca",
                "steph h can",
                "steph h canc",
                "steph h cance",
                "steph h cancer",
                "h",
                "c",
                "ca",
                "can",
                "canc",
                "cance",
                "cancer"
            ],
            "lastLoginTime": 1622601286000,
            "lastLogoutTime": 0,
            "lastName": "H",
            "lat": 32.70535597155324,
            "lng": -117.11231103725136,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "",
            "sms": "",
            "type": "u",
            "updatedAt": 1625668345000,
            "zipCode": "92113",
            "userRef": 1,
            "avatarKey": null,
            "userId": 1
        },
        {
            "attributes": [],
            "challenges": "!!!!!!!jkkghjghjhg",
            "createdAt": 1617839288000,
            "disabled": null,
            "email": "yuishean@gmail.com",
            "firstName": "Matt",
            "fullName": "Matt Chen",
            "geohash": "9mueksxy3r",
            "helpingOut": "",
            "id": 1017,
            "initialPersona": 0,
            "keywords": [
                "m",
                "ma",
                "mat",
                "matt",
                "matt",
                "matt c",
                "matt ch",
                "matt che",
                "matt chen",
                "c",
                "ch",
                "che",
                "chen"
            ],
            "lastLoginTime": 1632929787391,
            "lastLogoutTime": 1632929787391,
            "lastName": "Chen",
            "lat": 32.94086965214003,
            "lng": -117.2134142493164,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "",
            "sms": "324324",
            "type": "u",
            "updatedAt": 1632929787391,
            "zipCode": "92130",
            "userRef": 11,
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633650904&Signature=kIW8LLmq4FJEKzCvs5lAAZVO6O3Af5FK7WNslMMI38gUXWoC7OTfmjauBwsYIXgg1aG5z4GDeHg9tqRiDv5oXosOOQtkNy%2FW5Npi3HACVxhMNkgO8A4JRCqI2OpqLY3L1YnXkW0r1AxnLbnex5YNzEoWglJ03go8ipkDjs15qev8C3nnwgCmnZR8SOrj5Bwkpt6ph5Qvl2J07GECprNuOb1uzi0wAYuAxDPMkMcTFJP6HFdl%2ByGq%2Fg3nX5wFrATRLMib%2FG6m9GU988so57kEZHLISyNnO6QnRbC%2BbcoLipojPbuoQfzhFtC%2B%2BkcN304bIgnxHkLeamrMjYeEevF8Hw%3D%3D"
            },
            "userId": 11
        }
    ],
    "activeRecipients": [
        {
            "attributes": [
                "Cancer"
            ],
            "challenges": "",
            "createdAt": 1622601286000,
            "disabled": null,
            "email": "steph@familyproud.com",
            "firstName": "Steph",
            "fullName": "Steph H",
            "geohash": "9mudp1c6t2",
            "helpingOut": "",
            "id": 1018,
            "initialPersona": 0,
            "keywords": [
                "s",
                "st",
                "ste",
                "step",
                "steph",
                "steph ",
                "steph h",
                "steph h ",
                "steph h c",
                "steph h ca",
                "steph h can",
                "steph h canc",
                "steph h cance",
                "steph h cancer",
                "h",
                "c",
                "ca",
                "can",
                "canc",
                "cance",
                "cancer"
            ],
            "lastLoginTime": 1622601286000,
            "lastLogoutTime": 0,
            "lastName": "H",
            "lat": 32.70535597155324,
            "lng": -117.11231103725136,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "",
            "sms": "",
            "type": "u",
            "updatedAt": 1625668345000,
            "zipCode": "92113",
            "userRef": 1,
            "avatarKey": null,
            "userId": 1
        },
        {
            "attributes": [],
            "challenges": "!!!!!!!jkkghjghjhg",
            "createdAt": 1617839288000,
            "disabled": null,
            "email": "yuishean@gmail.com",
            "firstName": "Matt",
            "fullName": "Matt Chen",
            "geohash": "9mueksxy3r",
            "helpingOut": "",
            "id": 1017,
            "initialPersona": 0,
            "keywords": [
                "m",
                "ma",
                "mat",
                "matt",
                "matt",
                "matt c",
                "matt ch",
                "matt che",
                "matt chen",
                "c",
                "ch",
                "che",
                "chen"
            ],
            "lastLoginTime": 1632929787391,
            "lastLogoutTime": 1632929787391,
            "lastName": "Chen",
            "lat": 32.94086965214003,
            "lng": -117.2134142493164,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "",
            "sms": "324324",
            "type": "u",
            "updatedAt": 1632929787391,
            "zipCode": "92130",
            "userRef": 11,
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633650904&Signature=kIW8LLmq4FJEKzCvs5lAAZVO6O3Af5FK7WNslMMI38gUXWoC7OTfmjauBwsYIXgg1aG5z4GDeHg9tqRiDv5oXosOOQtkNy%2FW5Npi3HACVxhMNkgO8A4JRCqI2OpqLY3L1YnXkW0r1AxnLbnex5YNzEoWglJ03go8ipkDjs15qev8C3nnwgCmnZR8SOrj5Bwkpt6ph5Qvl2J07GECprNuOb1uzi0wAYuAxDPMkMcTFJP6HFdl%2ByGq%2Fg3nX5wFrATRLMib%2FG6m9GU988so57kEZHLISyNnO6QnRbC%2BbcoLipojPbuoQfzhFtC%2B%2BkcN304bIgnxHkLeamrMjYeEevF8Hw%3D%3D"
            },
            "userId": 11
        }
    ],
    "events": [],
    "media": []
}
```

##### :warning: Response Error

```json
null
```

##### :ab: Response Type Error

```json
ValidationError: Expected { id: string; nickname: string | null; isGroup: boolean; isPrivate: boolean; lastEventId: string | null; recipientsIndex: string; keywords: string[]; lastUpdated: number; createdAt: number; muted: boolean; lastChecked: number; read: boolean; avatarKey: { uri: string; } | null; allRecipients: ({ id: string; userId: string; } & { avatarKey: { uri: string; } | null; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; })[]; activeRecipients: ({ id: string; userId: string; } & { avatarKey: { uri: string; } | null; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; })[]; events: { id: string; eventType: "message"; conversationId: string; conversationMemberId: string; text: string; createdAt: number; updatedAt: number; user: { id: string; userId: string; } & { avatarKey: { uri: string; } | null; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; attachmentsMap: { [_: string]: { id: string; conversationId: string; eventId: string; mediaType: "image"; ref: { uri: string; }; createdAt: number; } }; }[]; media: { id: string; conversationId: string; eventId: string; mediaType: "image"; ref: { uri: string; }; createdAt: number; }[]; }, but was incompatible
```

##### :mag_right: Verification Cases

### Add Conversation recipients

> Route: **conversation.add_recipients**
> Time elapsed: **1.045s**
> Variations successful: 0/1


#### Variation 1 (1.038s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "conversationId": "13",
    "recipients": [
        "3"
    ]
}
```

##### :package: Response Data

```json
{
    "createdAt": 1619530964000,
    "id": 13,
    "isGroup": true,
    "isPrivate": true,
    "keywords": [
        "t",
        "tr",
        "tre",
        "trev",
        "trevo",
        "trevor",
        "trevor ",
        "trevor  ",
        "trevor  p",
        "trevor  pr",
        "trevor  pro",
        "trevor  prop",
        "trevor  proph",
        "trevor  prophe",
        "trevor  prophet",
        "trevor  prophet ",
        "trevor  prophet  ",
        "trevor  prophet  m",
        "trevor  prophet  ma",
        "trevor  prophet  mat",
        "trevor  prophet  matt",
        "trevor  prophet  matth",
        "trevor  prophet  matthe",
        "trevor  prophet  matthew",
        "trevor  prophet  matthew ",
        "trevor  prophet  matthew c",
        "trevor  prophet  matthew ch",
        "trevor  prophet  matthew che",
        "trevor  prophet  matthew chen",
        "p",
        "pr",
        "pro",
        "prop",
        "proph",
        "prophe",
        "prophet",
        "m",
        "ma",
        "mat",
        "matt",
        "matth",
        "matthe",
        "matthew",
        "c",
        "ch",
        "che",
        "chen"
    ],
    "lastEventId": 620,
    "lastUpdated": 1633046237093,
    "nickname": null,
    "recipientsIndex": [
        10,
        11,
        3
    ],
    "type": "c",
    "avatarKey": null,
    "muted": false,
    "read": true,
    "allRecipients": [
        {
            "attributes": [],
            "challenges": "",
            "createdAt": 1625839286000,
            "disabled": null,
            "email": "mewtwo6271@gmail.com",
            "firstName": "Andy",
            "fullName": "Andy Lee",
            "geohash": "c23p86uf5s",
            "helpingOut": "",
            "id": 1019,
            "initialPersona": 2,
            "keywords": [
                "a",
                "an",
                "and",
                "andy",
                "andy ",
                "andy l",
                "andy le",
                "andy lee",
                "l",
                "le",
                "lee"
            ],
            "lastLoginTime": 1625839286000,
            "lastLogoutTime": 0,
            "lastName": "Lee",
            "lat": 47.74008340941491,
            "lng": -122.3260837528106,
            "locationName": "Seattle, WA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "",
            "sms": "",
            "type": "u",
            "updatedAt": 1625839305000,
            "zipCode": "98133",
            "userRef": 3,
            "avatarKey": null,
            "userId": 3
        },
        {
            "attributes": [
                "Veteran"
            ],
            "challenges": "New challenge to test save. ",
            "createdAt": 1619526930000,
            "disabled": null,
            "email": "trevor@familyproud.com",
            "firstName": "Trevor ",
            "fullName": "Trevor  Prop",
            "geohash": "9muds49fh4",
            "helpingOut": "Pick up foo",
            "id": 23,
            "initialPersona": 1,
            "keywords": [
                "t",
                "tr",
                "tre",
                "trev",
                "trevo",
                "trevor",
                "trevor ",
                "trevor  ",
                "trevor  p",
                "trevor  pr",
                "trevor  pro",
                "trevor  prop",
                "trevor  prop ",
                "trevor  prop v",
                "trevor  prop ve",
                "trevor  prop vet",
                "trevor  prop vete",
                "trevor  prop veter",
                "trevor  prop vetera",
                "trevor  prop veteran",
                "p",
                "pr",
                "pro",
                "prop",
                "v",
                "ve",
                "vet",
                "vete",
                "veter",
                "vetera",
                "veteran"
            ],
            "lastLoginTime": 1619526930000,
            "lastLogoutTime": 0,
            "lastName": "Prop",
            "lat": 32.797291898342145,
            "lng": -117.24351527372028,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "None xyz",
            "sms": "",
            "type": "u",
            "updatedAt": 1625667495000,
            "zipCode": "92109",
            "userRef": 10,
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VK6iwMLAOwR8KNagKU1cHu2NXTL2/0srQ8yFHbVpDqEhtVBAd?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633651037&Signature=g6C8eWaujT5GAwQBXzN5kCSMhOyeHa%2Fo%2Fqiv%2BT24VLj16LbSzKCVsjIpiqFmQFZ56q4GIA6IKLTYoQ8qrCFUBrRhmXxS3%2BAgdePWHH%2BB4%2F71TIj3WAocgJixpdpIpqjloNAHk3rrDais9t8JqCSJ2vkKdfw4Kl7eZVdrCYUAmGo6WBbtFk%2FkN%2FkF9ezD2yFqUhbFqhjWznLrFChOjJzW1Rrwm8iPgwVEgZ6z9CB8MX%2FAU8lyWrhripD8h6%2FNlq%2B6gKC%2FQXCuNmiigFAy6Q0TqkT11GXg3fhnHVo0Zgi76dI0qVXypEBtoID9BdBx36FbO31r0qq%2FbD%2FjLZLyLD6QCg%3D%3D"
            },
            "userId": 10
        },
        {
            "attributes": [],
            "challenges": "!!!!!!!jkkghjghjhg",
            "createdAt": 1617839288000,
            "disabled": null,
            "email": "yuishean@gmail.com",
            "firstName": "Matt",
            "fullName": "Matt Chen",
            "geohash": "9mueksxy3r",
            "helpingOut": "",
            "id": 22,
            "initialPersona": 0,
            "keywords": [
                "m",
                "ma",
                "mat",
                "matt",
                "matt",
                "matt c",
                "matt ch",
                "matt che",
                "matt chen",
                "c",
                "ch",
                "che",
                "chen"
            ],
            "lastLoginTime": 1632929787391,
            "lastLogoutTime": 1632929787391,
            "lastName": "Chen",
            "lat": 32.94086965214003,
            "lng": -117.2134142493164,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "",
            "sms": "324324",
            "type": "u",
            "updatedAt": 1632929787391,
            "zipCode": "92130",
            "userRef": 11,
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633651037&Signature=Iy7vvoc0AjVCdKDIwJqSDQNOXQiLdP0fzFqIVaY0jFzRh3WWJSfMvCiMcDn%2FaqLW8m%2B%2BAtQFJn9vz5pA3%2FTFsRXBzqTwCik8bxWaOQkrmrSxVeHNiRKqt4tQ96jVgvVLPJrf3NlvTmtuhv7gm5wAR9MBcZ4OnRVTg5Xi29PoAj7ZiWsyhdqh8%2FZnIVztmzgdfBx8fLHUIFkVx25yxNQXHDPoSu0nOPVoVCbS697v6%2Bu8UB5Wllh%2FRZ89%2B7bvkvBJMKLh%2BV3dAz4XTkTuB4ppVG%2F8UYKeA9OoYfZe1mA3FdORKMtTQm8dzBtKUKeJMxB2QsOO%2BF9d0jIzvm4Nmp68ZA%3D%3D"
            },
            "userId": 11
        }
    ],
    "activeRecipients": [
        {
            "attributes": [],
            "challenges": "",
            "createdAt": 1625839286000,
            "disabled": null,
            "email": "mewtwo6271@gmail.com",
            "firstName": "Andy",
            "fullName": "Andy Lee",
            "geohash": "c23p86uf5s",
            "helpingOut": "",
            "id": 1019,
            "initialPersona": 2,
            "keywords": [
                "a",
                "an",
                "and",
                "andy",
                "andy ",
                "andy l",
                "andy le",
                "andy lee",
                "l",
                "le",
                "lee"
            ],
            "lastLoginTime": 1625839286000,
            "lastLogoutTime": 0,
            "lastName": "Lee",
            "lat": 47.74008340941491,
            "lng": -122.3260837528106,
            "locationName": "Seattle, WA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "",
            "sms": "",
            "type": "u",
            "updatedAt": 1625839305000,
            "zipCode": "98133",
            "userRef": 3,
            "avatarKey": null,
            "userId": 3
        },
        {
            "attributes": [
                "Veteran"
            ],
            "challenges": "New challenge to test save. ",
            "createdAt": 1619526930000,
            "disabled": null,
            "email": "trevor@familyproud.com",
            "firstName": "Trevor ",
            "fullName": "Trevor  Prop",
            "geohash": "9muds49fh4",
            "helpingOut": "Pick up foo",
            "id": 23,
            "initialPersona": 1,
            "keywords": [
                "t",
                "tr",
                "tre",
                "trev",
                "trevo",
                "trevor",
                "trevor ",
                "trevor  ",
                "trevor  p",
                "trevor  pr",
                "trevor  pro",
                "trevor  prop",
                "trevor  prop ",
                "trevor  prop v",
                "trevor  prop ve",
                "trevor  prop vet",
                "trevor  prop vete",
                "trevor  prop veter",
                "trevor  prop vetera",
                "trevor  prop veteran",
                "p",
                "pr",
                "pro",
                "prop",
                "v",
                "ve",
                "vet",
                "vete",
                "veter",
                "vetera",
                "veteran"
            ],
            "lastLoginTime": 1619526930000,
            "lastLogoutTime": 0,
            "lastName": "Prop",
            "lat": 32.797291898342145,
            "lng": -117.24351527372028,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "None xyz",
            "sms": "",
            "type": "u",
            "updatedAt": 1625667495000,
            "zipCode": "92109",
            "userRef": 10,
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VK6iwMLAOwR8KNagKU1cHu2NXTL2/0srQ8yFHbVpDqEhtVBAd?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633651037&Signature=g6C8eWaujT5GAwQBXzN5kCSMhOyeHa%2Fo%2Fqiv%2BT24VLj16LbSzKCVsjIpiqFmQFZ56q4GIA6IKLTYoQ8qrCFUBrRhmXxS3%2BAgdePWHH%2BB4%2F71TIj3WAocgJixpdpIpqjloNAHk3rrDais9t8JqCSJ2vkKdfw4Kl7eZVdrCYUAmGo6WBbtFk%2FkN%2FkF9ezD2yFqUhbFqhjWznLrFChOjJzW1Rrwm8iPgwVEgZ6z9CB8MX%2FAU8lyWrhripD8h6%2FNlq%2B6gKC%2FQXCuNmiigFAy6Q0TqkT11GXg3fhnHVo0Zgi76dI0qVXypEBtoID9BdBx36FbO31r0qq%2FbD%2FjLZLyLD6QCg%3D%3D"
            },
            "userId": 10
        },
        {
            "attributes": [],
            "challenges": "!!!!!!!jkkghjghjhg",
            "createdAt": 1617839288000,
            "disabled": null,
            "email": "yuishean@gmail.com",
            "firstName": "Matt",
            "fullName": "Matt Chen",
            "geohash": "9mueksxy3r",
            "helpingOut": "",
            "id": 22,
            "initialPersona": 0,
            "keywords": [
                "m",
                "ma",
                "mat",
                "matt",
                "matt",
                "matt c",
                "matt ch",
                "matt che",
                "matt chen",
                "c",
                "ch",
                "che",
                "chen"
            ],
            "lastLoginTime": 1632929787391,
            "lastLogoutTime": 1632929787391,
            "lastName": "Chen",
            "lat": 32.94086965214003,
            "lng": -117.2134142493164,
            "locationName": "San Diego, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "",
            "sms": "324324",
            "type": "u",
            "updatedAt": 1632929787391,
            "zipCode": "92130",
            "userRef": 11,
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633651037&Signature=Iy7vvoc0AjVCdKDIwJqSDQNOXQiLdP0fzFqIVaY0jFzRh3WWJSfMvCiMcDn%2FaqLW8m%2B%2BAtQFJn9vz5pA3%2FTFsRXBzqTwCik8bxWaOQkrmrSxVeHNiRKqt4tQ96jVgvVLPJrf3NlvTmtuhv7gm5wAR9MBcZ4OnRVTg5Xi29PoAj7ZiWsyhdqh8%2FZnIVztmzgdfBx8fLHUIFkVx25yxNQXHDPoSu0nOPVoVCbS697v6%2Bu8UB5Wllh%2FRZ89%2B7bvkvBJMKLh%2BV3dAz4XTkTuB4ppVG%2F8UYKeA9OoYfZe1mA3FdORKMtTQm8dzBtKUKeJMxB2QsOO%2BF9d0jIzvm4Nmp68ZA%3D%3D"
            },
            "userId": 11
        }
    ],
    "events": [],
    "media": []
}
```

##### :warning: Response Error

```json
null
```

##### :ab: Response Type Error

```json
ValidationError: Expected { id: string; nickname: string | null; isGroup: boolean; isPrivate: boolean; lastEventId: string | null; recipientsIndex: string; keywords: string[]; lastUpdated: number; createdAt: number; muted: boolean; lastChecked: number; read: boolean; avatarKey: { uri: string; } | null; allRecipients: ({ id: string; userId: string; } & { avatarKey: { uri: string; } | null; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; })[]; activeRecipients: ({ id: string; userId: string; } & { avatarKey: { uri: string; } | null; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; })[]; events: { id: string; eventType: "message"; conversationId: string; conversationMemberId: string; text: string; createdAt: number; updatedAt: number; user: { id: string; userId: string; } & { avatarKey: { uri: string; } | null; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; attachmentsMap: { [_: string]: { id: string; conversationId: string; eventId: string; mediaType: "image"; ref: { uri: string; }; createdAt: number; } }; }[]; media: { id: string; conversationId: string; eventId: string; mediaType: "image"; ref: { uri: string; }; createdAt: number; }[]; }, but was incompatible
```

##### :mag_right: Verification Cases

### Find Conversation

> Route: **conversation.find**
> Time elapsed: **0.711s**
> Variations successful: 0/1


#### Variation 1 (0.710s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "recipients": [
        "1"
    ]
}
```

##### :package: Response Data

```json
null
```

##### :warning: Response Error

```json
Error: Request failed with status code 500
    at createError (/Users/matteuc/Desktop/Family Proud/FamilyProudCloud/function-tests/node_modules/axios/lib/core/createError.js:16:15)
    at settle (/Users/matteuc/Desktop/Family Proud/FamilyProudCloud/function-tests/node_modules/axios/lib/core/settle.js:17:12)
    at IncomingMessage.handleStreamEnd (/Users/matteuc/Desktop/Family Proud/FamilyProudCloud/function-tests/node_modules/axios/lib/adapters/http.js:269:11)
    at IncomingMessage.emit (events.js:327:22)
    at endReadableNT (internal/streams/readable.js:1327:12)
    at processTicksAndRejections (internal/process/task_queues.js:80:21)
```

##### :ab: Response Type Error

```json
null
```

##### :mag_right: Verification Cases

