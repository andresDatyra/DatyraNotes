
# Circle Ask API Test Report

**Report Generated On**: Thu Sep 30 2021 15:41:28 GMT-0700 (Pacific Daylight Time)
**API Methods Tested**: 6

## Table of Contents

A. [Test Results](#test-results):

- 1. [Claim Circle Ask](#claim-circle-ask) :x:


- 2. [Create Circle Ask](#create-circle-ask) :x:


- 3. [Get Circle Ask](#get-circle-ask) :x:


- 4. [List Claimed Circle Asks](#list-claimed-circle-asks) :x:


- 5. [List Circle Asks](#list-circle-asks) :x:


- 6. [Update Circle Ask](#update-circle-ask) :x:
  7. [Delete Circle Ask](#delete-circle-ask) :x:


## Test Results

### Claim Circle Ask

> Route: **circle_ask.claim**
> Time elapsed: **0.940s**
> Variations successful: 0/2


#### Variation 1 (0.940s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41",
    "askId": "20",
    "claimed": true
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



#### Variation 2 (0.604s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41",
    "askId": "20",
    "claimed": false
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

### Create Circle Ask

> Route: **circle_ask.create**
> Time elapsed: **0.477s**
> Variations successful: 0/1


#### Variation 1 (0.477s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "title": "Family Proud QA - Test Ask",
    "description": "Ask created for Family Proud QA",
    "attachment": null,
    "circleId": "41",
    "startAt": 1633041640917,
    "endAt": 1633045240917
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

### Get Circle Ask

> Route: **circle_ask.get**
> Time elapsed: **0.659s**
> Variations successful: 0/1


#### Variation 1 (0.659s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "askId": "20",
    "circleId": "41"
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

### List Claimed Circle Asks

> Route: **circle_ask.list_claimed**
> Time elapsed: **1.938s**
> Variations successful: 0/1


#### Variation 1 (1.935s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{}
```

##### :package: Response Data

```json

[
    {
        "attachmentMap": {
            "items": [
                19
            ]
        },
        "circleRef": {
            "circleId": 41,
            "organizationId": null
        },
        "claimedAt": 1618441394000,
        "claimerUserRef": {
            "userId": 11,
            "organizationId": null
        },
        "createdAt": 1617839508000,
        "description": "Everyone enjoys a warm meal!",
        "endAt": 1617843101000,
        "id": 20,
        "intervalPeriod": 0,
        "location": null,
        "refId": null,
        "startAt": 1617839501000,
        "title": "Meal Delivery",
        "updatedAt": 1617839508000,
        "userRef": {
            "userId": 11,
            "organizationId": null
        },
        "attachment": {
            "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/circles/OKHAYegYgMUNSVx807Xo/OHSCr1p8GGKvXGhvLxhD?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633646487&Signature=TLHs7NcE6hvkd%2FwtSc5gc1EJAsu5brvwLgOK6fnXyA7wvuiEVNPzmL0gUVpNMA8IOJL2eB9r9w0Ocph3OnB75X6HuvS8FJv4XEKS8y0f8Vwrf2fqo3ucKiG%2FsX7F7bHCf5Z0rUe7g%2BKVOyCfDfPtOZv%2FGQpH3Iyzq%2FMVoSnO%2Bj46nUJXeVisB8hhVVQm0yuN2jp0buLQ8QlXdvpTeXlzuHzQm%2BWebnVoOLPRUXVvIPwwrNQ5OIp5pIrFLweihJi%2FsKp5VmkBUvlY9iCPDyD49M%2Fb2hvS0Y9w1g0GFoVxKbq%2FGQx1t9yU701QCv4G36vMEsYn34osJvFp%2BzaKZYNhHw%3D%3D"
        },
        "claimerUserId": 11,
        "userId": 11,
        "circleId": 41,
        "author": {
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
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "",
            "sms": "324324",
            "type": "u",
            "updatedAt": 1632929787391,
            "zipCode": "92130",
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633646487&Signature=hgV2SqNB1aXB14%2F9PD01ouE6XgSSg8VCSg5ur1MXFfq5cWvH9a%2FT2FeQ6ECIE3cU04QJPj7fVhxpnslMrLxjk7wsEWN2GUcPWguOLMhqDhI3JPDrFqWsqEgo5LUOXfqpAR9IQ26pj4gajNbHcpASxmuHDuCXa%2BM29C1Tnpc2k6dC6Y25DZH8VNdmAmOYu45GmetrlE4445u2VAE4z4GW6r2pjGo1G1tqpIGKgNmfFSuRUAJQl5u5j%2FUoMQ2udsTt9SsgEu3k%2FqOKui03tcMu3aM2UIK0LHsOqzvLImTPjmzQ4t97LnevinT%2Ba008fviLwHkpYzc1drPCKj5YlA0tAw%3D%3D"
            }
        },
        "claimer": {
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
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "",
            "sms": "324324",
            "type": "u",
            "updatedAt": 1632929787391,
            "zipCode": "92130",
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633646487&Signature=hgV2SqNB1aXB14%2F9PD01ouE6XgSSg8VCSg5ur1MXFfq5cWvH9a%2FT2FeQ6ECIE3cU04QJPj7fVhxpnslMrLxjk7wsEWN2GUcPWguOLMhqDhI3JPDrFqWsqEgo5LUOXfqpAR9IQ26pj4gajNbHcpASxmuHDuCXa%2BM29C1Tnpc2k6dC6Y25DZH8VNdmAmOYu45GmetrlE4445u2VAE4z4GW6r2pjGo1G1tqpIGKgNmfFSuRUAJQl5u5j%2FUoMQ2udsTt9SsgEu3k%2FqOKui03tcMu3aM2UIK0LHsOqzvLImTPjmzQ4t97LnevinT%2Ba008fviLwHkpYzc1drPCKj5YlA0tAw%3D%3D"
            }
        }
    },
    {
        "attachmentMap": {
            "items": [
                25
            ]
        },
        "circleRef": {
            "circleId": 52,
            "organizationId": null
        },
        "claimedAt": 1619629542000,
        "claimerUserRef": {
            "userId": 11,
            "organizationId": null
        },
        "createdAt": 1619559529000,
        "description": "I need a Tesla truck",
        "endAt": 1619791200000,
        "id": 28,
        "intervalPeriod": 0,
        "location": null,
        "refId": null,
        "startAt": 1619787600000,
        "title": "But me a tesla",
        "updatedAt": 1619559529000,
        "userRef": {
            "userId": 22,
            "organizationId": null
        },
        "attachment": {
            "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/circles/kwm21MbPNkkFmF4fTu1l/ih2WLB651ZDWAYPJNZHv?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633646487&Signature=O%2BzmhTuYLQKBwnxbm8sC1Qpiw9oNPjCIZ6HEPToHvFEN2a%2F8c7j1kVjBkeCTgHAdJgGIVszAyomFRoFMZp9rujd1VOZQ%2FH1HWzuUlQ%2FO8pm0f5cbiyzBEZT28jvTS3j2Bzvv89NWsSzfEC0hf6We88qsIhpr6dxsU4G30rAG08tqzhzfGYXZSexm0ZjQmgj66DIInxIhSlCC8%2F%2BNKbCTFQkfnOUeMIRgT8ccL1Kn%2FmUwOTPE8EK4sp4L%2FYvZgichOpBHMp8v4v7dlvcJy6LcTlLNJ2e9SgbhsjRKB2ahy79RYNNQUC4iPcTJBEWilr1Ktl0P%2FwnzEOGNYLX8o84qrQ%3D%3D"
        },
        "claimerUserId": 11,
        "userId": 22,
        "circleId": 52,
        "author": {
            "attributes": [],
            "challenges": "",
            "createdAt": 1619559297000,
            "disabled": null,
            "email": "ray@familyproud.com",
            "firstName": "Ray",
            "fullName": "Ray Corchado",
            "geohash": "9mu9q95s24",
            "helpingOut": "",
            "id": 22,
            "initialPersona": 0,
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
            "lastLoginTime": 1619559297000,
            "lastLogoutTime": 0,
            "lastName": "Corchado",
            "lat": 32.56971131543735,
            "lng": -117.13141383094215,
            "locationName": "Imperial Beach, CA",
            "mapVisibility": true,
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "",
            "sms": "",
            "type": "u",
            "updatedAt": 1619559636000,
            "zipCode": "91932",
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/vdsQVod3uTO3gKEFpoK42zOOeu43/BkeRshngPg1Cb7U33fbZ?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633646487&Signature=BzEJsoKxNXwvucyH5HQISsZ1YAZNdkSKDkXTNh10gPjy%2BpD%2FUhvE5i691JVZBhv8u77w31vJjqEqyKPKZUI1GMdipnZ%2FxDOs6XXg5Y8NBjM1H8uk3KrLReVHqRJGccFofbwUtz4021NQ4VK7n5ax%2B%2F7Mq2muFxXNVqHJf4qpUUDO6Sa8ccCVL1CCko96ckmPYENUuBI%2BazycRrhgeCu1fgtVDvOBGo8euf9ks2NOKE%2FnJ%2BBhWzoEXnCaNWnfbM%2Fv1FSFUs24J8jHRx1pf%2BbZU%2B96rpZWIV66rJ8f0jcSR%2Fp1aj1PV6D5AtMPKxBVsgwEJS%2B3pD8I1GdM4x8CWnhFbw%3D%3D"
            }
        },
        "claimer": {
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
            "onBoardingComplete": true,
            "onboardingProgress": null,
            "organizationId": null,
            "ownNeeds": "",
            "sms": "324324",
            "type": "u",
            "updatedAt": 1632929787391,
            "zipCode": "92130",
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633646487&Signature=hgV2SqNB1aXB14%2F9PD01ouE6XgSSg8VCSg5ur1MXFfq5cWvH9a%2FT2FeQ6ECIE3cU04QJPj7fVhxpnslMrLxjk7wsEWN2GUcPWguOLMhqDhI3JPDrFqWsqEgo5LUOXfqpAR9IQ26pj4gajNbHcpASxmuHDuCXa%2BM29C1Tnpc2k6dC6Y25DZH8VNdmAmOYu45GmetrlE4445u2VAE4z4GW6r2pjGo1G1tqpIGKgNmfFSuRUAJQl5u5j%2FUoMQ2udsTt9SsgEu3k%2FqOKui03tcMu3aM2UIK0LHsOqzvLImTPjmzQ4t97LnevinT%2Ba008fviLwHkpYzc1drPCKj5YlA0tAw%3D%3D"
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
ValidationError: Expected { id: string; title: string; description: string; attachmentMap: { [_: string]: { id: string; mediaType: "image"; entityType: "ask" | "post"; entityId: string; createdAt: number; userId: string; circleId: string; ref: { uri: string; }; } }; startAt: number; endAt: number; intervalPeriod: number; createdAt: number; updatedAt: number; claimerUserRef: { userId: string; organizationId: string | null; } | null; claimedAt: number | null; location: { lat: number; lng: number; locationName: string | null; address: string; } | null; circleId: string; attachment: { uri: string; } | null; claimerUserId: string | null; author: { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; userId: string; claimer: { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; } | null; }[], but was incompatible
```

##### :mag_right: Verification Cases


***

### List Circle Asks

> Route: **circle_ask.list**
> Time elapsed: **0.551s**
> Variations successful: 0/1


#### Variation 1 (0.550s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41"
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

### Update Circle Ask

> Route: **circle_ask.update**
> Time elapsed: **0.480s**
> Variations successful: 0/1


#### Variation 1 (0.480s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41",
    "askId": "20",
    "update": {
        "description": "Help us QA the Family Proud app!",
        "title": "Join our QA team!"
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

### Delete Circle Ask

> Route: **circle_ask.delete**
> Time elapsed: **0.626s**
> Variations successful: 0/1


#### Variation 1 (0.625s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41",
    "askId": "20"
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

