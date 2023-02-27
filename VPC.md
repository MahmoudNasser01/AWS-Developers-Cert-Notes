## Definishon

is a Virtual Private Cloud allow users to have their own isolate netowrk in AWS cloud



## why we need VPC
 VPC provides the user with the ability to define and customize their network infrastructure, such as IP addressing, subnets and route tables, as well as configure security and access control. It also provides the user with the ability to leverage AWS features such as Amazon EC2, Amazon RDS, and Amazon S3 that require a VPC. Additionally, it allows users to connect their VPC to their own datacenter, as well as other VPCs, allowing for a more secure and flexible network architecture.
 
 
 ## what is the subnet
 - allow you partition your network inside the VPC


## public subnet
- is the subnet that accessible via the internet 

## private subnet
- not accessible via the internet

`Note`: to define access to the internet between the subnet we use `Route Table`

## internet gateway
- help our VPC to access the outside internet

## Nat Gatway
- allow your instances in a private subnet to access the internet while staying private


## NACL
- a firewall which controls the traffic from and to the subnet
- Can Allow and Deny rules
- attach to subnet level
- Rules only include Ip address eg.(I want to allow all traffic from the following IPs and Deny from the following IPs)

<img width="378" alt="image" src="https://user-images.githubusercontent.com/55510819/221479685-89bc43e3-60d8-4559-bbf1-24db089c3b41.png">

`Note`: we could apply NACL and Security group togather to make high level of security


## VPC flow logs
- capture information about ip traffic going into your instances:
 - VPC flow
 - subnet flow logs
 - Elastic Network Interface flow logs
- help you to monitor and troubleshoot connection issues 


## Endpoints
- allow you to connect to AWS services using a private network instead of public network
- connection between (private subnet and AWS services)

## VPC Peering
- allow you to connect your VPCs togather


## Important Architecture come in the exam
<img width="1063" alt="image" src="https://user-images.githubusercontent.com/55510819/221482586-bcaebdf3-9eaf-4854-8284-e0fa566589d9.png">


 
