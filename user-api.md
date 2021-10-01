
# User API Test Report

**Report Generated On**: Thu Sep 30 2021 15:10:39 GMT-0700 (Pacific Daylight Time)
**API Methods Tested**: 11

## Table of Contents

A. [Test Results](#test-results):

- 1. [Block User](#block-user) :white_check_mark:


- 2. [Create User](#create-user) :x:


- 3. [Get User](#get-user) :x:


- 4. [List User Notifications](#list-user-notifications) :x:


- 5. [List User Recipients](#list-user-recipients) :x:


- 6. [List Users](#list-users) :x:


- 7. [Mark all notifications seen](#mark-all-notifications-seen) :white_check_mark:


- 8. [Mark notification seen](#mark-notification-seen) :white_check_mark:


- 9. [Register User Token](#register-user-token) :white_check_mark:


- 10. [Report User](#report-user) :x:


- 11. [Submit User Feedback](#submit-user-feedback) :white_check_mark:


## Test Results

### Block User

> Route: **user.block**
> Time elapsed: **1.033s**
> Variations successful: 2/2


#### Variation 1 (1.032s) :white_check_mark:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "userId": "3",
    "blocked": true
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



#### Variation 2 (0.963s) :white_check_mark:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "userId": "3",
    "blocked": false
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

### Create User (IGNORE: Manual QA Needed)

> Route: **user.create**
> Time elapsed: **0.526s**
> Variations successful: 0/1


#### Variation 1 (0.526s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "firstName": "QA",
    "lastName": "Member",
    "zipCode": "92130",
    "email": "qa.team+1633039793858@familyproud.com",
    "mapVisibility": false
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


***

### Get User

> Route: **user.info**
> Time elapsed: **1.276s**
> Variations successful: 0/1


#### Variation 1 (1.271s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{}
```

##### :package: Response Data

```json
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
    "id": 11,
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
    "notificationOptions": {
        "email": {
            "circleInvite": true,
            "conversationMessage": true
        },
        "sms": {
            "circleInvite": true,
            "conversationMessage": true
        },
        "push": {
            "circleInvite": true,
            "claimedAsk": false,
            "newAsk": true,
            "conversationMessage": true
        }
    },
    "onBoardingComplete": true,
    "onboardingProgress": null,
    "organizationId": null,
    "ownNeeds": "",
    "sms": "324324",
    "type": "u",
    "updatedAt": 1632929787391,
    "zipCode": "92130",
    "avatarKey": {
        "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633644630&Signature=TWpNJl32vUYpOs4GFgFNaERUMZdWL3DjNovcNdEQ95lCZOv3eFYBaEcqxCJc2aRi3G9J2tGJw3L1%2FbUKt2W3mwoyqiuzljHC3hsq6EZ%2BqF2CgMxfBmjkgzbK8IiYPsVJRk2HViyacBhsbdkuBS4W%2FDKtdyGw9jxVfRnh%2FyUakwvScUXeSoULj%2FU0PURmjQF4EAm1D0tDdlmEW1NoleYXa57%2FLULBQVRn%2FUdMJP0OT9rR4JpelL3XnXh7Bv7%2B59G%2FH4fB7SlVYVIMkoGNWxQlJc3ZlDfhLBVA%2FsUZN8glTg6skvKVu5ygvtJx2IKpiv6WIKwQur2SP66D1jtM%2F4sSpg%3D%3D"
    },
    "blockedUsers": [
        "0",
        "1"
    ]
}
```

##### :warning: Response Error

```json
null
```

##### :ab: Response Type Error

```json
ValidationError: Expected { avatarKey: { uri: string; } | null; blockedUsers: string[]; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; email: string; onBoardingComplete: boolean; sms: string; locationName: string; zipCode: string; lat: number; lng: number; initialPersona: 0 | 1 | 2; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; notificationOptions: { push: { conversationMessage: boolean; circleInvite: boolean; claimedAsk: boolean; newAsk: boolean; newPost: boolean; newPostComment: boolean; }; sendMessageHandler: { conversationMessage: boolean; circleInvite: boolean; }; email: { conversationMessage: boolean; circleInvite: boolean; }; }; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }, but was incompatible
```

##### :mag_right: Verification Cases


***

### List User Notifications

> Route: **user.list_notifications**
> Time elapsed: **1.829s**
> Variations successful: 0/1


#### Variation 1 (1.826s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{}
```

##### :package: Response Data

```json

[
    {
        "askId": 29,
        "circleRef": 52,
        "commentId": null,
        "createdAt": 1619642548000,
        "eventType": "new-ask",
        "id": 128,
        "inviteId": null,
        "joinRequestId": null,
        "postId": null,
        "seen": true,
        "userRef": 11,
        "event": {
            "attachmentMap": {
                "items": [
                    24
                ]
            },
            "circleRef": {
                "circleId": 52,
                "organizationId": null
            },
            "claimedAt": 1619652243000,
            "claimerUserRef": {
                "userId": 10,
                "organizationId": null
            },
            "createdAt": 1619642548000,
            "description": "Everyone enjoys a warm meal!",
            "endAt": 1619818939000,
            "id": 29,
            "intervalPeriod": 0,
            "location": null,
            "refId": null,
            "startAt": 1619815339000,
            "title": "Meal Delivery",
            "updatedAt": 1619642548000,
            "userRef": {
                "userId": 22,
                "organizationId": null
            },
            "userId": 22,
            "circleId": 52,
            "claimerUserId": 10,
            "attachment": null,
            "author": {
                "lastName": "Corchado",
                "zipCode": "91932",
                "keywords": [
                    "r",
                    "ra",
                    "ray",
                    "ray ",
                    "ray c",
                    "ray co",
                    "ray cor",
                    "ray corc",
                    "ray corch",
                    "ray corcha",
                    "ray corchad",
                    "ray corchado",
                    "c",
                    "co",
                    "cor",
                    "corc",
                    "corch",
                    "corcha",
                    "corchad",
                    "corchado"
                ],
                "challenges": "",
                "organizationId": null,
                "lastLogoutTime": 0,
                "createdAt": 1619559297000,
                "onBoardingComplete": true,
                "geohash": "9mu9q95s24",
                "sms": "",
                "id": 22,
                "email": "ray@familyproud.com",
                "lat": 32.56971131543735,
                "initialPersona": 0,
                "updatedAt": 1619559636000,
                "ownNeeds": "",
                "mapVisibility": true,
                "locationName": "Imperial Beach, CA",
                "lng": -117.13141383094215,
                "fullName": "Ray Corchado",
                "firstName": "Ray",
                "lastLoginTime": 1619559297000,
                "helpingOut": "",
                "attributes": [],
                "avatarKey": {
                    "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/vdsQVod3uTO3gKEFpoK42zOOeu43/BkeRshngPg1Cb7U33fbZ?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633644631&Signature=N54Y%2Bbp5VOsxi8HY5%2BJapSXERjWQ8ajTC7HMJ6j5dZ%2FH3OtLvfyE7VcdSpVnCM%2BJlhx72O9Md4t34rtXm75bVK%2FfPl0fjHmkhhrvARyEVZHEBhcN28%2FDlzoIMcuX%2FBEyLrZNnxWJUoXM%2F7Lfl823C8iTOspWOS1q%2B6F6BXyKoOdHfleMaB5OKPPAHgjJfFu6AmLM5wZc8F5VdzuDU1TowyKFefINS2PEvdduJinesJH3QwgAXee3XMqlW6Uaz%2BqZzd7bmvaxtsPHiz2%2BnsppNy7a76ztYO3LcMfWjnMUpY5ymkEgDmI93dHS%2BrqSoaz0nGrjxqWjzrVwPOGalOWvQQ%3D%3D"
                }
            },
            "claimer": {
                "lastName": "Prop",
                "zipCode": "92109",
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
                "challenges": "New challenge to test save. ",
                "organizationId": null,
                "lastLogoutTime": 0,
                "createdAt": 1619526930000,
                "onBoardingComplete": true,
                "geohash": "9muds49fh4",
                "sms": "",
                "id": 10,
                "email": "trevor@familyproud.com",
                "lat": 32.797291898342145,
                "initialPersona": 1,
                "updatedAt": 1625667495000,
                "ownNeeds": "None xyz",
                "mapVisibility": true,
                "locationName": "San Diego, CA",
                "lng": -117.24351527372028,
                "fullName": "Trevor  Prop",
                "firstName": "Trevor ",
                "lastLoginTime": 1619526930000,
                "helpingOut": "Pick up foo",
                "attributes": [
                    "Veteran"
                ],
                "avatarKey": {
                    "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VK6iwMLAOwR8KNagKU1cHu2NXTL2/0srQ8yFHbVpDqEhtVBAd?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633644631&Signature=KjwPp0vny3sGOfeo2xDWiqOw6cPEDJSoVQaSYd%2FZQoWYM3RriDIBgoWk0sVBpf6bPNhywv4kvxljeygc0f%2Byy8wYrAYlaV94fcFrYiX2f5L53caW2AIRqfa9Uy%2FrBIB2jZZ6NAgdNoEEHBNB2SzbUbkq3Rx9PF7hPdgH6OfHS%2FbqAklEw50qmqMGjsaRXMO9WcgHJHRuFMIuNmobdHtQUfBz6MWUw6idsHrAs17GGAufq1dQO9hB4EPwk8BTclkjvPUAMR%2FsjZDOB7rtZD2DFY0OxEXa9s9r1AlBN34BH00n76tcdxvbozuJ2HT8cJlg25RSiCJtxo5XQ1d3vxqwpA%3D%3D"
                }
            }
        }
    },
    {
        "askId": 5,
        "circleRef": 33,
        "commentId": null,
        "createdAt": 1619465028000,
        "eventType": "claimed-ask",
        "id": 129,
        "inviteId": null,
        "joinRequestId": null,
        "postId": null,
        "seen": true,
        "userRef": 11,
        "event": {
            "attachmentMap": {
                "items": [
                    7
                ]
            },
            "circleRef": {
                "circleId": 33,
                "organizationId": null
            },
            "claimedAt": 1619465764000,
            "claimerUserRef": {
                "userId": 13,
                "organizationId": null
            },
            "createdAt": 1618402134000,
            "description": "Everyone enjoys a warm meal!",
            "endAt": 1618405727000,
            "id": 5,
            "intervalPeriod": 0,
            "location": null,
            "refId": null,
            "startAt": 1618402127000,
            "title": "Meal Delivery",
            "updatedAt": 1618402134000,
            "userRef": {
                "userId": 11,
                "organizationId": null
            },
            "userId": 11,
            "circleId": 33,
            "claimerUserId": 13,
            "attachment": null,
            "author": {
                "lastName": "Chen",
                "zipCode": "92130",
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
                "challenges": "!!!!!!!jkkghjghjhg",
                "organizationId": null,
                "lastLogoutTime": 1632929787391,
                "createdAt": 1617839288000,
                "onBoardingComplete": true,
                "geohash": "9mueksxy3r",
                "sms": "324324",
                "id": 11,
                "email": "yuishean@gmail.com",
                "lat": 32.94086965214003,
                "initialPersona": 0,
                "updatedAt": 1632929787391,
                "ownNeeds": "",
                "mapVisibility": true,
                "locationName": "San Diego, CA",
                "lng": -117.2134142493164,
                "fullName": "Matt Chen",
                "firstName": "Matt",
                "lastLoginTime": 1632929787391,
                "helpingOut": "",
                "attributes": [],
                "avatarKey": {
                    "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633644631&Signature=D0y2Sfq0Ay9fifgbagO28jEwaFzw%2FpWjSi79IeUm3jb9a0KIlwcc08y3zDJkKsUUQv5NcicC3%2FDGf%2B0VDDWiMmj0TKhQkAYqjFMPnCPI%2BUJ%2FjxGNsahYfrMJNq9V7oOtCJqVEkN13TttjzlQAbu1D%2F07yloT0mVZ1Gw%2FrVjOyhge3yzk8rWbeBqWNQmwBn3kapYAUy%2B%2B6h6PLZ1cxoaDqXSF5aUzF1AySYmIrHYLBp5amToRQFlEhEggGTpBx692MD0JGXNkyWAtdrwgcSVPZ2RYNuEukxcZeUNaEIovcBYnp9TCp8ZJbon2OgsCXFLoZ6qCWEuA4L1tsmJdYBE8ew%3D%3D"
                }
            },
            "claimer": {
                "lastName": "Doe",
                "zipCode": "92129",
                "keywords": [
                    "j",
                    "jo",
                    "joh",
                    "john",
                    "john ",
                    "john d",
                    "john do",
                    "john doe",
                    "d",
                    "do",
                    "doe"
                ],
                "challenges": "",
                "organizationId": null,
                "lastLogoutTime": 0,
                "createdAt": 1618340400000,
                "onBoardingComplete": true,
                "geohash": "9muex16ry6",
                "sms": "",
                "id": 13,
                "email": "yui.shean@gmail.com",
                "lat": 32.96719645384466,
                "initialPersona": 2,
                "updatedAt": 1625652308000,
                "ownNeeds": "",
                "mapVisibility": true,
                "locationName": "San Diego, CA",
                "lng": -117.11089061513302,
                "fullName": "John Doe",
                "firstName": "John",
                "lastLoginTime": 1618340400000,
                "helpingOut": "",
                "attributes": [],
                "avatarKey": null
            }
        }
    },
    {
        "askId": 5,
        "circleRef": 33,
        "commentId": null,
        "createdAt": 1619465076000,
        "eventType": "claimed-ask",
        "id": 130,
        "inviteId": null,
        "joinRequestId": null,
        "postId": null,
        "seen": true,
        "userRef": 11,
        "event": {
            "attachmentMap": {
                "items": [
                    7
                ]
            },
            "circleRef": {
                "circleId": 33,
                "organizationId": null
            },
            "claimedAt": 1619465764000,
            "claimerUserRef": {
                "userId": 13,
                "organizationId": null
            },
            "createdAt": 1618402134000,
            "description": "Everyone enjoys a warm meal!",
            "endAt": 1618405727000,
            "id": 5,
            "intervalPeriod": 0,
            "location": null,
            "refId": null,
            "startAt": 1618402127000,
            "title": "Meal Delivery",
            "updatedAt": 1618402134000,
            "userRef": {
                "userId": 11,
                "organizationId": null
            },
            "userId": 11,
            "circleId": 33,
            "claimerUserId": 13,
            "attachment": null,
            "author": {
                "lastName": "Chen",
                "zipCode": "92130",
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
                "challenges": "!!!!!!!jkkghjghjhg",
                "organizationId": null,
                "lastLogoutTime": 1632929787391,
                "createdAt": 1617839288000,
                "onBoardingComplete": true,
                "geohash": "9mueksxy3r",
                "sms": "324324",
                "id": 11,
                "email": "yuishean@gmail.com",
                "lat": 32.94086965214003,
                "initialPersona": 0,
                "updatedAt": 1632929787391,
                "ownNeeds": "",
                "mapVisibility": true,
                "locationName": "San Diego, CA",
                "lng": -117.2134142493164,
                "fullName": "Matt Chen",
                "firstName": "Matt",
                "lastLoginTime": 1632929787391,
                "helpingOut": "",
                "attributes": [],
                "avatarKey": {
                    "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633644631&Signature=D0y2Sfq0Ay9fifgbagO28jEwaFzw%2FpWjSi79IeUm3jb9a0KIlwcc08y3zDJkKsUUQv5NcicC3%2FDGf%2B0VDDWiMmj0TKhQkAYqjFMPnCPI%2BUJ%2FjxGNsahYfrMJNq9V7oOtCJqVEkN13TttjzlQAbu1D%2F07yloT0mVZ1Gw%2FrVjOyhge3yzk8rWbeBqWNQmwBn3kapYAUy%2B%2B6h6PLZ1cxoaDqXSF5aUzF1AySYmIrHYLBp5amToRQFlEhEggGTpBx692MD0JGXNkyWAtdrwgcSVPZ2RYNuEukxcZeUNaEIovcBYnp9TCp8ZJbon2OgsCXFLoZ6qCWEuA4L1tsmJdYBE8ew%3D%3D"
                }
            },
            "claimer": {
                "lastName": "Doe",
                "zipCode": "92129",
                "keywords": [
                    "j",
                    "jo",
                    "joh",
                    "john",
                    "john ",
                    "john d",
                    "john do",
                    "john doe",
                    "d",
                    "do",
                    "doe"
                ],
                "challenges": "",
                "organizationId": null,
                "lastLogoutTime": 0,
                "createdAt": 1618340400000,
                "onBoardingComplete": true,
                "geohash": "9muex16ry6",
                "sms": "",
                "id": 13,
                "email": "yui.shean@gmail.com",
                "lat": 32.96719645384466,
                "initialPersona": 2,
                "updatedAt": 1625652308000,
                "ownNeeds": "",
                "mapVisibility": true,
                "locationName": "San Diego, CA",
                "lng": -117.11089061513302,
                "fullName": "John Doe",
                "firstName": "John",
                "lastLoginTime": 1618340400000,
                "helpingOut": "",
                "attributes": [],
                "avatarKey": null
            }
        }
    },
    {
        "askId": 6,
        "circleRef": 33,
        "commentId": null,
        "createdAt": 1619464593000,
        "eventType": "claimed-ask",
        "id": 132,
        "inviteId": null,
        "joinRequestId": null,
        "postId": null,
        "seen": true,
        "userRef": 11,
        "event": {
            "attachmentMap": {
                "items": [
                    6
                ]
            },
            "circleRef": {
                "circleId": 33,
                "organizationId": null
            },
            "claimedAt": 1619464938000,
            "claimerUserRef": {
                "userId": 13,
                "organizationId": null
            },
            "createdAt": 1618401866000,
            "description": "Everyone enjoys a warm meal!!!",
            "endAt": 1618405461000,
            "id": 6,
            "intervalPeriod": 0,
            "location": null,
            "refId": null,
            "startAt": 1618401861000,
            "title": "Meal Delivery",
            "updatedAt": 1618402118000,
            "userRef": {
                "userId": 11,
                "organizationId": null
            },
            "userId": 11,
            "circleId": 33,
            "claimerUserId": 13,
            "attachment": null,
            "author": {
                "lastName": "Chen",
                "zipCode": "92130",
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
                "challenges": "!!!!!!!jkkghjghjhg",
                "organizationId": null,
                "lastLogoutTime": 1632929787391,
                "createdAt": 1617839288000,
                "onBoardingComplete": true,
                "geohash": "9mueksxy3r",
                "sms": "324324",
                "id": 11,
                "email": "yuishean@gmail.com",
                "lat": 32.94086965214003,
                "initialPersona": 0,
                "updatedAt": 1632929787391,
                "ownNeeds": "",
                "mapVisibility": true,
                "locationName": "San Diego, CA",
                "lng": -117.2134142493164,
                "fullName": "Matt Chen",
                "firstName": "Matt",
                "lastLoginTime": 1632929787391,
                "helpingOut": "",
                "attributes": [],
                "avatarKey": {
                    "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633644631&Signature=D0y2Sfq0Ay9fifgbagO28jEwaFzw%2FpWjSi79IeUm3jb9a0KIlwcc08y3zDJkKsUUQv5NcicC3%2FDGf%2B0VDDWiMmj0TKhQkAYqjFMPnCPI%2BUJ%2FjxGNsahYfrMJNq9V7oOtCJqVEkN13TttjzlQAbu1D%2F07yloT0mVZ1Gw%2FrVjOyhge3yzk8rWbeBqWNQmwBn3kapYAUy%2B%2B6h6PLZ1cxoaDqXSF5aUzF1AySYmIrHYLBp5amToRQFlEhEggGTpBx692MD0JGXNkyWAtdrwgcSVPZ2RYNuEukxcZeUNaEIovcBYnp9TCp8ZJbon2OgsCXFLoZ6qCWEuA4L1tsmJdYBE8ew%3D%3D"
                }
            },
            "claimer": {
                "lastName": "Doe",
                "zipCode": "92129",
                "keywords": [
                    "j",
                    "jo",
                    "joh",
                    "john",
                    "john ",
                    "john d",
                    "john do",
                    "john doe",
                    "d",
                    "do",
                    "doe"
                ],
                "challenges": "",
                "organizationId": null,
                "lastLogoutTime": 0,
                "createdAt": 1618340400000,
                "onBoardingComplete": true,
                "geohash": "9muex16ry6",
                "sms": "",
                "id": 13,
                "email": "yui.shean@gmail.com",
                "lat": 32.96719645384466,
                "initialPersona": 2,
                "updatedAt": 1625652308000,
                "ownNeeds": "",
                "mapVisibility": true,
                "locationName": "San Diego, CA",
                "lng": -117.11089061513302,
                "fullName": "John Doe",
                "firstName": "John",
                "lastLoginTime": 1618340400000,
                "helpingOut": "",
                "attributes": [],
                "avatarKey": null
            }
        }
    },
    {
        "askId": 5,
        "circleRef": 33,
        "commentId": null,
        "createdAt": 1619465673000,
        "eventType": "claimed-ask",
        "id": 133,
        "inviteId": null,
        "joinRequestId": null,
        "postId": null,
        "seen": true,
        "userRef": 11,
        "event": {
            "attachmentMap": {
                "items": [
                    7
                ]
            },
            "circleRef": {
                "circleId": 33,
                "organizationId": null
            },
            "claimedAt": 1619465764000,
            "claimerUserRef": {
                "userId": 13,
                "organizationId": null
            },
            "createdAt": 1618402134000,
            "description": "Everyone enjoys a warm meal!",
            "endAt": 1618405727000,
            "id": 5,
            "intervalPeriod": 0,
            "location": null,
            "refId": null,
            "startAt": 1618402127000,
            "title": "Meal Delivery",
            "updatedAt": 1618402134000,
            "userRef": {
                "userId": 11,
                "organizationId": null
            },
            "userId": 11,
            "circleId": 33,
            "claimerUserId": 13,
            "attachment": null,
            "author": {
                "lastName": "Chen",
                "zipCode": "92130",
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
                "challenges": "!!!!!!!jkkghjghjhg",
                "organizationId": null,
                "lastLogoutTime": 1632929787391,
                "createdAt": 1617839288000,
                "onBoardingComplete": true,
                "geohash": "9mueksxy3r",
                "sms": "324324",
                "id": 11,
                "email": "yuishean@gmail.com",
                "lat": 32.94086965214003,
                "initialPersona": 0,
                "updatedAt": 1632929787391,
                "ownNeeds": "",
                "mapVisibility": true,
                "locationName": "San Diego, CA",
                "lng": -117.2134142493164,
                "fullName": "Matt Chen",
                "firstName": "Matt",
                "lastLoginTime": 1632929787391,
                "helpingOut": "",
                "attributes": [],
                "avatarKey": {
                    "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633644631&Signature=D0y2Sfq0Ay9fifgbagO28jEwaFzw%2FpWjSi79IeUm3jb9a0KIlwcc08y3zDJkKsUUQv5NcicC3%2FDGf%2B0VDDWiMmj0TKhQkAYqjFMPnCPI%2BUJ%2FjxGNsahYfrMJNq9V7oOtCJqVEkN13TttjzlQAbu1D%2F07yloT0mVZ1Gw%2FrVjOyhge3yzk8rWbeBqWNQmwBn3kapYAUy%2B%2B6h6PLZ1cxoaDqXSF5aUzF1AySYmIrHYLBp5amToRQFlEhEggGTpBx692MD0JGXNkyWAtdrwgcSVPZ2RYNuEukxcZeUNaEIovcBYnp9TCp8ZJbon2OgsCXFLoZ6qCWEuA4L1tsmJdYBE8ew%3D%3D"
                }
            },
            "claimer": {
                "lastName": "Doe",
                "zipCode": "92129",
                "keywords": [
                    "j",
                    "jo",
                    "joh",
                    "john",
                    "john ",
                    "john d",
                    "john do",
                    "john doe",
                    "d",
                    "do",
                    "doe"
                ],
                "challenges": "",
                "organizationId": null,
                "lastLogoutTime": 0,
                "createdAt": 1618340400000,
                "onBoardingComplete": true,
                "geohash": "9muex16ry6",
                "sms": "",
                "id": 13,
                "email": "yui.shean@gmail.com",
                "lat": 32.96719645384466,
                "initialPersona": 2,
                "updatedAt": 1625652308000,
                "ownNeeds": "",
                "mapVisibility": true,
                "locationName": "San Diego, CA",
                "lng": -117.11089061513302,
                "fullName": "John Doe",
                "firstName": "John",
                "lastLoginTime": 1618340400000,
                "helpingOut": "",
                "attributes": [],
                "avatarKey": null
            }
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
ValidationError: Expected ({ id: string; seen: boolean; createdAt: number; } & ({ eventType: "conversation"; event: { id: string; eventType: "message"; conversationId: string; conversationMemberId: string; text: string; createdAt: number; updatedAt: number; user: { id: string; userId: string; } & { avatarKey: { uri: string; } | null; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; attachmentsMap: { [_: string]: { id: string; conversationId: string; eventId: string; mediaType: "image"; ref: { uri: string; }; createdAt: number; } }; }; } | { eventType: "invite"; event: ({ id: string; status: 0 | 1 | 2; createdAt: number; delivered: boolean; statusChangedAt: number | null; message: string | null; } & { circle: { id: string; organizationId: string | null; nickname: string; avatarKey: { uri: string; } | null; coverKey: { uri: string; } | null; createdAt: number; updatedAt: number; description: string; isPrivate: boolean; memberCount: number; unclaimedAskCount: number; askCount: number; postCount: number; joinRequestCount: number; registryUrl: string | null; zipCode: string; locationName: string; lat: number; lng: number; attributes: string[]; keywords: string[]; venmoUserId?: string | null; creatorUserId: string; joinedOn: number | null; joinRequested: boolean; role: 0 | 1 | 2 | 3; }; inviter: { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; }) & ({ inviteType: "user"; user: { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; } | { inviteType: "email"; userName: string; email: string; } | { inviteType: "sms"; userName: string; phone: string; }); } | { eventType: "new-ask"; event: { id: string; title: string; description: string; attachmentMap: { [_: string]: { id: string; mediaType: "image"; entityType: "ask" | "post"; entityId: string; createdAt: number; userId: string; circleId: string; ref: { uri: string; }; } }; startAt: number; endAt: number; intervalPeriod: number; createdAt: number; updatedAt: number; claimerUserRef: { userId: string; organizationId: string | null; } | null; claimedAt: number | null; location: { lat: number; lng: number; locationName: string | null; address: string; } | null; circleId: string; attachment: { uri: string; } | null; claimerUserId: string | null; author: { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; userId: string; claimer: { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; } | null; }; } | { eventType: "claimed-ask"; event: { id: string; title: string; description: string; attachmentMap: { [_: string]: { id: string; mediaType: "image"; entityType: "ask" | "post"; entityId: string; createdAt: number; userId: string; circleId: string; ref: { uri: string; }; } }; startAt: number; endAt: number; intervalPeriod: number; createdAt: number; updatedAt: number; claimerUserRef: { userId: string; organizationId: string | null; } | null; claimedAt: number | null; location: { lat: number; lng: number; locationName: string | null; address: string; } | null; circleId: string; attachment: { uri: string; } | null; claimerUserId: string | null; author: { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; userId: string; claimer: { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; } | null; }; } | { eventType: "new-post"; event: { id: string; text: string; likeCount: number; commentCount: number; createdAt: number; updatedAt: number; lastCommentId: string | null; user: { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; userId: string; circleId: string; attachmentMap: { [_: string]: { id: string; mediaType: "image"; entityType: "ask" | "post"; entityId: string; createdAt: number; userId: string; circleId: string; ref: { uri: string; }; } }; comments: { id: string; text: string; createdAt: number; updatedAt: number; postId: string; user: { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; userId: string; circleId: string; }[]; liked: boolean; }; } | { eventType: "new-post-comment"; event: { post: { id: string; text: string; likeCount: number; commentCount: number; createdAt: number; updatedAt: number; lastCommentId: string | null; user: { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; userId: string; circleId: string; attachmentMap: { [_: string]: { id: string; mediaType: "image"; entityType: "ask" | "post"; entityId: string; createdAt: number; userId: string; circleId: string; ref: { uri: string; }; } }; comments: { id: string; text: string; createdAt: number; updatedAt: number; postId: string; user: { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; userId: string; circleId: string; }[]; liked: boolean; }; comment: { id: string; text: string; createdAt: number; updatedAt: number; postId: string; user: { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; userId: string; circleId: string; }; }; }))[], but was incompatible
```

##### :mag_right: Verification Cases


***

### List User Recipients

> Route: **user.list_recipients**
> Time elapsed: **1.940s**
> Variations successful: 0/1


#### Variation 1 (1.890s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{}
```

##### :package: Response Data

```json

[
    {
        "attributes": [],
        "challenges": "",
        "createdAt": 1631115438617,
        "disabled": null,
        "email": "eduardo@test.com",
        "firstName": "Eduardo",
        "fullName": "Eduardo Watanabe",
        "geohash": "9mudwj53bh",
        "helpingOut": "",
        "id": 367,
        "initialPersona": 2,
        "keywords": [
            "e",
            "ed",
            "edu",
            "edua",
            "eduar",
            "eduard",
            "eduardo",
            "eduardo",
            "eduardo w",
            "eduardo wa",
            "eduardo wat",
            "eduardo wata",
            "eduardo watan",
            "eduardo watana",
            "eduardo watanab",
            "eduardo watanabe",
            "w",
            "wa",
            "wat",
            "wata",
            "watan",
            "watana",
            "watanab",
            "watanabe"
        ],
        "lastLoginTime": 1631115438617,
        "lastLogoutTime": 0,
        "lastName": "Watanabe",
        "lat": 32.8109928008565,
        "lng": -117.15373312289995,
        "locationName": "San Diego, CA",
        "mapVisibility": true,
        "onBoardingComplete": false,
        "onboardingProgress": null,
        "organizationId": null,
        "ownNeeds": "",
        "sms": "",
        "type": "u",
        "updatedAt": 1631115438617,
        "zipCode": "92123",
        "avatarKey": null
    },
    {
        "attributes": [],
        "challenges": "",
        "createdAt": 1626817511000,
        "disabled": null,
        "email": "ericjbondoc@gmail.com",
        "firstName": "Eric",
        "fullName": "Eric Bondoc",
        "geohash": "9musd8jm3t",
        "helpingOut": "",
        "id": 15,
        "initialPersona": 2,
        "keywords": [
            "e",
            "er",
            "eri",
            "eric",
            "eric ",
            "eric b",
            "eric bo",
            "eric bon",
            "eric bond",
            "eric bondo",
            "eric bondoc",
            "b",
            "bo",
            "bon",
            "bond",
            "bondo",
            "bondoc"
        ],
        "lastLoginTime": 1626817511000,
        "lastLogoutTime": 0,
        "lastName": "Bondoc",
        "lat": 33.135697114743394,
        "lng": -117.30473630561836,
        "locationName": "Carlsbad, CA",
        "mapVisibility": true,
        "onBoardingComplete": true,
        "onboardingProgress": null,
        "organizationId": null,
        "ownNeeds": "",
        "sms": "",
        "type": "u",
        "updatedAt": 1627130288000,
        "zipCode": "92008",
        "avatarKey": null
    },
    {
        "attributes": [],
        "challenges": "",
        "createdAt": 1623268411000,
        "disabled": null,
        "email": "ray@test.com",
        "firstName": "Rayyy",
        "fullName": "Rayyy Test",
        "geohash": "9mu9qed32m",
        "helpingOut": "",
        "id": 17,
        "initialPersona": 0,
        "keywords": [
            "r",
            "ra",
            "ray",
            "rayy",
            "rayyy",
            "rayyy ",
            "rayyy t",
            "rayyy te",
            "rayyy tes",
            "rayyy test",
            "t",
            "te",
            "tes",
            "test"
        ],
        "lastLoginTime": 1623268411000,
        "lastLogoutTime": 0,
        "lastName": "Test",
        "lat": 32.58294499357669,
        "lng": -117.13312043315649,
        "locationName": "Imperial Beach, CA",
        "mapVisibility": true,
        "onBoardingComplete": true,
        "onboardingProgress": null,
        "organizationId": null,
        "ownNeeds": "",
        "sms": "",
        "type": "u",
        "updatedAt": 1623268439000,
        "zipCode": "91932",
        "avatarKey": null
    },
    {
        "attributes": [],
        "challenges": "",
        "createdAt": 1617973033000,
        "disabled": null,
        "email": "aren6271@gmail.com",
        "firstName": "Andy",
        "fullName": "Andy Ren",
        "geohash": "c23p8e2sc8",
        "helpingOut": "",
        "id": 19,
        "initialPersona": 0,
        "keywords": [
            "a",
            "an",
            "and",
            "andy",
            "andy ",
            "andy r",
            "andy re",
            "andy ren",
            "r",
            "re",
            "ren"
        ],
        "lastLoginTime": 1617973033000,
        "lastLogoutTime": 0,
        "lastName": "Ren",
        "lat": 47.74327809807953,
        "lng": -122.32102093253246,
        "locationName": "Seattle, WA",
        "mapVisibility": true,
        "onBoardingComplete": true,
        "onboardingProgress": null,
        "organizationId": null,
        "ownNeeds": "",
        "sms": "",
        "type": "u",
        "updatedAt": 1625839176000,
        "zipCode": "98133",
        "avatarKey": null
    },
    {
        "attributes": [],
        "challenges": "",
        "createdAt": 1618340400000,
        "disabled": null,
        "email": "yui.shean@gmail.com",
        "firstName": "John",
        "fullName": "John Doe",
        "geohash": "9muex16ry6",
        "helpingOut": "",
        "id": 13,
        "initialPersona": 2,
        "keywords": [
            "j",
            "jo",
            "joh",
            "john",
            "john ",
            "john d",
            "john do",
            "john doe",
            "d",
            "do",
            "doe"
        ],
        "lastLoginTime": 1618340400000,
        "lastLogoutTime": 0,
        "lastName": "Doe",
        "lat": 32.96719645384466,
        "lng": -117.11089061513302,
        "locationName": "San Diego, CA",
        "mapVisibility": true,
        "onBoardingComplete": true,
        "onboardingProgress": null,
        "organizationId": null,
        "ownNeeds": "",
        "sms": "",
        "type": "u",
        "updatedAt": 1625652308000,
        "zipCode": "92129",
        "avatarKey": null
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
ValidationError: Expected { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }[], but was incompatible
```

##### :mag_right: Verification Cases


***

### List Users

> Route: **user.list**
> Time elapsed: **1.612s**
> Variations successful: 0/1


#### Variation 1 (1.572s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{}
```

##### :package: Response Data

```json

[
    {
        "attributes": [],
        "challenges": "",
        "createdAt": 1631115438617,
        "disabled": null,
        "email": "eduardo@test.com",
        "firstName": "Eduardo",
        "fullName": "Eduardo Watanabe",
        "geohash": "9mudwj53bh",
        "helpingOut": "",
        "id": 367,
        "initialPersona": 2,
        "keywords": [
            "e",
            "ed",
            "edu",
            "edua",
            "eduar",
            "eduard",
            "eduardo",
            "eduardo",
            "eduardo w",
            "eduardo wa",
            "eduardo wat",
            "eduardo wata",
            "eduardo watan",
            "eduardo watana",
            "eduardo watanab",
            "eduardo watanabe",
            "w",
            "wa",
            "wat",
            "wata",
            "watan",
            "watana",
            "watanab",
            "watanabe"
        ],
        "lastLoginTime": 1631115438617,
        "lastLogoutTime": 0,
        "lastName": "Watanabe",
        "lat": 32.8109928008565,
        "lng": -117.15373312289995,
        "locationName": "San Diego, CA",
        "mapVisibility": true,
        "onBoardingComplete": false,
        "onboardingProgress": null,
        "organizationId": null,
        "ownNeeds": "",
        "sms": "",
        "type": "u",
        "updatedAt": 1631115438617,
        "zipCode": "92123",
        "avatarKey": null
    },
    {
        "attributes": [],
        "challenges": "",
        "createdAt": 1626817511000,
        "disabled": null,
        "email": "ericjbondoc@gmail.com",
        "firstName": "Eric",
        "fullName": "Eric Bondoc",
        "geohash": "9musd8jm3t",
        "helpingOut": "",
        "id": 15,
        "initialPersona": 2,
        "keywords": [
            "e",
            "er",
            "eri",
            "eric",
            "eric ",
            "eric b",
            "eric bo",
            "eric bon",
            "eric bond",
            "eric bondo",
            "eric bondoc",
            "b",
            "bo",
            "bon",
            "bond",
            "bondo",
            "bondoc"
        ],
        "lastLoginTime": 1626817511000,
        "lastLogoutTime": 0,
        "lastName": "Bondoc",
        "lat": 33.135697114743394,
        "lng": -117.30473630561836,
        "locationName": "Carlsbad, CA",
        "mapVisibility": true,
        "onBoardingComplete": true,
        "onboardingProgress": null,
        "organizationId": null,
        "ownNeeds": "",
        "sms": "",
        "type": "u",
        "updatedAt": 1627130288000,
        "zipCode": "92008",
        "avatarKey": null
    },
    {
        "attributes": [],
        "challenges": "",
        "createdAt": 1623268411000,
        "disabled": null,
        "email": "ray@test.com",
        "firstName": "Rayyy",
        "fullName": "Rayyy Test",
        "geohash": "9mu9qed32m",
        "helpingOut": "",
        "id": 17,
        "initialPersona": 0,
        "keywords": [
            "r",
            "ra",
            "ray",
            "rayy",
            "rayyy",
            "rayyy ",
            "rayyy t",
            "rayyy te",
            "rayyy tes",
            "rayyy test",
            "t",
            "te",
            "tes",
            "test"
        ],
        "lastLoginTime": 1623268411000,
        "lastLogoutTime": 0,
        "lastName": "Test",
        "lat": 32.58294499357669,
        "lng": -117.13312043315649,
        "locationName": "Imperial Beach, CA",
        "mapVisibility": true,
        "onBoardingComplete": true,
        "onboardingProgress": null,
        "organizationId": null,
        "ownNeeds": "",
        "sms": "",
        "type": "u",
        "updatedAt": 1623268439000,
        "zipCode": "91932",
        "avatarKey": null
    },
    {
        "attributes": [],
        "challenges": "",
        "createdAt": 1617973033000,
        "disabled": null,
        "email": "aren6271@gmail.com",
        "firstName": "Andy",
        "fullName": "Andy Ren",
        "geohash": "c23p8e2sc8",
        "helpingOut": "",
        "id": 19,
        "initialPersona": 0,
        "keywords": [
            "a",
            "an",
            "and",
            "andy",
            "andy ",
            "andy r",
            "andy re",
            "andy ren",
            "r",
            "re",
            "ren"
        ],
        "lastLoginTime": 1617973033000,
        "lastLogoutTime": 0,
        "lastName": "Ren",
        "lat": 47.74327809807953,
        "lng": -122.32102093253246,
        "locationName": "Seattle, WA",
        "mapVisibility": true,
        "onBoardingComplete": true,
        "onboardingProgress": null,
        "organizationId": null,
        "ownNeeds": "",
        "sms": "",
        "type": "u",
        "updatedAt": 1625839176000,
        "zipCode": "98133",
        "avatarKey": null
    },
    {
        "attributes": [],
        "challenges": "",
        "createdAt": 1618340400000,
        "disabled": null,
        "email": "yui.shean@gmail.com",
        "firstName": "John",
        "fullName": "John Doe",
        "geohash": "9muex16ry6",
        "helpingOut": "",
        "id": 13,
        "initialPersona": 2,
        "keywords": [
            "j",
            "jo",
            "joh",
            "john",
            "john ",
            "john d",
            "john do",
            "john doe",
            "d",
            "do",
            "doe"
        ],
        "lastLoginTime": 1618340400000,
        "lastLogoutTime": 0,
        "lastName": "Doe",
        "lat": 32.96719645384466,
        "lng": -117.11089061513302,
        "locationName": "San Diego, CA",
        "mapVisibility": true,
        "onBoardingComplete": true,
        "onboardingProgress": null,
        "organizationId": null,
        "ownNeeds": "",
        "sms": "",
        "type": "u",
        "updatedAt": 1625652308000,
        "zipCode": "92129",
        "avatarKey": null
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
ValidationError: Expected { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }[], but was incompatible
```

##### :mag_right: Verification Cases


***

### Mark all notifications seen

> Route: **user.mark_all_notifications_seen**
> Time elapsed: **0.459s**
> Variations successful: 1/1


#### Variation 1 (0.459s) :white_check_mark:

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
null
```

##### :ab: Response Type Error

```json
null
```

##### :mag_right: Verification Cases


***

### Mark notification seen

> Route: **user.mark_notification_seen**
> Time elapsed: **0.580s**
> Variations successful: 1/1


#### Variation 1 (0.579s) :white_check_mark:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "notificationId": "126"
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

### Register User Token

> Route: **user.register_token**
> Time elapsed: **0.505s**
> Variations successful: 2/2


#### Variation 1 (0.504s) :white_check_mark:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "token": "123",
    "register": true
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



#### Variation 2 (0.423s) :white_check_mark:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "token": "123",
    "register": false
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

### Report User

> Route: **user.report**
> Time elapsed: **0.612s**
> Variations successful: 0/1


#### Variation 1 (0.612s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "userId": "41",
    "reason": "This is from an automated testing suite."
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

### Submit User Feedback

> Route: **user.submit_feedback**
> Time elapsed: **1.051s**
> Variations successful: 1/1


#### Variation 1 (1.050s) :white_check_mark:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "userName": "Tom Riddle",
    "text": "Hello! This is from an automated testing suite.",
    "email": "iamvoldemort@hogwarts.com",
    "feedbackType": "comment",
    "phone": null
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

