
# Circle Request API Test Report

**Report Generated On**: Thu Sep 30 2021 16:07:47 GMT-0700 (Pacific Daylight Time)
**API Methods Tested**: 1

## Table of Contents

A. [Test Results](#test-results):

- 1. [List Circle requests](#list-circle-requests) :white_check_mark:
  2. [Create Circle Join Request](#create-circle-join-request) :x:
  3. [Accept Circle Join Request](#accept-circle-join-request) :x:
  4. [Decline Circle Join Request](#decline-circle-join-request) :x:
  5. CircleRequestRemove (Manual QA Needed)


## Test Results

### List Circle requests

> Route: **circle_request.list**
> Time elapsed: **0.889s**
> Variations successful: 1/1


#### Variation 1 (0.887s) :white_check_mark:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41"
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

### Create Circle Join Request

> Route: **circle_request.create**
> Time elapsed: **0.693s**
> Variations successful: 0/1


#### Variation 1 (0.693s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "1"
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

### Accept Circle Join Request

> Route: **circle_request.accept**
> Time elapsed: **0.980s**
> Variations successful: 0/1


#### Variation 1 (0.978s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "153",
    "requestId": "36"
}
```

##### :package: Response Data

```json
452
```

##### :warning: Response Error

```json
null
```

##### :ab: Response Type Error

```json
ValidationError: Expected string, but was number
```

##### :mag_right: Verification Cases

### Decline Circle Join Request

> Route: **circle_request.decline**
> Time elapsed: **0.769s**
> Variations successful: 1/1


#### Variation 1 (0.768s) :white_check_mark:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "153",
    "requestId": "36"
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

