## CrossAccount S3 Access 

- Why set up cross-account access? 

  By setting up cross-account access we don't need to create individual IAM users in each account. In addition, users don't have to sign out of one account and sign in to another to access resources in different AWS accounts. 
  
- Use-case 

  In this tutorial, imagine that the Production account is where live applications are managed. The Development Account is a sandbox where developers can freely test applications. In each account, application information is stored in Amazon S3 buckets. You manage an AWS EC2 instance in the Development account which acts as a sandbox. Users via sandbox Ec2 can work in the Development account and access resources there. From time to time, a developer must update the live applications in the Production account. These applications are stored in an Amazon S3 bucket called productionapp. 
  
  Developers can now access the productionapp bucket in the Production account via an AWS EC2 instance in the Development account. They can also access the bucket by using API calls that are authenticated by temporary credentials provided by the role.
