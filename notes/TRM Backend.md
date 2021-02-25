---
attachments: [path_enviroment.png]
title: TRM Backend
created: '2021-02-25T22:21:40.340Z'
modified: '2021-02-25T23:13:59.837Z'
---

# TRM Backend

## Back-end App with Serverless, NodeJS and Apollo

### Pre-requisites
- NodeJS 10.x+ - https://github.com/creationix/nvm or https://nodejs.org/en/
- Serverless framework `npm install serverless -g` -> https://serverless.com/
- Node Gyp `npm install -g node-gyp` -> https://github.com/nodejs/node-gyp#installation
- Sequelize `npm install -g sequelize cli` -> https://github.com/nodejs/node-gyp#installation


#### Node Gyp - On Windows

Install the current version of Python from the [Microsoft Store package](https://docs.python.org/3/using/windows.html#the-microsoft-store-package).

Install tools and configuration manually:

- Install Visual C++ Build Environment: [Visual Studio Build Tools](https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools) (using "Visual C++ build tools" workload) or [Visual Studio 2017 Community](https://visualstudio.microsoft.com/pl/thank-you-downloading-visual-studio/?sku=Community) (using the "Desktop development with C++" workload)

#### Sequelize - On Windows
- After successful installation you should see something like this

```
C:\Users\YOUR_USER\AppData\Roaming\npm\sequelize -> C:\Users\YOUR_USER\AppData\Roaming\npm\node_modules\sequelize-cli\lib\sequelize C:\Users\YOUR_USER\AppData\Roaming\npm — sequelize-cli@3.0.0
```
- Copy path to environmental variables (don’t forget the backslash)
```
 C:\Users\YOUR_USER\AppData\Roaming\npm\
```

<p align="center">
  <img src="https://github.com/andresDatyra/DatyraNotes/blob/main/attachments/path_enviroment.png" width="400" alt="Notable">
</p>

### DEVELOPMENT Workflow

#### Install node dependencies
- `npm install`

#### Set-up environment vars
copy `.env.example` file to a `.env.staging` file, and change its values

#### Set-up database
- create mysql schema named `trm-staging`
- use name as DB env variable on .env file
- Create database tables - `npm run migrate:staging`
- add SLS_COGNITO_IDENTITY_ID=1234 on .env file(will use this as userId to seed data to mysql)
- Add table data - `npm run seed:staging`

#### You are ready to kick off! Run server locally
- comment `serverless-webpack` plugin on serverless.yml on development(doesn't work well yet or not properly configured w/ serverless-offline)
- `npm run start:staging`
- open playground -> http://localhost://3000/graphql/private 

#### You can also test your SNS subscriber functions/lambdas
- SNS filter doesn't seem to work with sns-serverless-offline plugin. follow workaround on next line
- uncomment the SNS subscription w/ no filters on serverless/subscribers/onboardingUpdate.yml & salesforceUpdate.yml 
- simulate a salesforce update -> `npm run sns:salesforceUpdate` 
- check package.json, scripts field for more SNS simulation scripts

#### Scheduled tasks workflow
- `npm run startSnsServer`
- `npm run schedule`

### DEPLOYMENT Workflow

#### Set-up your AWS account. 
Create your AWS Account

#### After doing so, add environment variables!
- Follow this guide - https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-envvars.html

#### configure your domain and certificates
- Edit `serverless.yml` file, where customDomain config is specified

#### Create your sub-domain using a script
`STAGE=prod sls create_domain`

#### Deploy your app
`STAGE=prod sls deploy`

#### Contribute and have fun!

### Resources/Tools
- https://github.com/apollographql/apollo-server/tree/master/packages/apollo-server-lambda
- https://github.com/dherault/serverless-offline
- https://github.com/mj1618/serverless-offline-sns
- https://github.com/serverless-heaven/serverless-webpack
- https://serverless.com/framework/docs/providers/aws/guide/serverless.yml
- https://sequelize.org/v5/

### Patterns/scaffolding
- as you can see on src folder, we have db, graphql, scripts, services, subscribers, utils - folders. let's provide some explanation to understand what those folders mean

#### src/db
- all related to database. migration files, configurations, seed data, data models, seeders.
- migrations - create/update/delete tables/indices/columns. - https://sequelize.org/v5/manual/migrations.html
- config - can be set per environment. TODO: improve the current implementation.
- seeders - can migrate data from existing databases. can add sample data. and it should be able to delete seeded data as well
- models - definition of tables, validation layer, associations, table-specific functions. - https://sequelize.org/v5/manual/migrations.html
- primary resource/documentation - https://sequelize.org/v5

#### src/graphql
- contains all the apollo graphQL endpoints
- contains HOF/HOC(Higher order components/functions) 
- totally separate code per specific endpoint. 
- TODO: create common folder, and add repeated code in the to keep the application DRY(dont repeat yourself) compliant :)
- https://github.com/Urigo/merge-graphql-schemas
- https://github.com/apollographql/apollo-server/tree/master/packages/apollo-server-lambda
- https://github.com/prisma-labs/graphql-playground

#### src/scripts
- any type of script that we can execute locally. what we have so far, are scripts that can trigger SNS subscription(s)

#### src/services
- code to encapsulate business logic. should be reusable across the entire app

#### src/subscribers
- a lambda can subscribe to a lot of AWS events. right now, we subscribe to SNS topics & cognito hooks
- https://github.com/mj1618/serverless-offline-sns
- https://serverless.com/framework/docs/providers/aws/guide/serverless.yml

#### src/utils
- mini-modules / helpers / utilities. they are like services, but on a lower level. examples: logger, file system, etc.

Should you have any questions, feel free to send Theo a message on slack :)
