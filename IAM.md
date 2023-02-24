`IAM` : dentity and Access Managment, Global services

`Root Account`: created by default, shouldn't be used or shared.

`Users`: All users accounts in your orgnasiation

`Groups`: only contains users


`Policies`: is the permmisions in AWS

`inline Policies`: its a type of policies that you could attach to a specific user.

`JSON Policiy structure`:

<img width="1363" alt="image" src="https://user-images.githubusercontent.com/55510819/221179908-cb23c68e-21f2-4b86-94f0-05bee100989b.png">


`IAM Roles`: just normal accounts as users but it only used for AWS services (not human users)

`IAM security Tool`: 
- IAM creds report : report that lists all the users and their credentials
- IAM Access Advisor: shows the service permissions granted to a user and when those services was accessed.


## IAM Best Practices

- Don't use root account accept for account setup
- One Pyhcial user = One AWS user (do not share the creds for the users)
- Assign users to groups and assign permissions to groups
- create a strong password policy
- use Mulit factor auth (MFA)
- Create Roles when you want to give permissions to services
- Use Access keys for programmatic access (CLI/SDKs)
- Manage and monitor your users and permissions using IAM creds report

