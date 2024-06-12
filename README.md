# mlflow_experiment_tracking


## For Dagshub Integration

```https://dagshub.com/donadviser/mlflow_experiment_tracking.mlflow

import dagshub
dagshub.init(repo_owner='donadviser', repo_name='mlflow_experiment_tracking', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)
```

# MLFlow on AWS

## MLFlow on AWS Setup

1. Login to AWS console
2. Create IAM user with AdminsitratorAccess
3. Export the credentials in your AWS CLI by running `aws configure`
2. Create an S3 bucket
5. Create EC2 machine (ubuntu) & add security groups 5000 port

Run the following command on EC2 machine

```bash

sudo apt update

sudo apt install python3-pip

sudo pip3 install pipenv

sudo pip3 install virtualenv

mkdir mlflow

cd mlflow

pipenv install mlflow

pipenv install awscli

pipenv install boto3

pipenv shell

## Set AWS Credentials

aws configure

```



