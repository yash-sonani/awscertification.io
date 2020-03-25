# AWS Certified Developer Assosiate (DVA-C01) Practise Test 1 #


**Question : 1 ]** As a developer, you have an application running on Amazon EC2. That application needs read-only access to several other AWS services. What is the best practice to grant that application permissions only to a specific set of resources within your aws account?

  1. Use API credentials
  
  2. Use IAM role with ReadOnlyAccess IAM-managed policy
  
  3. Use AWS SDK configuration file and credentials
  
  4. Use IAM role with custom IAM policies for the permissions

 <details>
  <summary><b>Click to get Answer</b></summary>
   <p><b>Option D</b>. Use the custom IAM policy to configure the permissions to a specific set of resources in your account. The ReadOnlyAccess IAM policy restricts write access but grants access to all resources within your account. AWS account credentials are unrestricted. Policies do not go in an SDK configuration file. They are enforced by AWS on the backend.</p>
 </details>

----

**Question : 2 ]** As a developer, you have deployed a application in the US East (Virginia) Region. However, you have accidentally deployed an Amazon Polly lexicon needed for your application in EU (London). How can you use your lexicon to synthesize speech while minimizing the changes to your application code and reducing cost?

  1. Point your SDK client to the EU (London) for all requests to Amazon Polly, but to US East (Virginia) for all other API calls.
  2. No action needed
  3. Upload a copy of the lexicon to US East (Virginia)
  4. Move the rest of the application resources to EU (London)

<details>
   <summary><b>Click to get Answer</b></summary>
<p><b>Option C.</b> This is the simplest approach because only a single resource is in the wrong Region. Option A is a possible approach, but it is not the simplest approach because it introduces cross-region calls that may increase latency and cross-region data transfer pricing.</p>
 </details>

----

