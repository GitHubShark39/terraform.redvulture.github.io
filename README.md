# terraform.redvulture.github.io
Engineers - Homework Problem



Security Engineer, For all Engineers - Homework Problem.txt
Timelimit: (3 hours) Truth: This was quite fun and educational, I went over the time limit.


Security Engineer, For all Engineers - Homework Problem - 12/2019
Royal C. Jackson Jr.
Repository

Prerequites:

aws account [Don't trust the free one]
aws cli
terraform cli

C:\Users\redvulture>terraform -version
Terraform v0.10.3

Your version of Terraform is out of date! The latest version
is 0.12.17. You can update by downloading from www.terraform.io

C:\Users\redvulture>
------------------------------------
git repository: 

git clone command: git clone https://github.com/terraform-providers/terraform-provider-aws.git

git clone command: git clone https://github.com/GitHubShark39/terraform.redvulture.github.io.git


Also look at the images directory, it contains all the images
I got my inspiration from, especially:
Stitch-Fix-devops-diagram.png

Serverless Application Model (SAM)
Supported by SAM
AWS Lambda, DynamoDB, API Gateway

Not Supported by SAM
IAM Role, IAM Policy, ACM Certificate for HTTPS API Gateway, 
Cloudwatch Events Scheduler, KMS, Route 53 records for CNAME, etc.


Components of an AWS Lambda Function

1. Testing - 
2. 3rd-Party Packages  - should I just use ipaddress.js?
3. Module Bundler — 3rd-party packages Module Bundler, such as Gulp or Webpack for Node.js.
4. Supporting AWS Resources — supporting resources such as KMS, CloudWatch Logs, etc.
5. Multiple Environments — Integration and Staging before you deploy to Production. 
6. Monitoring -


You may be thinking that all it takes to deploy Lambda with Terraform is to:
1. Create a JavaScript file.
2. Create a Terraform configuration file that references that JavaScript file.
3. Apply Terraform.
4. Lets go Party!

To bring it up, we shall be touching these 4 aws services:
1. Lambda
2. API Gateway
3. DynamoDb
4. IAM (to enable above services to talk to each other)

Notes:

Documentation and a Readme.md is provide due to that I am documenting
as I do my research and write the code in aws lambda and terraform.
I put all documents that I worked on, just look at the time stamps.
Once started, I just had to keep going due to I am not working on 
this on Saturday(12-7-2019), I am watching College Football tomorrow.....

Also I have include some images that I found on the web, which I did
not create them, but use them in reference in understanding the flow
of deploying aws lambda, aws api-gateway, and terraform.

I am going to use this problem as my Cyber Security Project for my
Master of Science in Cybersecurity, with Specialization in Ethical Hacking & Pen Testing
The Ethical Hacking & Pen Testing specialization is designed to provide unique
applications involved in the professional domain of Cyber Security and Information
Assurance (CSIA).


Stitch Fix security team is in the process of implementing Content Security Policy (CSP) 
to detect and mitigate Cross Site Scipting attacks(XSS).

References:
https://www.owasp.org/index.php/Cross-site_Scripting_(XSS)
https://www.owasp.org/index.php/XSS_(Cross_Site_Scripting)_Prevention_Cheat_Sheet


The organization has approximately 50 public facing hostnames where CSP must be implemented.

The security team needs a solution to monitor these hostnames for CSP headers - ensuring 
that they are always present at the root (/) of each hostname.

Write a serverless function which tests for the presence or absense of CSP headers in an 
HTTP response. The function should be deployable to

References:
https://serverless.com/framework/docs/providers/aws/events/apigateway/


SearchOn: serverless function tests CSP headers HTTP

AWS Lambda with an AWS API Gateway for invoking, and it should be deployable with 
Hashicorp Terraform.

Import
aws-lambda-terraform-csp-api can be imported by using the REST API ID, e.g.

$ terraform import aws-lambda-terraform-csp-api 12345abcde


References:
https://serverless.com/framework/docs/providers/aws/events/apigateway/
https://aws.amazon.com/blogs/compute/deploying-a-personalized-api-gateway-serverless-developer-portal/
https://www.terraform.io/docs/providers/aws/r/api_gateway_rest_api.html



SearchOn: AWS Lambda AWS API Gateway deployable Terraform


Additional Guidance


The take-home project evaluates your problem solving and coding skills. 
We want to see that you:

Have the ability to write Infrastructure as Code (Terraform)

Have the ability to write functional code (Lambda)

References:


https://medium.com/better-programming/how-to-build-your-first-serverless-api-with-aws-lambda-and-api-gateway-c7149c2e8d23

https://medium.com/@gsarkar/build-a-csp-report-uri-endpoint-on-aws-serverless-caa6dc843c03

https://developer.mozilla.org/en-US/docs/Web/HTTP/CSP#Sample_violation_report

https://medium.com/faun/hardening-the-http-security-headers-with-aws-lambda-edge-and-cloudfront-2e2da1ae4d83

https://medium.com/faun/hardening-the-http-security-headers-with-aws-lambda-edge-and-cloudfront-2e2da1ae4d83

https://aws.amazon.com/premiumsupport/knowledge-center/custom-headers-api-gateway-lambda/

https://docs.aws.amazon.com/lambda/latest/dg/getting-started.html

https://docs.aws.amazon.com/lambda/latest/dg/gettingstarted-awscli.

https://www.terraform.io/docs/providers/aws/r/api_gateway_deployment.html

https://medium.com/galvanize/aws-lambda-deployment-with-terraform-24d36cc86533

https://www.terraform.io/downloads.html

https://www.terraform.io/docs/cli-index.html

https://www.terraform.io/docs/providers/aws/r/api_gateway_deployment.html

https://www.terraform.io/docs/providers/index.html

https://www.terraform.io/docs/provisioners/index.html

https://dzone.com/articles/terraform-cli-cheat-sheet

https://playcode.io/online-javascript-editor

https://alligator.io/react/index-js-public-interfaces/

https://learn.hashicorp.com/terraform/aws/lambda-api-gateway


Push the code to a private GitHub repo and share it with https://github.com/almostwhitehat

References:
https://help.github.com/en/github/setting-up-and-managing-your-github-user-account/inviting-collaborators-to-a-personal-repository







