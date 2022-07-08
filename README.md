# cloudfront react with s3 and nginx server

# launchconfiguration

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
