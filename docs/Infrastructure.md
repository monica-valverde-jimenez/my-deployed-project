# Infrastructure
My-deployed-project includes the following infrastructure:

### udagram-api
Database: Postgres version 12.9 hosted in RSD.

![Database information](./images/db-info.PNG)

Configuration:

![Database configuration](./images/db-configuration.PNG)

Hosted: Elastic beanstalk

### udagram-frontend
A simple website hosted in S3 bucket. It consumes udagram-api data.

#### Architecture Diagram
![Architecture](./images/aws.drawio.png)


Return to [Process](Process.md).

