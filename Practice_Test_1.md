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

