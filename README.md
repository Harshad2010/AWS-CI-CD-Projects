## End to End MAchine Learning Project

1. Docker Build checked
2. Github Workflow
3. Iam User In AWS
4. Create ECR private repo.
5. Create and Launch EC2 instance and install necesary packages especially related for dockers mentioned in docker setup below.
6. App Runner setup: whenver u do any code commit automatically this runner should trigger and should do deployment, for runn setup : follow instruction given in github itself, for setup and configuration setting: Runner image, Download and configuration instruction just copy paste. your sekf hosted runner should be created which connected with ec2.
7. Run workflow and check.

## Docker Setup In EC2 commands to be Executed

#optinal

sudo apt-get update -y

sudo apt-get upgrade

#required

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker

## Configure EC2 as self-hosted runner:

## Setup github secrets:

AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = us-east-1

AWS_ECR_LOGIN_URI = demo>>  566373416292.dkr.ecr.ap-south-1.amazonaws.com

ECR_REPOSITORY_NAME = simple-app
