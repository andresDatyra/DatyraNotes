
# Circle Invite API Test Report

**Report Generated On**: Thu Sep 30 2021 15:28:05 GMT-0700 (Pacific Daylight Time)
**API Methods Tested**: 4

## Table of Contents

A. [Test Results](#test-results):

- 1. [Accept Circle invite](#accept-circle-invite) :x:


- 2. [Decline Circle invite](#decline-circle-invite) :white_check_mark:


- 3. [Get Circle Invite](#get-circle-invite) :x:


- 4. [Send Circle Invites](#send-circle-invites) :x:


## Test Results

### Accept Circle invite

> Route: **circle_invite.accept**
> Time elapsed: **0.582s**
> Variations successful: 0/1


#### Variation 1 (0.582s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "33",
    "inviteId": "7"
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

### Decline Circle invite

> Route: **circle_invite.decline**
> Time elapsed: **0.518s**
> Variations successful: 1/1


#### Variation 1 (0.518s) :white_check_mark:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "33",
    "inviteId": "7"
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

### Get Circle Invite

> Route: **circle_invite.get**
> Time elapsed: **0.597s**
> Variations successful: 0/1


#### Variation 1 (0.597s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41",
    "inviteId": "159"
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

### Send Circle Invites

> Route: **circle_invite.send**
> Time elapsed: **0.940s**
> Variations successful: 0/1


#### Variation 1 (0.938s) :x:

> Verification cases passed: 0/1

##### :rocket: Payload Data

```json
{
    "circleId": "41",
    "users": [
        {
            "userId": "3"
        }
    ],
    "message": "This is an invite from Family Proud QA!",
    "emails": [
        {
            "email": "matt@familyproud.com",
            "userName": "Matt"
        }
    ],
    "phoneNumbers": []
}
```

##### :package: Response Data

```json

[]

/* For this preview, a max of 5 items shown */

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


###### Verify that all invites are returned (0.000s) :x:
> Confirm that the number of invites submitted matches the number of invites returned.

```
Not all invites were sent.
```