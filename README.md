# LambdaFunctiontoRotateSecretKeys

Rotate Secret Keys in AWS Using Lambda functions.

Excited to share the successful deployment of AWS Lambda functions to Rotate Secret Keys

how to effectively use Lambda functions to automate secret rotation in AWS. Managing sensitive information like API keys, database passwords, or encryption keys is crucial for security, and AWS Lambda can help streamline this process. I created the Lambda Function with the runtime versions python3.9 Using Boto3 Module. Also I will elaborate step-by-step guidance on setting up Lambda functions, writing the necessary code, and configuring them to automatically rotate secrets. Enhance your AWS security and simplify secret management with this comprehensive guide. 

Step1. We use Secrets Manager to store, rotate, monitor, and control access to secrets such as database credentials, API keys, and OAuth tokens. After storing  the Secrets in Secret Manager I am going to turn on rotation for  secrets using AWS Lambda functions. To retrieve secrets, you simply replace hardcoded secrets in applications with a call to Secrets Manager APIs, eliminating the need to expose plaintext secrets.

Step 2 . Created a lambda function using Python 3.9 runtime  using boto3 module. 
Step3. But we have to  give permission to lambda function as well.  I have to add the permission  LambdainvokeFunction. 
Step4: Also we have to create the inline policy inside Lambda function in order to rotate the secret.  To create policy click on the incline policy  and add Json policy.
Step5: After policy and Permission has been setup I just have to deploy the code 
Step6: Once Lambda Function Deployed , enable the automatic rotation enable and select the Lambda functions as Rotation function , with proving the timeframe I have to rotate after.

In code Lambda function rotate the secret with random number. And the Major benefits of this lab can provide us are 

Rotate secrets safely
Easily rotate secrets and enable users and applications to retrieve the most recent secret without a code deployment.

Manage access with fine-grained permissions
Control access to secrets using fine-grained permissions with AWS Identity and Access Management policies.


I did Rotate the keys immediately to make sure my code is working fine. 
I have pushed the code con my GitHub repository : https://github.com/IamsinghJaskaran/LambdaFunctiontoRotateSecretKeys.git
Improved my understanding of using  Severless  architecture using python scripts to achieve Security for application. 
Excited to continue exploring new technologies and methodologies in the DevOps space!
