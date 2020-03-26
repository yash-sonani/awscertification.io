# AWS Certified Developer Associate (DVA-C01) Practise Test 1 #


**Question : 1 ]** As a developer, you have an application running on Amazon EC2. That application needs read-only access to several other AWS services. What is the best practice to grant that application permissions only to a specific set of resources within your aws account?

  1. Use API credentials
  
  2. Use IAM role with ReadOnlyAccess IAM-managed policy
  
  3. Use AWS SDK configuration file and credentials
  
  4. Use IAM role with custom IAM policies for the permissions

 <details>
  <summary><b>Click to get Answer</b></summary>
   <p><b>Option 4</b>. Use the custom IAM policy to configure the permissions to a specific set of resources in your account. The ReadOnlyAccess IAM policy restricts write access but grants access to all resources within your account. AWS account credentials are unrestricted. Policies do not go in an SDK configuration file. They are enforced by AWS on the backend.</p>
 </details>

----

**Question : 2 ]** As a developer, you have deployed a application in the US East (Virginia) Region. However, you have accidentally deployed an Amazon Polly lexicon needed for your application in EU (London). How can you use your lexicon to synthesize speech while minimizing the changes to your application code and reducing cost?

  1. Point your SDK client to the EU (London) for all requests to Amazon Polly, but to US East (Virginia) for all other API calls.
  2. No action needed
  3. Upload a copy of the lexicon to US East (Virginia)
  4. Move the rest of the application resources to EU (London)

<details>
   <summary><b>Click to get Answer</b></summary>
<p><b>Option 3.</b> This is the simplest approach because only a single resource is in the wrong Region. Option 1 is a possible approach, but it is not the simplest approach because it introduces cross-region calls that may increase latency and cross-region data transfer pricing.</p>
 </details>

----

**Question : 3 ]** When you are placing subnets for a specific VPC, you can place the subnets in which of the following? 

  1. In any Availability Zone within the Region
  2. In any Availability Zone in any Region
  3. In any AWS edge location
  4. In any specific AWS data center
  
<details>
   <summary><b>Click to get Answer</b></summary>
<p><b>Option 1.</b> Each Amazon VPC is placed in a specific Region and can span all the Availability Zones within that Region. Option 2 is incorrect because a subnet must be placed within the Region for the selected VPC. Option 3 is incorrect because edge locations are not available for subnets, and option 4 is incorrect because you cannot choose specific data centers.</p>
 </details>
 
 ----
 
 **Question : 4 ]** If 2 EC2 Instances have same Private IP, what could be the reason?

  1. Instances are in different VPC
  2. Instances are in different subnets
  3. Instances have different network ACLs
  4. Instances have different security groups
  
<details>
   <summary><b>Click to get Answer</b></summary>
<p><b>Option 1.</b> Even though each instance in an Amazon VPC has a unique private IP address, you could assign the same private IP address ranges to multiple Amazon VPCs. Therefore, two instances in two different Amazon VPCs in your account could end up with the same private IP address. Options 2, 3, and 4 are incorrect because within the same Amazon VPC, there is no duplication of private IP addresses.</p>
 </details>

----

**Question : 5 ]** If your project required high workload like 16,000 consistent IOPS for data that must be durable. What combination of the following is more efficient? (Select TWO.)

  1. Amazon EBS optimized instance
  2. Instance store
  3. Provisioned IOPS SSD volume
  4. Previous-generation EBS volume
  
<details>
   <summary><b>Click to get Answer</b></summary>
<p><b>Option 1 and 3</b> Amazon EBS optimized instances reserve network bandwidth on the instance for I/O, and Provisioned IOPS SSD volumes provide the highest consistent IOPS. Option 2 is incorrect because instance store is not durable. Option 4 is incorrect because a previous-generation EBS volume offers an average of 100 IOPS.</p>
 </details>

----

**Question : 6 ]** Your company stores critical documents in Amazon S3, but it wants to minimize cost. Most documents are used actively for only about one month and then used much less frequently after that. However, all data needs to be available within minutes when requested. How can you meet these requirements?

  1. Migrate the data to Amazon S3 Reduced Redundancy Storage (RRS) after 30 days.
  2. Migrate the data to Amazon S3 Glacier after 30 days.
  3. Migrate the data to Amazon S3 Standard – Infrequent Access (IA) after 30 days.
  4. Turn on versioning and then migrate the older version to Amazon S3 Glacier.
  
