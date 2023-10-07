# Three-tier-web-app-in-AWS
I'm going to demonstrate how to set up basic networking and deploy a simple three-tier application in the AWS Cloud.

Services used: 
* VPC
* ALB
* EC2
* RDS

## Description:
A Three-Tier Web Application in AWS refers to a scalable and highly available architecture designed to host and deliver web-based services or applications. This architecture is organized into three distinct layers, each serving a specific purpose and providing flexibility, fault tolerance, and ease of management. Here's a breakdown of these tiers:

### Presentation Tier (Web Tier):

The top layer is the presentation tier, also known as the web tier. It is responsible for interacting with users and presenting the user interface of the application.
This tier typically consists of web servers, such as Amazon EC2 instances running web server software like Apache, Nginx, or Microsoft IIS.
It handles user requests, serves static content like HTML, CSS, and JavaScript files, and forwards dynamic requests to the application tier.
Elastic Load Balancers (ELB) are often used to distribute incoming traffic across multiple web server instances for load balancing and redundancy.
Application Tier (Logic Tier):

The middle layer is the application tier, also known as the logic tier. It contains the core business logic and application functionality.
Application servers, such as EC2 instances or AWS Elastic Beanstalk environments, run in this tier. These servers execute the code that processes user requests, communicates with databases, and performs other application-specific tasks.
Auto Scaling is commonly employed to dynamically adjust the number of application server instances based on traffic demands. AWS services like AWS Elastic Container Service (ECS) or AWS Lambda can also be used for containerized or serverless application deployments.
Data Tier (Database Tier):

The bottom layer is the data tier, responsible for storing and managing the application's data.
Databases, such as Amazon RDS (Relational Database Service), Amazon DynamoDB (NoSQL database), or Amazon Redshift (data warehousing), are deployed in this tier.
Data tier components ensure data integrity, availability, and scalability. Features like automated backups, replication, and caching are often used to enhance data management.
Key Benefits of a Three-Tier Web Application in AWS:

Scalability: Each tier can be independently scaled to handle varying levels of traffic and workloads.
High Availability: AWS provides tools and features like Auto Scaling, load balancers, and Multi-AZ deployments to ensure high availability and fault tolerance.
Security: AWS offers robust security features, including VPC (Virtual Private Cloud) configurations, IAM (Identity and Access Management), and encryption options, to protect data and applications.
Flexibility: Developers can choose from a wide range of programming languages, frameworks, and database technologies to build and customize their applications.
Managed Services: AWS offers managed services like AWS Elastic Beanstalk, RDS, and Lambda, which simplify infrastructure management and reduce operational overhead.
In summary, a Three-Tier Web Application in AWS is a versatile architecture that leverages the cloud's capabilities to build and operate web applications efficiently, reliably, and securely. It enables developers to focus on building and enhancing their applications while AWS handles the underlying infrastructure and scalability concerns.


Screenshots:
![database](https://github.com/pixelpix13/Three-tier-web-app-in-AWS/assets/70488966/7b71fc43-b152-4aa1-9f5e-0210cc57fa8f)
![ec2_instances](https://github.com/pixelpix13/Three-tier-web-app-in-AWS/assets/70488966/0b4378d9-d395-4e9d-baae-67cfbc726ce9)
![elastic_ip](https://github.com/pixelpix13/Three-tier-web-app-in-AWS/assets/70488966/3746216c-2833-4ce6-9f46-176e63c41338)
![internet_gateway](https://github.com/pixelpix13/Three-tier-web-app-in-AWS/assets/70488966/c84c3fe2-026d-481a-9f57-5d507fd249e3)
![Load_Balancer](https://github.com/pixelpix13/Three-tier-web-app-in-AWS/assets/70488966/9696474e-e913-4784-968c-9aaea1c8e135)
![nat_gateway](https://github.com/pixelpix13/Three-tier-web-app-in-AWS/assets/70488966/c20b5a48-ed3f-41f8-895d-fa30315f74d0)
![routetable](https://github.com/pixelpix13/Three-tier-web-app-in-AWS/assets/70488966/8209abfd-5a25-435f-9aa1-54297428da30)
![subnet](https://github.com/pixelpix13/Three-tier-web-app-in-AWS/assets/70488966/3cc34893-7d35-4456-b01d-6a3d77e69f1a)
![target_group](https://github.com/pixelpix13/Three-tier-web-app-in-AWS/assets/70488966/3a977749-880a-40ad-818a-541c7d00de5a)
![vpc](https://github.com/pixelpix13/Three-tier-web-app-in-AWS/assets/70488966/b0bc69a8-68ff-480c-99a1-1dec05a93ecf)
![website_database](https://github.com/pixelpix13/Three-tier-web-app-in-AWS/assets/70488966/e72ff486-64c6-448a-bb87-63dd57e8df81)

