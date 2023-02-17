# X-RAY
`its purpose`: helps developers analys and debug applications (Tracing system / performance monitoring system)

`what is the meaning of Disturbed Tracing`: is a method used to profile and monitor apps espcially those built using microservice architecture.

### similar services like X-RAY:
(datadog / NewRelic /  )

### X-RAY is a Distributed system:
- collects the data about requests
- view/filter collected data to identify issues and help to optimize it

example of profiling:

<img width="1324" alt="image" src="https://user-images.githubusercontent.com/55510819/219717337-f96ed442-2966-45e3-8ec1-0324b512f4e3.png">


### The Anatomy of X-RAY:
1- X-Ray console:
here where the data could be represneted


2- X-Ray daemon:
 is a software application that listens for traffic on UDP port 2000, gathers raw segment data, and relays it to the AWS X-Ray API.


3- X-Ray API:
The X-Ray API provides access to all X-Ray functionality through the AWS SDK, AWS Command Line Interface, or directly over HTTPS.



4- X-Ray SDK:
the part that send the requests to the console it could be written in many programming languages (python/ ruby / js)


### image to identify the connection between X-Ray components:
<img width="1177" alt="image" src="https://user-images.githubusercontent.com/55510819/219718591-93ac93d4-cae5-4192-9de2-175f5be5eb5d.png">

Note: X-Ray Deamon need to be run in a sperate EC2/ECS Task to serve the app

note: Xray recieves the data as segments 

## service graph
- just a represntation of the backend/frontend services
<img width="1177" alt="image" src="https://user-images.githubusercontent.com/55510819/219758913-982614f0-28f8-4542-a241-c2b107913699.png">


## segments
<img width="1177" alt="image" src="https://user-images.githubusercontent.com/55510819/219759564-312f1d55-d05e-4a4d-83dc-3dfa1953cb19.png">


## sampling
- xray uses sampling algorithm to determine which request could be traced
- by default it records `the first request each second` and `5% addetional requests`


## Trace Header
- all requests traced , up to a configrable minimum. after reaching that minimum, a precentage of a requests are traced to avoid unncessary costs

## filter expressions
<img width="1177" alt="image" src="https://user-images.githubusercontent.com/55510819/219761967-79c63ff6-be1f-4ecc-8311-9cba32d4cad6.png">


## annotation and metadata
 - you could pass extra data in the subsequance
<img width="1177" alt="image" src="https://user-images.githubusercontent.com/55510819/219762394-00974097-419a-447f-9f29-67c1bb3c8d11.png">


## what AWS service that we could intergrate xray to it?
1. Lambda
2. API Gatway
3. ELB
4. SNS
5. SQS
6. EC2 / ECS / ECS Faragate
7. EB




## X-Ray CheatSheet
<img width="956" alt="image" src="https://user-images.githubusercontent.com/55510819/219765114-8f7acd51-393a-4f1a-9525-3dcea4487b03.png">

<img width="1177" alt="image" src="https://user-images.githubusercontent.com/55510819/219765239-8c349828-f11e-4eb0-ac1a-23a90d9e15f0.png">







 
