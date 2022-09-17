##This Cloudformation template creates an Amazon EC2 instance running the Amazon Linux AMI. The AMI is chosen based on the region in which the stack is run. This example creates an EC2 security group for the instance to give you SSH access. 

**WARNING** This template creates an Amazon EC2 instance. You will be billed for the AWS resources used if you create a stack from this template.


Steps:
1. Fork this repository by clicking on "Fork". 
2. Clone this repository to your local computer by running following:

   ```$ git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY```
3. Configure AWS CLI in your local machine
4. Run the following command to create the ec2 instance and security group in your AWS account


```
 aws cloudformation deploy \
  --stack-name my-cloudbasic-ec2 \
  --template-file ec2_securitygroup.template \
  --parameter-overrides KeyName=General-key-1
  ```

  Note: Replace "General-key-1" KeyName with your EC2 KeyPair name


Related Resource: https://towardsdatascience.com/cloud-basics-interacting-with-aws-da179d3f5829
