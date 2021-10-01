
# Circle Post API Test Report

**Report Generated On**: Thu Sep 30 2021 15:22:39 GMT-0700 (Pacific Daylight Time)
**API Methods Tested**: 8

## Table of Contents

A. [Test Results](#test-results):

- 1. [Create Circle Post Comment](#create-circle-post-comment) :x:


- 2. [Create Circle Post](#create-circle-post) :x:


- 3. [Delete Circle Post](#delete-circle-post) :x:


- 4. [Get Circle Post Comment](#get-circle-post-comment) :x:


- 5. [Get Circle Post](#get-circle-post) :x:


- 6. [Like Circle Post](#like-circle-post) :x:


- 7. [List Circle Post Comments](#list-circle-post-comments) :x:


- 8. [Update Circle Post](#update-circle-post) :x:


## Test Results

### Create Circle Post Comment

> Route: **circle_post.create_comment**
> Time elapsed: **0.681s**
> Variations successful: 0/1


#### Variation 1 (0.680s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41",
    "postId": "27",
    "text": "Hello from Family Proud QA!"
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

### Create Circle Post

> Route: **circle_post.create**
> Time elapsed: **0.508s**
> Variations successful: 0/1


#### Variation 1 (0.507s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "text": "Post created for Family Proud QA",
    "attachments": [],
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

### Delete Circle Post

> Route: **circle_post.delete**
> Time elapsed: **0.567s**
> Variations successful: 0/1


#### Variation 1 (0.567s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "33",
    "postId": "11"
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

### Get Circle Post Comment

> Route: **circle_post.get_comment**
> Time elapsed: **0.497s**
> Variations successful: 0/1


#### Variation 1 (0.497s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "postId": "27",
    "circleId": "41",
    "commentId": "24"
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

### Get Circle Post

> Route: **circle_post.get**
> Time elapsed: **1.513s**
> Variations successful: 0/1


#### Variation 1 (1.513s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "postId": "27",
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

### Like Circle Post

> Route: **circle_post.like**
> Time elapsed: **3.278s**
> Variations successful: 0/2


#### Variation 1 (3.278s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41",
    "postId": "27",
    "liked": true
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



#### Variation 2 (0.483s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41",
    "postId": "27",
    "liked": false
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

### List Circle Post Comments

> Route: **circle_post.list_comments**
> Time elapsed: **0.552s**
> Variations successful: 0/1


#### Variation 1 (0.551s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41",
    "postId": "27"
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

### Update Circle Post

> Route: **circle_post.update**
> Time elapsed: **0.534s**
> Variations successful: 0/1


#### Variation 1 (0.533s) :x:

> Verification cases passed: 0/0

##### :rocket: Payload Data

```json
{
    "circleId": "41",
    "postId": "27",
    "updates": {
        "text": "Hello from Family Proud QA!"
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

