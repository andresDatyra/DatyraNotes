
# Circle Member API Test Report

**Report Generated On**: Thu Sep 30 2021 15:35:20 GMT-0700 (Pacific Daylight Time)
**API Methods Tested**: 3

## Table of Contents

A. [Test Results](#test-results):

- 1. [List Circle members](#list-circle-members) :x:


- 2. [Remove Circle member](#remove-circle-member) :x:


- 3. [Update Circle Member](#update-circle-member) :x:


## Test Results

### List Circle members

> Route: **circle_member.list**
> Time elapsed: **3.339s**
> Variations successful: 0/2


#### Variation 1 (2.090s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41"
}
```

##### :package: Response Data

```json

[
    {
        "id": 41,
        "role": 1,
        "createdAt": 1619624560000,
        "updatedAt": 1619624560000,
        "user": {
            "id": 10,
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
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VK6iwMLAOwR8KNagKU1cHu2NXTL2/0srQ8yFHbVpDqEhtVBAd?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633646117&Signature=BALfwUyqtSPZjyrTHgMFF1MsmS1nRisxP%2F%2FtprIIChOVYfDGX1rmJEkbdW%2B2Jt%2F7O1HgmvH3EJTOspqzf9MnrN5F%2FyrOT4ZkIeO%2FhgpDDTcIqPNtxFFNBOzq6doNh6mkTyRj14s1C2R1O%2B336Q9o%2FemLOpkioXcezG%2FnfNKA0Tt9AQy5u20SQqoB47hKnAkQ%2Fe%2FuFtcLyNNZec%2BSqxVtbUE2hLO8nZwHMxFRHw6enm%2B1NML4SCk6PP22csyCgQeg2rmycFvD1LG8NuZezQSesr%2FZxNZ5z95cOQSVpn4q1M7pYDyFth23n7Rx2MbKZtvpy69VYYImq367slj4YD6Auw%3D%3D"
            }
        },
        "userId": 10,
        "circleId": 41
    },
    {
        "id": 48,
        "role": 3,
        "createdAt": 1617839325000,
        "updatedAt": 1617839325000,
        "user": {
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
            "attributes": [],
            "challenges": "!!!!!!!jkkghjghjhg",
            "createdAt": 1617839288000,
            "disabled": null,
            "email": "yuishean@gmail.com",
            "firstName": "Matt",
            "fullName": "Matt Chen",
            "geohash": "9mueksxy3r",
            "helpingOut": "",
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/VYB6TVNitAX42UwA64qwOSBg2hM2/swOZon3nvUaMWr56F4yC?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633646117&Signature=hXkV7MuDWaFlX%2F%2F%2B5tglOf1iIYJuLeIYyB4ZUa8v8f8GnXeaulOMNtVeiq7mwLlp1GEmXEBkE%2BfeqV5wyGm06NCwSfF%2BY8OBhT6E8L7jZxjXnrRA3pqrfWrOBjGHXJsEyGt%2BPTxb7kIZNWZSpKieRIAK2iIjjMBznNIl2HvZC0HTwEI5nl8YGH%2BFfr1EmB%2BMMUmDEZYPODnREmRhjSN4R%2FrnR19fJzT9HhFYNJDqS%2FRgiDs3a1Va9jS%2B66QYsdKj4YsIVDDEtBIxsMafXlzxYDFIp8PIM9rwib4J3Q98LVOHjGcRa%2FpJNmPkwOcIeyaTJ7thSDfAuQcVbisi8ImMfA%3D%3D"
            }
        },
        "userId": 11,
        "circleId": 41
    },
    {
        "id": 50,
        "role": 1,
        "createdAt": 1619628547000,
        "updatedAt": 1619628547000,
        "user": {
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
            "attributes": [],
            "challenges": "",
            "createdAt": 1618340400000,
            "disabled": null,
            "email": "yui.shean@gmail.com",
            "firstName": "John",
            "fullName": "John Doe",
            "geohash": "9muex16ry6",
            "helpingOut": "",
            "avatarKey": null
        },
        "userId": 13,
        "circleId": 41
    },
    {
        "id": 61,
        "role": 1,
        "createdAt": 1617989126000,
        "updatedAt": 1617989126000,
        "user": {
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
            "attributes": [],
            "challenges": "",
            "createdAt": 1617973033000,
            "disabled": null,
            "email": "aren6271@gmail.com",
            "firstName": "Andy",
            "fullName": "Andy Ren",
            "geohash": "c23p8e2sc8",
            "helpingOut": "",
            "avatarKey": null
        },
        "userId": 19,
        "circleId": 41
    },
    {
        "id": 69,
        "role": 1,
        "createdAt": 1619624566000,
        "updatedAt": 1619624566000,
        "user": {
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
            "attributes": [],
            "challenges": "",
            "createdAt": 1619559297000,
            "disabled": null,
            "email": "ray@familyproud.com",
            "firstName": "Ray",
            "fullName": "Ray Corchado",
            "geohash": "9mu9q95s24",
            "helpingOut": "",
            "avatarKey": {
                "uri": "https://storage.googleapis.com/fp-native-dev.appspot.com/users/vdsQVod3uTO3gKEFpoK42zOOeu43/BkeRshngPg1Cb7U33fbZ?GoogleAccessId=fp-native-dev%40appspot.gserviceaccount.com&Expires=1633646117&Signature=C7G3zaAtpuGV3l0gJmFKE2v71UI4S0pBNrKRknWvA7lSolBFxMnWgzF8U02zdm2HP7%2BMJrxMR%2B%2B5ugNVMKGCXCnJLS8XWAYvdXHClSW0Qoj6IiJplc4FLN3DCMSqLUJgDz4suRj6WL%2BKg5phB7A5C96C%2B72E8qv0g7ZEn4kgfaQkdcbfQh2PfVanFohqOUVl4iYHGIH3IUq1vUmyH4D%2B2CvGNTZcohRR6SkYNHgIWGIGmhchVzOVo7vmWNwzsnvZqbPOpeZsYV9i56HWxDInLXiuxgdYbxu59tn01umgtPKS4hRGJu5Dhn35be8J5CzLVeXDkhfbhqtXS%2B0Az8KQkg%3D%3D"
            }
        },
        "userId": 22,
        "circleId": 41
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
ValidationError: Expected { id: string; role: 0 | 1 | 2 | 3; createdAt: number; updatedAt: number; userId: string; circleId: string; user: { avatarKey: { uri: string; } | null; id: string; organizationId: string | null; firstName: string; lastName: string; fullName: string; locationName: string; zipCode: string; lat: number; lng: number; helpingOut: string; ownNeeds: string; challenges: string; attributes: string[]; keywords: string[]; createdAt: number; updatedAt: number; mapVisibility: boolean; disabled?: boolean; }; }[], but was incompatible
```

##### :mag_right: Verification Cases



#### Variation 2 (3.307s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41",
    "before": 1633041283288
}
```

##### :package: Response Data

```json
null
```

##### :warning: Response Error

```json
Error: Request failed with status code 422
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

### Remove Circle member

> Route: **circle_member.remove**
> Time elapsed: **0.495s**
> Variations successful: 0/1


#### Variation 1 (0.494s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41",
    "memberId": "50"
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

### Update Circle Member

> Route: **circle_member.update**
> Time elapsed: **1.519s**
> Variations successful: 0/1


#### Variation 1 (1.518s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41",
    "memberId": "41",
    "update": {
        "role": 2
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

