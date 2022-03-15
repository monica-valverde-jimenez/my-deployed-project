#My deployed project [my-deployed-project]

This repo contains a full configuration to deploy a Full-Stack application. It includes a started Udagram project with api project and frontend project. Also configuration files to run Circle CI, deploy to elastic beanstalk and S3 bucket.


##Circle CI Status

[![CircleCI](https://circleci.com/gh/monica-valverde-jimenez/my-deployed-project/tree/master.svg?style=svg)](https://circleci.com/gh/monica-valverde-jimenez/my-deployed-project/tree/master)


## Deployment process and Infrastructure

Go to [Document deployment process](/docs/Process.md).

## Getting Started

1. Clone this repo locally into the location of your choice.
2. Open a terminal and navigate to the root of the repo
3. follow the instructions in the installation step

### Udagram-api
    1. Create a .env file with the following information:

```
POSTGRES_USERNAME = ''
POSTGRES_PASSWORD = ''
POSTGRES_DB = ''
PORT = ''
POSTGRES_HOST = ''
AWS_REGION = ''
AWS_PROFILE = ''
AWS_BUCKET = ''
URL = ''
JWT_SECRET = ''

```

### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

### Installation

Provision the necessary AWS services needed for running the application:

1. In AWS, provision a publicly available RDS database running Postgres. <Place holder for link to classroom article>
2. In AWS, provision a s3 bucket for hosting the uploaded files. <Place holder for tlink to classroom article>
3. Export the ENV variables needed or use a package like [dotnev](https://www.npmjs.com/package/dotenv)/.
4. From the root of the repo, navigate udagram-api folder `cd starter/udagram-api` to install the node_modules `npm install`. After installation is done start the api in dev mode with `npm run dev`.
5. Without closing the terminal in step 1, navigate to the udagram-frontend `cd starter/udagram-frontend` to intall the node_modules `npm install`. After installation is done start the api in dev mode with `npm run start`.

6. ## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
2. `npm run test`
3. `npm run e2e`
4. There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## License

[License](LICENSE.txt)