<details>
	<summary><b>Click to get Answer</b></summary>
	<p><b>Option 3</b> Migrating the data to Amazon S3 Standard-IA after 30 days using a lifecycle policy is correct. The lifecycle policy will automatically change the storage class for objects aged over 30 days. The Standard-IA storage class is for data that is accessed less frequently, but still requires rapid access when needed. It offers the same high durability, high throughput, and low latency of Standard, with a lower per gigabyte storage price and per gigabyte retrieval fee. Option 1 is incorrect because RRS provides a lower level of redundancy. The question did not state that the customer is willing to reduce the redundancy level of the data, and RRS does not replicate objects as many times as standard Amazon S3 storage. This storage option enables customers to store noncritical, reproducible data. Option 2 is incorrect because the fastest retrieval option for Amazon S3 Glacier is typically 3–5 hours. The customer requires retrieval in minutes. Option 4 is incorrect. Versioning will increase the number of files if new versions of files are being uploaded, which will increase cost. The question did not mention a need for multiple versions of files.</p>
</details>

----

**Question : 7 ]** You have to transfer 3 PB of Data from on-premises to AWS cloud. Which migration option will be good choice with minimal cost and in less time?

  1. AWS Snowball
  2. AWS Snowmobile
  3. Through Internet upload to S3
  4. Amazon Kinesis Data Firehose

<details>
	<summary><b>Click to get Answer</b></summary>
	<p><b>Option 1</b> Option 2 is incorrect. You could use Snowmobile, but that would not be as cost effective because it is meant to be used for datasets of 10 PB or more. Option 3 is incorrect because uploading files directly over the Internet to Amazon S3 would take many months and would be using your on-premises bandwidth. Option 4 is incorrect because Amazon Kinesis Data Firehose would still be transferring over the internet and take months to complete while using your on-premises bandwidth. </p>
</details>

----

**Question : 8 ]** Which of the following AWS service is best for storing session state information of application?

  1. Amazon DynamoDB
  2. Amazon Redshift
  3. AWS Storage Gateway
  4. Amazon Kinesis

<details>
	<summary><b>Click to get Answer</b></summary>
	<p><b>Option 1</b> DynamoDB is a NoSQL database store that is a good alternative because of its scalability, high availability, and durability characteristics. Many platforms provide open source, drop-in replacement libraries that enable you to store native sessions in DynamoDB. DynamoDB is a suitable candidate for a session storage solution in a share-nothing, distributed architecture.</p>
</details>	

----

***Question : 9 ]** As a developer, you need to query 3 TB of data to obtain Report of business. Which of the following AWS service is best for deliver this result?

  1. Amazon EBS
  2. Amazon S3
  3. Amazon RDS
  4. Amazon Redshift
  
<details>
	<summary><b>Click to get Answer</b></summary>
	<p><b>Option 4</b> Amazon Redshift is the best choice for data warehouse workloads that typically span multiple data repositories and are at least 2 TB in size.</p>
</details>	

----

**Question : 10 ]** Your ecommerce application provides daily and ad hoc reporting to various business units on customer purchases. These operations result in a high level of read traffic to your MySQL (Amazon RDS) instance. What can you do to scale up read traffic without impacting your database’s performance?

  1. Increase the allocated storage for the Amazon RDS instance.
  2. Modify the Amazon RDS instance to be a Multi-AZ deployment.
  3. Create a read replica for an Amazon RDS instance.
  4. Change the Amazon RDS instance DB engine version.
  
<details>
	<summary><b>Click to get Answer</b></summary>
	<p><b>Option 3</b> Amazon RDS read replicas provide enhanced performance and durability for Amazon RDS instances. This replication feature makes it easy to scale out elastically beyond the capacity constraints of a single Amazon RDS instance for read-heavy database workloads. You can create one or more replicas of a given source Amazon RDS instance and serve high-volume application read traffic from multiple copies of your data, increasing aggregate read throughput. </p>
</details>	
