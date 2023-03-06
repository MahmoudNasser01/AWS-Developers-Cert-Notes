







# Gateway load balancer

- Deploy, scale, manage of 3rd party in AWS

## How it works
- first it send your request to somewhere else to analyize it for example and then forword it again to the distnation

<img width="356" alt="image" src="https://user-images.githubusercontent.com/55510819/223112075-0eb7d22f-fd10-46df-80b5-390e5b413d18.png">


Note: It uses GENEVE protocol on port 6081

## What can be target for GLB:
- EC2 - Private IP addresses


# Sticky Sessions
- make you be able to assign a single clinet to be redrected to the same place each time
- it works using a Cookies


# Cross-Zone load balancing
- each LB instance will distributed the traffic evenly accross diffrent AZ

for example:
<img width="1050" alt="image" src="https://user-images.githubusercontent.com/55510819/223116008-8a168025-3bd6-4914-93e4-0eccd5a006bb.png">



# SSL certs
- An SSL certificate allows traffic between your clients and your load balancer 

- how LB handle SSL certs:
- <img width="1050" alt="image" src="https://user-images.githubusercontent.com/55510819/223118231-da68ffd3-70ce-4c31-8898-2dae79c14ad7.png">





