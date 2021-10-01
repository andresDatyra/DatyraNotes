
# Care Map API Test Report

**Report Generated On**: Thu Sep 30 2021 15:13:01 GMT-0700 (Pacific Daylight Time)
**API Methods Tested**: 1

## Table of Contents

A. [Test Results](#test-results):

- 1. [List Care Map markers](#list-care-map-markers) :x:


## Test Results

### List Care Map markers

> Route: **care_map.list_markers**
> Time elapsed: **3.089s**
> Variations successful: 0/4


#### Variation 1 (3.038s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "query": "test"
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



#### Variation 2 (3.046s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "entityType": "user"
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



#### Variation 3 (0.853s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "entityType": "circle"
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



#### Variation 4 (0.548s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "entityType": "circle",
    "query": "test",
    "bounds": {
        "northEast": {
            "latitude": 32,
            "longitude": -117
        },
        "southWest": {
            "latitude": 33,
            "longitude": -118
        }
    }
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

