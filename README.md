# AWS-Developers-Cert-Notes


# Elastic BeansTalk

- think about it as heroku of the AWS (highly automated)
- not reommended if you want full customization

- in EB you have to diffrentae between the Web environment and the Worker Environment
<img width="940" alt="image" src="https://user-images.githubusercontent.com/55510819/218367034-844d7ff0-302d-4d61-9d27-b464b295d997.png">


- there is 2 types of EB web environments (Load Balanced Env / single instance env)

load balanced) using load balance feature and also auto scaling

single) not using load balance to save cost and also still have the auto scaling

<img width="940" alt="image" src="https://user-images.githubusercontent.com/55510819/218367597-f79e3eb6-8b57-4a6f-8ad8-3a2a8aa465d1.png">




## Deployment methods

## 1 All at once
<img width="940" alt="image" src="https://user-images.githubusercontent.com/55510819/218367856-10b9d87c-6c41-484c-b7e6-93d029c0588f.png">


## 2 Rolling
<img width="940" alt="image" src="https://user-images.githubusercontent.com/55510819/218368005-1700eb12-a747-4a37-bda7-1920b2cb7b76.png">

## 3 Rolling With Additional Batch
<img width="940" alt="image" src="https://user-images.githubusercontent.com/55510819/218368157-aa1c2f04-bad5-4c9f-890f-98dbde16d22a.png">


## 4 Immutable
<img width="940" alt="image" src="https://user-images.githubusercontent.com/55510819/218368546-639f36c4-2b7a-4bfd-9810-f612c0a21060.png">



<img width="1130" alt="image" src="https://user-images.githubusercontent.com/55510819/216828476-fc24279e-9ac9-4dc1-8557-48f9d533505b.png">



## In-place vs Blue/Green Deplyments
<img width="1130" alt="image" src="https://user-images.githubusercontent.com/55510819/216828700-bf4e205e-e076-458c-95a7-d0e1cd49c1e4.png">

<img width="1130" alt="image" src="https://user-images.githubusercontent.com/55510819/216828788-26bf3a10-3abe-4dfd-a079-c60c2cf7c0cc.png">


note: if the switch happend in the same ENV then it will be concidered as In-place otherwise it will be Blue/Green depoyment
note: Blue/Green with EB requires that your Database is outside the ENV because in Blue/Green method the old ENV is destroyed and replaced with another one.

## server configrations
<img width="1130" alt="image" src="https://user-images.githubusercontent.com/55510819/216830027-e232263f-c2e0-4918-8238-8370c86ac6f2.png">


## EB cheet sheet
<img width="1370" alt="image" src="https://user-images.githubusercontent.com/55510819/216830257-f0b15f6b-1555-45ed-bc2f-5bbe02b3e159.png">

<img width="1370" alt="image" src="https://user-images.githubusercontent.com/55510819/216830285-b8746ecb-51fd-4588-8dc6-8322cdb89206.png">












