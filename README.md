## Overview
This application is an example of a multi-docker appplication running on AWS Elastic Beanstalk. The application is integrated with [Travis CI](http://travis-ci.org/) and deployed to Elastic Beanstalk using Multicontainer Docker configuration.

- The below diagram shows an overview of the application architecture.

![Architecture](https://github.com/ptadros/multi-docker/blob/master/architecture.png)

## Getting Started

### Development
- You can run the application by executing the following command in the project directory.

```sh
  docker-compose up
```

- Then open the application in the browser through
```
  http://localhost:3050/
```

### production

You need to create the following resources in AWS to prepare production environment

- Create Elastic Beanstalk application and add required environment variables.
- Create Postgres RDS instance.
- Create Redis ElasticCache instance
- Adjust a security group between the above three resources.
- Create a deployment user and place credentials in Travis CI environment variables

## Reference
This application is an exercise application from [Docker and Kubernetes The Complete Guide](https://www.udemy.com/course/docker-and-kubernetes-the-complete-guide/) course.
