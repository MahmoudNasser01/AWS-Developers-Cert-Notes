
## ECS Archtecture:

`Task Definition`:
A task definition is a blueprint for a container-based application that specifies details such as which Docker image to use, 
the resources needed for the container, and networking information. 
A task definition can include one or more containers, and it can be versioned and updated as needed.


`Task`:
A task is an instance of a task definition that runs on a container instance in an ECS cluster. 
A task can include one or more containers that are scheduled to run on the same host, and each container in a task shares the same network namespace, enabling them to communicate with each other easily.


`Container Instances`: 
A container instance is a server that has the Docker engine installed and is running the ECS agent, which communicates with the ECS service. A container instance can run multiple tasks, and it can be part of an auto-scaling group that automatically adds or removes instances based on demand.


`ECS Cluster`:
An ECS cluster is a logical grouping of container instances that are managed as a single unit. A cluster can span multiple Availability Zones, providing high availability and fault tolerance for containerized applications.



<img width="541" alt="image" src="https://user-images.githubusercontent.com/55510819/230994523-59da9890-9d8b-4001-a6f0-f19a7bc98040.png">


