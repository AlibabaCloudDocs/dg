Benefits 
=============================

Database Gateway provides secure, reliable, and cost-effective database connection services.

* Security:
  * Database Gateway does not require you to open the service ports of databases to the Internet because account permissions are authenticated at each network layer. Database Gateway also transmits data over HTTPS to implement natural asymmetric encryption.
  
  * Before a Database Gateway agent establishes a channel to the Database Gateway server, the agent requests the Database Gateway server to assign a token. After the agent receives the token, it encrypts the token and uses the encrypted token to perform identity verification on the Database Gateway server. This ensures that the channel is available to only the user who creates the database gateway. The token expires in 5 minutes after it is generated and can be verified only once.
  
  * Database Gateway transmits data over HTTPS to implement natural asymmetric encryption.
  
  * When you use Alibaba Cloud services to access databases that are not deployed on Alibaba Cloud, you can call API operations to obtain only a list of the database gateways that are created by your account. This prevents unauthorized access to database gateways and on-premises databases that are connected to the database gateways.
  
  * When you use Alibaba Cloud services to access on-premises databases that are connected to a database gateway, you must provide the AccessKey pair and the database gateway ID to pass authentication. This prevents unauthorized access to your on-premises databases.
  
  * When you install and start a Database Gateway agent on an on-premises server, you must provide the Alibaba Cloud account information and the gateway verification code to pass authentication. Channels that are established between Database Gateway agents and Database Gateway are identified by Alibaba Cloud AccessKey pairs and database gateway IDs.
  

  

* Ease of use: Database Gateway does not require complex network and routing configurations. You can use an AccessKey pair to connect your databases to Alibaba Cloud in a few minutes.

* Cost-effectiveness: Database Gateway provides free database connection services. Database Gateway agents can run on servers that have available memory. Therefore, you do not need to separately purchase Elastic Compute Service (ECS), Virtual Private Cloud (VPC), or Express Connect. In terms of data transmission, Database Gateway compresses data before it transmits data over the Internet. This reduces network costs.

* High availability: On-premises servers are configured in disaster recovery mode. You can deploy multiple nodes to implement disaster recovery across servers or data centers. Database Gateway automatically performs disaster recovery across data centers. This ensures that connections can be recovered in seconds after disconnection.

* End-to-end ecosystem services: Database Gateway is gradually integrated with Alibaba Cloud database services to form an end-to-end ecosystem. The ecosystem covers cross-cloud, cloud-based, and on-premises services, which include database migration, disaster recovery, cross-database JOIN operations, data analysis, and data security. Database Gateway allows you to use integrated database services from Alibaba Cloud.



