# Antra SEP java evaluation project
## 1. Setup the environment and make it run.
 All three projects are Sprintboot application.<br>

 Need to setup AWS SNS/SQS/S3 in order to use the async API.(Videos in LMS)<br>

 Make sure to update your <i>application.properties</i> file with your AWS IAM account secrets and region.(Videos in LMS)

 AWS Lambda(Sending email) is optional. Code is in [sendEmailCode.py](./lambda/sendEmailCode.py)

## 2. Understand the structure and details
Look at the [ReportingSystemArchitecture.pdf](./ReportingSystemArchitecture.pdf)

## 3. Make improvement in the code/system level.
Suggestions:
1. Add new features like update/delete/edit report.
2. Improve sync API performance by using multithreading and sending request concurrently to both services.
3. Use a database instead of hashmap in the ExcelRepositoryImpl.
4. Improve code coverage by adding more tests.
5. Convert sync API into microservices by adding Eureka/Ribbon support.
6. Add pressure tests to benchmark the system.
7. Change MongoDB to DynamoDB.
8. Fix bugs.
9. Make the system more robust by adding fault tolerance such like : DeadLetter Queue, retry, cache, fallback etc.
10. Add security and jwt support.
11. Add more fancy UI using angular/react.
12. Setup your CI/CD pipeline.
13. Add new Services like PNGService, JPEGService etc
14. ...
