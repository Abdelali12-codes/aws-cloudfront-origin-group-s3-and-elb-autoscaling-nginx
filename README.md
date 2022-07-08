# cloudfront react with s3 and nginx server

## launchconfiguration

- user data

```
#!/bin/bash
sudo amazon-linux-extras install nginx1 -y
sudo service nginx start
sudo yum install ruby -y
sudo yum install wget -y
cd /home/ec2-user
sudo wget https://aws-codedeploy-us-east-1.s3.amazonaws.com/latest/install
sudo chmod +x ./install
sudo ./install auto

```

## IAM

- create iam policies to allow aws codebuild to make requests
  to amazon s3

- create iam polices to allow aws cloudfront

- attache the above polices to the aws codebuild service role
