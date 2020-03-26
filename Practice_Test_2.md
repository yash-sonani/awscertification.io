# AWS Certified Developer Associate (DVA-C01) Practise Test 2 #


**Question : 1 ]** As a developer, you need to migrate you application database from SQL to NoSQL database. Which AWS service is best solution?

  1. Amazon RDS
  
  2. NoSql database setup on Amazon EC2
  
  3. Amazon DynaoDB
  
  4. Amazon Redshift

 <details>
  <summary><b>Click to get Answer</b></summary>
   <p><b>Option 3.</b> Option 1 and 4 are incorrect because Amazon RDS and Redshift are SQL database. Option 2 is incorrect because NoSQL database setup on Amazon EC2 is not best practice. DynamoDB is a managed NoSQL service. </p>
 </details>

----

**Question : 2 ]** Your company is migrating application which is using Amazon RDS for database. Automatic backup is also enabled. You need to make sure that last backup should be retain. As a developer what should you do?

  1. Delete the database because automatic backup is already enabled.
  2. Create manual snapshot before deleting database.
  3. Use Amazon Database Migration service.
  4. Connect RDS database and perform SQL Dump operation.

<details>
   <summary><b>Click to get Answer</b></summary>
<p><b>Option 2.</b> Automatic backups do not retain the backup after the database is deleted. Therefore, option 1 is incorrect. Option 4 is not possible. Option 3 is incorrect because Amazon DMS is used for Migration Databases from one source to another source.</p>
 </details>

----

**Question : 3 ]** Which not used to run SQL queries in Amazon Redshift?

  1. Compute Node
  2. Cluster Node
  3. Master Node
  4. Leader Node
  
<details>
   <summary><b>Click to get Answer</b></summary>
<p><b>Option 4.</b> The leader node acts as the SQL endpoint and receives queries from applications, parses the queries, and develops query execution plans. Option 1, 2 and 3 are incorrect because Compute node is used for execute the query execution plan, Cluster node and master node are not present in Amazon Redshift.</p>
 </details>
 
 ----
 
 **Question : 4 ]** Which Amazon service is used for graph database?

  1. Amazon RDS
  2. Amazon Neptune
  3. Amazon ElastiCache
  4. Amazon Redshift
  
<details>
   <summary><b>Click to get Answer</b></summary>
<p><b>Option 2.</b> Amazon Neptune is a managed graph database service. Option 1 is incorrect because Amazon RDS is a managed relational database service. Option 3 is incorrect because Amazon ElastiCache is a caching managed database service. Option 4 is incorrect because Amazon Redshift is a data warehouse service.</p>
 </details>

----

**Question : 5 ]** You created one DynamoDB table with partition key and a sort key. A new requirement comes which need to different partition key. As a developer what should you do?

  1. Create a local secondary index.
  2. Create a global secondary index.
  3. Create new DynamoDB table.
  4. Requirement not possible.
  
<details>
   <summary><b>Click to get Answer</b></summary>
<p><b>Option 2.</b> A global secondary index enables you to use a different partition key or primary key in addition to a different sort key. Option 1 is incorrect because a local secondary index can only have a different sort key.Option C is incorrect. Option 3 is incorrect because A new DynamoDB table would not solve the issue. Option 4 is incorrect because it is possible.</p>
 </details>


----

**Question : 6 ]** In your company, an application is using Amazon DynamoDB. Support team noticed that sometime application does not return the most up-to-date data on read operation. As developer, how can you resolve this issue?

  1. Increase RCU of tables.
  2. Increase WCU of tables.
  3. Migrate to SQL database.
  4. Configure the application to perform a strongly consistent read.
  
<details>
	<summary><b>Click to get Answer</b></summary>
	<p><b>Option 4.</b> The application is configured to perform an eventually consistent read, which may not return the most up-to-date data. Option 1 is incorrect because increasing RCUs does not solve the problem. Option 2 is incorrect because this is a read issue, not a write issue. Option 3 is incorrect. There is no need to migrate the database, because the issue is solvable.</p>
</details>

----

**Question : 7 ]** Of all the cryptographic algorithms that the AWS Encryption SDK supports, which one is the default algorithm?

  1. AES-256
  2. AES-192
  3. AES-128
  4. SSH-256

<details>
	<summary><b>Click to get Answer</b></summary>
	<p><b>Option 1.</b> Options 2, 3, and 4 refer to more outdated encryption algorithms. By default, the AWS Encryption SDK uses the industry-recommended AES-256 algorithm.</p>
</details>

----

**Question : 8 ]** Amazon EBS volumes are encrypted by default.

  1. True
  2. False
  
<details>
	<summary><b>Click to get Answer</b></summary>
	<p><b>Option 2.</b> Encryption of Amazon EBS volumes is optional.</p>
</details>	

----

***Question : 9 ]** When you deleting an AWS Elastic Beanstalk environment, Which of the following cannot be retained?

  1. Source code of Git Repository
  2. Data from the automatic backups of an Amazon RDS instance
  3. Packaged code from the source bundle stored in an Amazon S3
  4. Data from the snapshot of an Amazon RDS instance
  
<details>
	<summary><b>Click to get Answer</b></summary>
	<p><b>Option 2.</b> Elastic Beanstalk automatically deletes your Amazon RDS instance when your environment is deleted and does not automatically retain the data. You must create a snapshot of the Amazon RDS instance to retain the data.</p>
</details>	

----

**Question : 10 ]** Which of the following is not part of the AWS Elastic Beanstalk functionality?

  1. Notify the account user of language runtime platform changes
  2. Display events per environment
  3. Show instance statuses per environment
  4. Perform automatic changes to AWS IAM policies
  
<details>
	<summary><b>Click to get Answer</b></summary>
	<p><b>Option 4.</b> Elastic Beanstalk cannot make automated changes to the policies attached to the service roles and instance roles.</p>
</details>	
