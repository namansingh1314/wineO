live demo :https://youtu.be/LtkYIAwEyww
![criteria](https://github.com/namansingh1314/wineO/assets/120774187/0f7aec80-3d9f-4052-a8a5-bdf60aa4b1bd)

![result](https://github.com/namansingh1314/wineO/assets/120774187/af254c7c-b677-46bf-9c64-21671f9e9f91)

## Workflows

1. Update config.yaml
2. Update schema.yaml
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline 
8. Update the main.py
9. Update the app.py



# How to run?
### STEPS:

Clone the repository

```bash
https://github.com/namansingh1314/wineO
```
### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n mlproj python=3.9 -y
```

```bash
conda activate mlproj
```


### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```


```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up you local host and port
```



## MLflow

[Documentation](https://mlflow.org/docs/latest/index.html)


##### cmd
- mlflow ui

### dagshub
[dagshub](https://dagshub.com/)

MLFLOW_TRACKING_URI=https://dagshub.com/api/v1/repo-buckets/s3/namansingh1314 \
MLFLOW_TRACKING_USERNAME=namansingh1314  \
MLFLOW_TRACKING_PASSWORD=006f1e3cebab3d0b3b301a7b8d0bd938d6461456 \
python script.py

Run this to export as env variables:

```bash

export MLFLOW_TRACKING_URI=https://dagshub.com/api/v1/repo-buckets/s3/namansingh1314

export MLFLOW_TRACKING_USERNAME=namansingh1314 

export MLFLOW_TRACKING_PASSWORD=006f1e3cebab3d0b3b301a7b8d0bd938d6461456

```



# AWS-CICD-Deployment-with-Github-Actions

## 1. Login to AWS console.

## 2. Create IAM user for deployment

	#with specific access

	1. EC2 access : It is virtual machine

	2. ECR: Elastic Container registry to save your docker image in aws


	#Description: About the deployment

	1. Build docker image of the source code

	2. Push your docker image to ECR

	3. Launch Your EC2 

	4. Pull Your image from ECR in EC2

	5. Lauch your docker image in EC2

	#Policy:

	1. AmazonEC2ContainerRegistryFullAccess

	2. AmazonEC2FullAccess

	
## 3. Create ECR repo to store/save docker image
    - Save the URI: 952344816757.dkr.ecr.ap-south-1.amazonaws.com/wine-o

	
## 4. Create EC2 machine (Ubuntu) 

## 5. Open EC2 and Install docker in EC2 Machine:
	
	
	#optinal

	sudo apt-get update -y

	sudo apt-get upgrade
	
	#required

	curl -fsSL https://get.docker.com -o get-docker.sh

	sudo sh get-docker.sh

	sudo usermod -aG docker ubuntu

	newgrp docker
	
# 6. Configure EC2 as self-hosted runner:
    setting>actions>runner>new self hosted runner> choose os> then run command one by one


# 7. Setup github secrets:

    AWS_ACCESS_KEY_ID=

    AWS_SECRET_ACCESS_KEY=

    AWS_REGION = us-east-1

    AWS_ECR_LOGIN_URI = demo>>  566373416292.dkr.ecr.ap-south-1.amazonaws.com

    ECR_REPOSITORY_NAME = simple-app




## About MLflow 
MLflow

 - Its Production Grade
 - Trace all of your expriements
 - Logging & tagging your model
![actionsrunner](https://github.com/namansingh1314/wineO/assets/120774187/2758ad8e-1816-4c2c-8d41-b203cf22ac03)

![ec2ubuntu](https://github.com/namansingh1314/wineO/assets/120774187/4f383ba8-7bf0-4b6c-9aa2-6dc2976c1376)

![firstec2instance](https://github.com/namansingh1314/wineO/assets/120774187/5aeb56c3-995c-4a58-bd23-7f5b386e996a)


